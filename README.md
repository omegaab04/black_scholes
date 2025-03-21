Here, I'm using the **Black-Scholes model** to value a European Call Option... with a twist.

I have written the magic in C, but you can call it from Python directly. Just enter the relevant parameters that exist in the model.
---
## Play around with it:

### **Clone Repo**
```sh
git clone https://github.com/your-username/black_scholes.git
cd black_scholes
```

### **Dependencies**
```sh
pip install --upgrade setuptools wheel
```

### **C Extension**
```sh
python setup.py build_ext --inplace
```

### **Install the Package**
```sh
pip install -e .
```

---

## Usage Example

```python
import bs

s = 163.80      # Spot price
k = 900     # Strike price
r = 0.0016       # Risk-free rate
t = 80/365      # Time to expiration (60 days)
sigma = 0.15    # Volatility

return bs.bs_call(s, k, r, t, sigma)

You should obtain: 

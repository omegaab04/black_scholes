Here, I'm using the **Black-Scholes model** for European options pricing. 
---
## Play around with it:

### **1⃣ Clone the Repository**
```sh
git clone https://github.com/your-username/black_scholes.git
cd black_scholes
```

### **2⃣ Create & Activate a Virtual Environment**
```sh
python3 -m venv .venv
source .venv/bin/activate  # macOS/Linux
# On Windows, use: .venv\Scripts\activate
```

### **3⃣ Install Dependencies**
```sh
pip install --upgrade setuptools wheel
```

### **4⃣ Build the C Extension**
```sh
python setup.py build_ext --inplace
```

### **5⃣ Install the Package**
```sh
pip install -e .
```

---

## 🔥 Usage Example

```python
import black_scholes

s = 147.30      # Spot price
k = 150.0       # Strike price
r = 0.001       # Risk-free rate
t = 60/365      # Time to expiration (60 days)
sigma = 0.45    # Volatility

price = black_scholes.bs_call(s, k, r, t, sigma)
print(f"Black-Scholes Call Option Price: {price}")
```

### **📈 Expected Output**
```
Black-Scholes Call Option Price: 9.518562265392418
```

---

## 🛠️ Development & Contribution
We welcome contributions! Follow these steps to contribute:

1. **Fork** the repository.
2. Clone your forked repo:
   ```sh
   git clone https://github.com/your-username/black_scholes.git
   ```
3. Create a new branch:
   ```sh
   git checkout -b feature-name
   ```
4. Make changes and commit:
   ```sh
   git add .
   git commit -m "Added new feature"
   ```
5. Push changes:
   ```sh
   git push origin feature-name
   ```
6. Create a **Pull Request** on GitHub.

---

## ⚖️ License
This project is licensed under the **MIT License**. See [LICENSE](LICENSE) for details.

---

## 💬 Contact & Support
If you have any questions or feature requests, feel free to **open an issue** on GitHub or reach out to:

💎 **Your Email**: your-email@example.com  
🐦 **Twitter**: [@yourusername](https://twitter.com/yourusername)  
📢 **LinkedIn**: [Your Profile](https://linkedin.com/in/yourusername)

---

## ⭐ Support the Project
If you find this project useful, **please give it a star ⭐ on GitHub!**


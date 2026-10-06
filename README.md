# 🔐 Affine Cipher Tool

A simple, modern web tool to **encrypt and decrypt text** using the Affine Cipher, built with plain HTML, CSS and JavaScript. No libraries, no installation, no backend.

---

## ✨ Features

- Encrypt and decrypt with one click using the Encrypt / Decrypt tabs
- Live results that update as you type
- Key `a` dropdown that offers only valid values (coprime with 26) and shows its modular inverse
- Handles any value of `b`, including negative and large numbers
- Preserves letter case, spaces, digits and symbols
- Shows the active formula for the chosen keys
- Copy to clipboard and a quick "use output as input" button
- Responsive dark UI that works on desktop and mobile

---

## 🧠 How the Affine Cipher Works

Each letter is converted to a number (A = 0, B = 1, ... Z = 25), then transformed:

| Operation | Formula |
|-----------|---------|
| Encryption | `E(x) = (a·x + b) mod 26` |
| Decryption | `D(y) = a⁻¹·(y − b) mod 26` |

- `a` and `b` are the secret keys.
- `a` must be **coprime with 26**, so the valid values are `1, 3, 5, 7, 9, 11, 15, 17, 19, 21, 23, 25`.
- `a⁻¹` is the modular inverse of `a` mod 26, meaning `a × a⁻¹ ≡ 1 (mod 26)`.

Example

With `a = 5` and `b = 8`:

```
Plaintext  : HELLO
Ciphertext : RCLLA
```

---

## 🚀 How to Use

1. Open `index.html` (or `affine_cipher.html`) in any web browser.
2. Choose **Encrypt** or **Decrypt**.
3. Type or paste your message.
4. Select the key `a` and enter the key `b`.
5. Copy the result.

To run it locally:

---

## 🛠️ Built With

- HTML5
- CSS3 (glassmorphism-style dark theme)
- Vanilla JavaScript

---

## ⚠️ Disclaimer

The Affine Cipher is a classical cipher and is **not secure** for real-world data.
This project is for learning and demonstration purposes only. project is for learning and demonstration purposes only.

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

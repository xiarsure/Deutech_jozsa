# 🧠 Deutsch-Jozsa Algorithm with Qiskit

This project demonstrates the **Deutsch-Jozsa quantum algorithm** using [Qiskit](https://qiskit.org/), simulating both **constant** and **balanced** oracles.

---

## 📌 Overview

The **Deutsch-Jozsa algorithm** determines whether a given Boolean function `f(x): {0,1}ⁿ → {0,1}` is:

* **Constant**: outputs the same value for all inputs (either always 0 or always 1), or
* **Balanced**: outputs 0 for exactly half of the inputs and 1 for the other half.

This quantum algorithm solves the problem in **one evaluation**, while a classical algorithm could require up to $2^{n-1} + 1$ evaluations in the worst case.

---

## 🧪 What This Code Does

* Creates a **constant oracle** that returns the same output regardless of input.
* Creates a **balanced oracle** using CNOT gates.
* Builds and runs the Deutsch-Jozsa quantum circuit.
* Simulates the circuit using Qiskit Aer.
* Visualizes the output using a histogram.

---

## 📂 File Structure

```bash
.
├── deutsch_jozsa.ipynb  # Main code in Jupyter Notebook or script
├── README.md            # You're here
```

---

## ⚙️ How to Run

1. **Install Qiskit**:

   ```bash
   pip install qiskit qiskit-aer matplotlib
   ```

2. **Run the script/notebook**:

   * Use a Jupyter notebook environment (recommended) or
   * Convert to `.py` and run via Python.

---

## 📈 Output

* **Constant oracle result**: always `'000'` (for 3-qubit example).
* **Balanced oracle result**: any non-zero bitstring (e.g., `'101'`).

---

## 🧩 Customization

* Change `n = 3` to use more or fewer qubits.
* Toggle between using `const_Oracle` or `balance_oracle` when composing the main circuit.

---

## 📜 License

This project is for educational use under the MIT License.

---

## 🤖 Author

Built with ❤️ using Qiskit.
Feel free to fork, remix, or plug it into your own quantum learning tools.

# 🌡️ Simple Temperature Converter

A straightforward Python script for converting temperatures between **Celsius (°C)** and **Fahrenheit (°F)**.

---

## 🚀 How to Use

1.  **Save the Code:** Save the provided Python code into a file named (for example) `temp_converter.py`.
2.  **Run in Terminal:** Execute the script using your Python interpreter:

    ```bash
    python temp_converter.py
    ```
3.  **Follow Prompts:** The script will ask you to specify the initial unit (**C** or **F**) and the temperature value.

---

##  formulas

The conversions are based on the standard formulas:

* **Celsius to Fahrenheit:**
    $$F = (C \times 9/5) + 32$$
* **Fahrenheit to Celsius:**
    $$C = (F - 32) \times 5/9$$

---

## 📜 Source Code

```python
unit = input("Is this temperature in Celsius or Fahrenheit (C/F): ")
temp = float(input("Enter the temperature: "))

if unit == "C":
    temp = round((9 * temp) / 5 + 32, 1)
    print(f"The temperature in Fahrenheit is: {temp}°F")
elif unit == "F":
    temp = round((temp - 32) * 5 / 9, 1)
    print(f"The temperature in Celsius is: {temp}°C")
else:
    print(f"{unit} is an invalid unit of measurement")

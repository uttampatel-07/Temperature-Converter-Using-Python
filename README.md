🌡️ Temperature ConverterA simple Python script to convert temperatures between Celsius (°C) and Fahrenheit (°F).🚀 UsageSave the code as a Python file (e.g., temp_converter.py).Run the script in your terminal:Bashpython temp_converter.py
The script will prompt you to enter the initial unit (C or F) and the temperature value.Conversion Formulas Used:C to F: $F = (C \times 9/5) + 32$F to C: $C = (F - 32) \times 5/9$📜 CodePythonunit = input("Is this temperature in Celsius or Fahrenheit (C/F): ")
temp = float(input("Enter the temperature: "))

if unit == "C":
    temp = round((9 * temp) / 5 + 32, 1)
    print(f"The temperature in Fahrenheit is: {temp}°F")
elif unit == "F":
    temp = round((temp - 32) * 5 / 9, 1)
    print(f"The temperature in Celsius is: {temp}°C")
else:
    print(f"{unit} is an invalid unit of measurement")
✍️ Author

import math

def length_converter():
    print("\nLength Converter:")
    meters = float(input("Enter length in meters: "))
    print("Length in Centimeters:", meters * 100)
    print("Length in Kilometers:", meters / 1000)

def mass_converter():
    print("\nMass Converter:")
    kilograms = float(input("Enter mass in kilograms: "))
    print("Mass in Grams:", kilograms * 1000)
    print("Mass in Pounds:", kilograms * 2.20462)

def height_calculator():
    print("\nHeight Calculator:")
    feet = float(input("Enter height in feet: "))
    print("Height in Meters:", feet * 0.3048)

def simple_interest_calculator():
    print("\nSimple Interest Calculator:")
    principal = float(input("Enter principal amount: "))
    rate = float(input("Enter annual interest rate: "))
    time = float(input("Enter time in years: "))
    interest = (principal * rate * time) / 100
    print("Simple Interest:", interest)

def electricity_calculator():
    print("\nElectricity Calculator:")
    voltage = float(input("Enter voltage: "))
    current = float(input("Enter current: "))
    resistance = voltage / current
    power = voltage * current
    print("Resistance:", resistance, "Ohms")
    print("Power:", power, "Watts")

def main():
    while True:
        print("\nUniversal Calculator")
        print("1. Length Converter")
        print("2. Mass Converter")
        print("3. Height Calculator")
        print("4. Simple Interest Calculator")
        print("5. Electricity Calculator")
        print("6. Exit")

        choice = input("Enter your choice (1-6): ")

        if choice == "1":
            length_converter()
        elif choice == "2":
            mass_converter()
        elif choice == "3":
            height_calculator()
        elif choice == "4":
            simple_interest_calculator()
        elif choice == "5":
            electricity_calculator()
        elif choice == "6":
            print("Exiting the calculator.")
            break
        else:
            print("Invalid choice. Please enter a number between 1 and 6.")

if __name__ == "__main__":
    main()

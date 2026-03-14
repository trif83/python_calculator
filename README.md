num1 = float(input("Първо число: "))
operator = input("Оператор (+, -, *, /, %, //): ")
num2 = float(input("Второ число: "))

result = 0
if operator == "+":
    result = num1 + num2
elif operator == "-":
    result = num1 - num2
elif operator == "*":
    result = num1 * num2
elif operator == "/":
    if num2 != 0:
        result = num1 / num2
    else:
        print("Грешка: деление на нула")
        exit()
elif operator == "%":
    result = num1 % num2
elif operator == "//":
    result = num1 // num2
else:
    print("Невалиден оператор")
    exit()

print("Резултат:", result)

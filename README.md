# calicalator-by-python

while True:
    try:
        # إدخال الرقم الأول
        num1 = float(input("Enter first number: "))

        # إدخال العملية
        operation = input("Enter operation type (+, -, *, /) or 'q' to quit: ")

        # التحقق مما إذا كان المستخدم يريد الخروج
        if operation.lower() == 'q':
            print("Calculator exiting...")
            break

        # إدخال الرقم الثاني
        num2 = float(input("Enter second number: "))

        # إجراء العملية الحسابية وإظهار النتيجة
        if operation == "+":
            print("Result:", num1 + num2)
        elif operation == "-":
            print("Result:", num1 - num2)
        elif operation == "*":
            print("Result:", num1 * num2)
        elif operation == "/":
            if num2 == 0:
                print("Error: Division by zero is not allowed.")
            else:
                print("Result:", num1 / num2)
        else:
            print("Error: Invalid operation.")

    except ValueError:
        print("Error: Please enter a valid number.")



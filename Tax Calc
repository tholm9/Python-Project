headline = {"Employee Name": [], "Hours Worked": [], "Pay Rate": [], "Regular Pay": [], "OT Pay": [], "Gross Pay": [],
            "Fed Tax": [], "State Tax": [], "FICA": [], "NetPay": []}
for x in range(10):
    name = input("What is the employee name? ")
    print("Hello" + " " + name + "!")
    hours = input("How many hours did you work? ")
    rate = input("Please enter your hourly rate. ")
    reg = (int(hours) * float(rate))
    reg = round(reg, 2)
    # print("Your regular pay is " + str(reg))
    othours = int(hours) - 40
    ot = 1.5 * float(rate) * float(othours)
    if int(hours) > 40:
        # print("Your overtime pay is " + str(ot))
        headline["OT Pay"].append(ot)
    else:
        ot = 0
    gross = int(reg) + int(ot)
    gross = round(gross, 2)
    # print("Your gross pay is " + str(gross))
    headline["Gross Pay"].append(gross)

    tax = float(gross) * (0.1 + 0.06 + 0.03)
    netpay = float(gross) - float(tax)
    netpay = round(netpay, 2)
    # print("Your net pay is " + str(netpay))
    headline["Employee Name"].append(name)
    headline["Pay Rate"].append(rate)
    headline["Regular Pay"].append(reg)
    headline["Hours Worked"].append(hours)
    headline["NetPay"].append(netpay)
    headline["Fed Tax"].append(str(10) + "%")
    headline["State Tax"].append(str(6) + "%")
    headline["FICA"].append(str(3) + "%")

    print(headline)

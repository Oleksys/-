# -
дз
coin1 = int(input("Введіть номінал монети 1: "))
coin2 = int(input("Введіть номінал монети 2: "))
number = int(input("Введіть загальну суму: "))

if coin1 > coin2:
    num_coin1 = number // coin1
    remaining_amount = number % coin1
    num_coin2 = remaining_amount // coin2
else:
    num_coin2 = number // coin2
    remaining_amount = number % coin2
    num_coin1 = remaining_amount // coin1

remaining_amount = remaining_amount % coin1 if coin1 > coin2 else remaining_amount % coin2

print("Кількість монети 1:", num_coin1)
print("Кількість монети 2:", num_coin2)
print("Залишок суми:", remaining_amount)

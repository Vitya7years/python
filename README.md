money = float(input("Введите сумму вклада: "))

per_cent = {'ТКБ': 5.6, 'СКБ': 5.9, 'ВТБ': 4.28, 'СБЕР': 4.0}

deposit = {}
for bank, percent in per_cent.items():
    deposit[bank] = money * (percent / 100)

print("Накопленные средства за год в разных банках:")
for bank, amount in deposit.items():
    print(f"{bank}: {amount:.2f}")

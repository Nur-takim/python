import math

def kenar_hesapla(x1, y1, x2, y2):
    return math.sqrt((x2 - x1)**2 + (y2 - y1)**2)

# Üçgenin köşe noktalarının koordinatlarını kullanıcıdan al
x1, y1 = map(float, input("Birinci köşe noktasının koordinatlarını girin (x1 y1): ").split())
x2, y2 = map(float, input("İkinci köşe noktasının koordinatlarını girin (x2 y2): ").split())
x3, y3 = map(float, input("Üçüncü köşe noktasının koordinatlarını girin (x3 y3): ").split())

# Kenar uzunluklarını hesapla
kenar1 = kenar_hesapla(x1, y1, x2, y2)
kenar2 = kenar_hesapla(x2, y2, x3, y3)
kenar3 = kenar_hesapla(x3, y3, x1, y1)

print(f"Birinci kenar uzunluğu: {kenar1:.2f}")
print(f"İkinci kenar uzunluğu: {kenar2:.2f}")
print(f"Üçüncü kenar uzunluğu: {kenar3:.2f}")

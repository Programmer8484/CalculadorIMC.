# CalculadorIMC.

#Calcular IMC de una persona. IMC = masa / (estatura ^ 2).
try:
    peso=int(input("Escriba su peso:"))
except ValueError:
    print("Escriba números, no letras.")
try:
    estatura=float(input("Escriba su estatura:"))
except ValueError:
    print("Escriba números, no letras.")

IMC=peso/(estatura**2)
print(f"\nSu IMC es de:{IMC:.2f}, y tiene ")
if IMC>30:
    print("obesidad.")
elif IMC==25.0 or -29.9:
    print("peso superior al normal.")
elif IMC<18.5:
    print("peso inferior al normal.")

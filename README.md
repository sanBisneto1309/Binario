dividendo = int(input("Insira um numero para converter em binario: "))
numero_digitado = dividendo
quociente = 1
lista = []

while quociente >= 1:
  resto = dividendo % 2
  lista.insert(0, resto)
  quociente = dividendo // 2
  dividendo = quociente

binario = ''.join([str(item) for item in lista])
print("O número em binário é " + binario)

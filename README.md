# Aulas-de-POO
# tabela de multiplicação do 5 até o 15
inicio = 5
fim = 15

for i in range(inicio, fim +1):
  for j in range(inicio , fim +1):
    resultado = i * j
    print(f'{i}*{j} = {resultado}')
  print()



# cpf informado
cpf_informado = input("Digite o numero de cpf: ")
num_digitos = len(cpf_informado)
if num_digitos == 11:
  print("cpf válido")
else:
  print("cpf inválido")



# Fibonacci
num = int(input("Digite um numero: "))
fib_serie = [0,1]
if num <= 1:
  print("A série de Fibonacci até", num, "é:")
  while len(fib_serie) < num:
    fib_serie.append(fib_serie[-1] + fib_serie[-2])
  print("A serie de Fibonacci até", num , "é", fib_serie[:num])
else:
  while len(fib_serie)< num + 1:
    fib_serie.append(fib_serie[-1] + fib_serie[-2])
  print("A serie de Fibonacci até", num , "é", fib_serie[:num])



# Investimento mensal
investimento_mes = float(input("Informe o investimento mensal: "))
taxa_juro_mes = float(input("Informe a taxa de juro mensal: "))
saldo_ano = 0
ano = 1
while True:
  saldo = saldo_ano
  for mes in range(1,13):
      # saldo += investimento_mes
      saldo += saldo * taxa_juro_mes
  print(f"Saldo do investimento após {ano} ano(s): R$ {saldo:.2f}")
  resposta =input("Deseja fazer um novo calculo?(S/N)")
  if resposta != "S":
    break
  ano += 1
print(f"Saldo no final do ano:",saldo)



# valor aproximado do pi
num_termos = int(input("Digite um numero: "))
pi = 0
for i in range(num_termos):
  pi += 2 * (-1)** i / (2 * i + 1)
  print(f"valor aproximado de pi:",pi)



# validar cpf
cpf_informado = input("Digite o número de CPF (somente números): ")
if len(cpf) != 11:
    print("CPF inválido: O CPF deve conter 11 dígitos.")
else:
    print("cpf valido")






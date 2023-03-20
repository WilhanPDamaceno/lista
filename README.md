# lista




# Esse algoritmo tem o objetivo calcular o valor de uma folha de pagamento de um funcionário de uma empresa. Para tanto
# ele irá seguir os seguintes passos:
# coletar as seguintes informações: Nome ; quantidade de horas trabalhadas no mês;
# turno de trabalho (M = Matutino, V = Vespertino e N = Noturno) categoria (G = Gerente e O = Operário)
# b) Salvar as informações dos funcionários em uma lista, não permitindo que sejam informados turnos e categorias
# inexistentes e não aceitar valores vazios e/ou nulos.
# c) Calcular o valor da hora trabalhada conforme a tabela a seguir.
# (Adotar o valor de R$ 1.320,00 para o salário mínimo.)
# Categoria Turno Valor da hora trabalhada
# G = N 10% do salário mínimo
# G = M ou V 15% do salário mínimo
# O = N 9% do salário mínimo
# O = M ou V 14% do salário mínimo
# d) Calcule e mostre o salário de cada funcionário com base nas horas trabalhadas e
# no valor calculado para hora trabalhada de cada funcionário.
#////////////////////////////////////////////////////////////////////////////////////////////




CATEROGIAS = ["Gerente", "Operacional"]
salario = 1320
PORCENTAGENS = {"Gerente": {"Noturno": 0.10,
                            "Matutino": 0.15,
                            "Vespertino": 0.15},
                'Operacional': {"Noturno": 0.09,
                                            "Matutino": 0.14,
                                            "Vespertino": 0.14, }}

nome = input("Digite seu  nome: ")
horasTrabalhadas = int(input("Digite a quantidade de horas trabalhadas no mês: "))
TURNO = input("Qual seu turno Turno {TURNO}: ")
CATEROGIAS categoria = input(" Qual a sua Categoria ? {CATEROGIAS}: ")


valorHoraTrabalhada = PORCENTAGENS[CATEROGIAS][TURNO]

TOTAL_A_RECEBER = (valorHoraTrabalhada * SM) * horasTrabalhadas

print(f"{nome}, O seu salário é de R${TOTAL_A_RECEBER}")

SALARIO = (int (1320))

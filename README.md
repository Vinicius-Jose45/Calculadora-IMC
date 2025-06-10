# Calculadora-IMC
Calculadora de IMC (simples).
nome = input("Digite seu nome: ")
idade = int(input("Digite sua idade: "))

peso = float(input("Por favor, introduza o seu peso (em kg): "))
altura = float(input("Por favor, introduza a sua altura (em metros): "))

imc = peso / (altura ** 2)

print('Nome =', nome)
print('Idade =', idade)
print('Peso =', peso)
print('Altura =', altura)
print(f'O seu IMC é: {imc:.2f}')

if imc < 18.5:
    print("Você está abaixo do peso.")
elif 18.5 <= imc < 25:
    print("Você está no peso ideal.")
elif 25 <= imc < 30:
    print("Você está com sobrepeso.")
elif 30 <= imc < 35:
    print("Você está com obesidade grau 1.")
elif 35 <= imc < 40:
    print("Você está com obesidade grau 2.")
else:
    print("Você está com obesidade grau 3.")

nom = str(input('Gostaria de saber o significado? '))

lista = ['sim','s','claro','obvio']
lista_not =['não','n']
if nom in lista:
    print('Certo')
if nom in lista_not:
    print('ok')

classificacao = str(input('Digite a classificação ou grau de obesidade:'
                          'OBS: abixo do peso, peso ideal, sobre peso, obesidade grau 1, 2 ou 3. '))

classi = ['abaixo do peso',]
if classificacao in classi:
    print('De acordo com o Índice de Massa Corporal (IMC), uma pessoa é considerada abaixo do peso se o resultado da sua avaliação for menor do que 18,5. Este valor indica que a pessoa tem uma relação entre peso e altura que pode estar relacionada a um risco de saúde ou desnutrição.')
classi = ['peso ideal']
if classificacao in classi:
    print('De acordo com o Índice de Massa Corporal (IMC), o peso ideal é aquele que se encontra na faixa entre 18,5 e 24,9 kg/m². Um IMC acima de 25 indica sobrepeso, e um IMC a partir de 30 indica obesidade, com diferentes graus de severidade.')
classi = ['sobrepeso']
if classificacao in classi:
    print('Segundo o Índice de Massa Corporal (IMC), uma pessoa está acima do peso quando seu IMC está entre 25 e 29,9. O IMC é um indicador que estima o peso corporal em relação à altura, sendo um valor entre 25 e 29,9 considerado sobrepeso.')
classi = ['grau 1']
if classificacao in classi:
    print('Segundo o Índice de Massa Corporal (IMC), a obesidade grau 1 é caracterizada por um IMC entre 30 e 34,9 kg/m². Este estágio de obesidade indica um excesso de peso moderado, que pode aumentar os riscos para a saúde.')
classi = ['grau 2']
if classificacao in classi:
    print('A obesidade grau 2, de acordo com o Índice de Massa Corporal (IMC), é definida como um IMC entre 35 e 39,9 kg/m². Esta condição é considerada uma obesidade leve ou moderada, indicando um excesso de gordura corporal que pode afetar a saúde e o bem-estar.')
classi = ['grau 3']
if classificacao in classi:
    print('Se

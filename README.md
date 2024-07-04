# C-digos-em-Python
# CALCULO DE IMC - indice de massa corporal

# menor que 18,5 - magreza
# entre 18,5 e 24,9 - normal
# entre 25,0 e 29,9 - sobrepeso 
# entre 30,0 e 39,9 - obesidade
# maior que 40,0 - obesidade grave



alt = float(input('Qual sua altura em cm? '))
peso = float(input('Qual seu peso em Kg? '))


imc = peso / (alt/100)**2      # dividido p 100 para transformar em metros


if imc < 18.5:
  print(f'Seu IMC é de {imc}, e é classificado como Magreza')
elif imc >= 18.5 and imc < 24.9:
  print(f'Seu IMC é de {imc}, e é classificado como Normal')

elif imc >= 25.0 and imc < 29.9:
  print(f'Seu IMC é de {imc}, e é classificado como Sobrepeso')

elif imc >= 30.0 and imc < 39.9:
  print(f'Seu IMC é de {imc}, e é classificado como Obesidade')

else:
  print(f'Seu IMC é de {imc}, e é classificado como Obesidade Grave')


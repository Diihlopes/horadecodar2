# horadecodar2
HORA DE CODAR 2
var numero1 = prompt("Digite o primeiro número:");
var numero2 = prompt("Digite o segundo número:");

// Converte os valores para números
numero1 = parseFloat(numero1);
numero2 = parseFloat(numero2);

// Verifica qual número é o maior
var maiorNumero;
if (numero1 > numero2) {
  maiorNumero = numero1;
} else if (numero2 > numero1) {
  maiorNumero = numero2;
} else {
  maiorNumero = "Os números são iguais.";
}

// Exibe o maior número
alert("O maior número é: " + maiorNumero);
valor = float(input("Digite um valor: "))

if valor > 0:
    print("O valor informado é positivo.")
elif valor < 0:
    print("O valor informado é negativo.")
else:
    print("O valor informado é zero.")
    valor1 = float(input("Digite o primeiro valor: "))
valor2 = float(input("Digite o segundo valor: "))
valor3 = float(input("Digite o terceiro valor: "))

if valor1 > valor2 and valor1 > valor3:
    maior = valor1
elif valor2 > valor1 and valor2 > valor3:
    maior = valor2
else:
    maior = valor3

print("O maior valor é:", maior)
valor1 = float(input("Digite o primeiro valor: "))
valor2 = float(input("Digite o segundo valor: "))
valor3 = float(input("Digite o terceiro valor: "))

if valor1 > valor2 and valor1 > valor3:
    maior = valor1
    if valor2 > valor3:
        segundo_maior = valor2
    else:
        segundo_maior = valor3
elif valor2 > valor1 and valor2 > valor3:
    maior = valor2
    if valor1 > valor3:
        segundo_maior = valor1
    else:
        segundo_maior = valor3
else:
    maior = valor3
    if valor1 > valor2:
        segundo_maior = valor1
    else:
        segundo_maior = valor2

soma_maiores = maior + segundo_maior
print("A soma dos dois maiores valores é:", soma_maiores)
valores = []

for i in range(6):
    valor = float(input(f"Digite o {i+1}º valor: "))
    valores.append(valor)

print("Números informados:", valores)

soma = sum(valores)
media = soma / len(valores)

print("Média aritmética dos valores:", media)
valores = []

for i in range(4):
    valor = float(input(f"Digite o {i+1}º valor: "))
    valores.append(valor)

primeiro_valor = valores[0]
ultimo_valor = valores[-1]
maior_valor = max(valores)

print("Primeiro valor:", primeiro_valor)
print("Último valor:", ultimo_valor)
print("Maior valor:", maior_valor)  
soma = 0
valores = []

for i in range(6):
    valor = float(input(f"Digite o {i+1}º número: "))
    valores.append(valor)
    
    if valor < 72:
        soma += valor

print("Valores informados:", valores)
print("Valor final da soma dos números inferiores a 72:", soma)
numeros = []

for i in range(4):
    numero = float(input(f"Digite o {i+1}º número: "))
    if numero > 0 and numero < 10:
        numeros.append(numero)
    else:
        print("Os números devem ser maiores que 0 e menores que 10. Tente novamente.")
        exit()

media = sum(numeros) / len(numeros)

if media > 5:
    print("Você passou no teste.")
else:
    print("Tente novamente.")
    from datetime import date

ano_atual = date.today().year
ano_nascimento = int(input("Digite o ano de nascimento: "))

idade = ano_atual - ano_nascimento

if idade >= 16:
    print("Você pode votar este ano!")
else:
    print("Você não pode votar este ano.")
    altura = float(input("Digite a altura em metros: "))
sexo = int(input("Digite o sexo (1 para feminino, 2 para masculino): "))

if sexo == 1:
    peso_ideal = (62.1 * altura) - 44.7
    print("O peso ideal para uma mulher de altura", altura, "é", peso_ideal, "kg")
elif sexo == 2:
    peso_ideal = (72.7 * altura) - 58
    print("O peso ideal para um homem de altura", altura, "é", peso_ideal, "kg")
else:
    print("Opção inválida. Digite 1 para feminino e 2 para masculino.")
    <!DOCTYPE html>
<html>
<head>
    <title>Micro Calculadora</title>
    <style>
        .calculator {
            width: 200px;
            padding: 10px;
            border: 1px solid #ccc;
        }
        .calculator input[type="button"] {
            width: 48%;
            padding: 5px;
            margin: 2px;
        }
    </style>
</head>
<body>
    <div class="calculator">
        <input type="text" id="result" readonly>
        <input type="button" value="1" onclick="addToResult(1)">
        <input type="button" value="2" onclick="addToResult(2)">
        <input type="button" value="3" onclick="addToResult(3)">
        <input type="button" value="+" onclick="addToResult('+')">
        <input type="button" value="4" onclick="addToResult(4)">
        <input type="button" value="5" onclick="addToResult(5)">
        <input type="button" value="6" onclick="addToResult(6)">
        <input type="button" value="-" onclick="addToResult('-')">
        <input type="button" value="7" onclick="addToResult(7)">
        <input type="button" value="8" onclick="addToResult(8)">
        <input type="button" value="9" onclick="addToResult(9)">
        <input type="button" value="*" onclick="addToResult('*')">
        <input type="button" value="0" onclick="addToResult(0)">
        <input type="button" value="=" onclick="calculate()">
        <input type="button" value="/" onclick="addToResult('/')">
        <input type="button" value="C" onclick="clearResult()">
    </div>

    <script>
        function addToResult(value) {
            document.getElementById("result").value += value;
        }

        function calculate() {
            var result = eval(document.getElementById("result").value);
            document.getElementById("result").value = result;
        }

        function clearResult() {
            document.getElementById("result").value = "";
        }
    </script>
</body>
</html>

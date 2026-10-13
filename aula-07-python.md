# COPIE E COLE A PLANILHA EM FORMATO DE CÓDIGO AQUI DO GITHUB E COLE NO FORMATO TEXTO NO GOOGLE COLAB, POIS SE VOCÊ TRADUZIR A PÁGINA PARA O PORTUGUÊS, ELE VAI TROCAR O PONTO PELA VÍRGULA E TODOS DARÃO O MESMO ERRO, VEJA SE O BLOCO ESTÁ NO FORMATO DE TEXTO NO GOOGLE COLAB.

# 📌 1: O "DIVISOR DE CONTA" SIMPLES (Sem garçom)

| ID | Cenário / Objetivo | Prompt / Entrada do Usuário | Resultado que o Aluno Deve Preencher |
| :--- | :--- | :--- | :--- |
| **01** | Teste Padrão (Divisão Exata) | **Valor total:** 100.00<br>**Quantidade de pessoas:** 4 | Cada pessoa vai pagar: R\$ XX.XX |
| **02** | Divisão com Dízima Periódica | **Valor total:** 100.00<br>**Quantidade de pessoas:** 3 | Cada pessoa vai pagar: R\$ XX.XX |
| **03** | Conta de Alto Valor | **Valor total:** 1545.80<br>**Quantidade de pessoas:** 5 | Cada pessoa vai pagar: R\$ XX.XX |
| **04** | Apenas Uma Pessoa | **Valor total:** 50.50<br>**Quantidade de pessoas:** 1 | Cada pessoa vai pagar: R\$ XX.XX |
| **05** | Valor Total Inteiro | **Valor total:** 80<br>**Quantidade de pessoas:** 2 | Cada pessoa vai pagar: R\$ XX.XX |
| **06** | Teste Crítico (Divisão por Zero) | **Valor total:** 50.00<br>**Quantidade de pessoas:** 0 | Ocorreu o erro: [_______________________] |
| **07** | Teste Crítico (Texto no Valor) | **Valor total:** vinte<br>**Quantidade de pessoas:** 2 | Ocorreu o erro: [_______________________] |
| **08** | Teste Crítico (Pessoas Decimais) | **Valor total:** 100.00<br>**Quantidade de pessoas:** 2.5 | Ocorreu o erro: [_______________________] |
| **09** | Centavos Quebrados | **Valor total:** 10.05<br>**Quantidade de pessoas:** 2 | Cada pessoa vai pagar: R\$ XX.XX |
| **10** | Teste Crítico (Padrão BR com Vírgula) | **Valor total:** 50,25<br>**Quantidade de pessoas:** 2 | Ocorreu o erro: [_______________________] |
```python
valor_total = float(input("Dígito do valor total da conta: R$ "))
# float - Armazena e processa números reais com casas decimais
# input() - Recebe dados digitados pelo usuário através do teclado
# variável - Armazena temporariamente dados na memória do computador para reutilização

total_pessoas = int(input("Digite a quantidade de pessoas: "))
# int - Utilização de números inteiros positivos e negativos não decimais

valor_por_pessoa = valor_total / total_pessoas

print(f"Cada pessoa vai pagar: R$ {valor_por_pessoa:.2f}")
#imprimir(); - Exibe textos, variáveis ​​e resultados na tela do computador
# f-string - Interpola e encaixar variáveis ​​diretamente dentro de um texto de forma simples
# formatação .2f. - Limita a exibição de um número decimal para apenas duas casas após a vírgula
# divisão /; - Dividir dois valores gerando sempre um resultado decimal (float)
```
# 📌 2: CONVERSOR DE MOEDAS - Dólar para Real

| ID | 1º Prompt | 2º Prompt | Resultado que o Aluno Deve Preencher |
| :--- | :--- | :--- | :--- |
| **01**  | Quantidade de dólares: 75.50 | Cotação do dólar: 5.45 | Resultado: __________________________________ | 
| **02**  | Quantidade de dólares: 154.80 | Cotação do dólar: 5.50 |  Resultado: __________________________________ | 
| **03**  | Quantidade de dólares: 1.50 | Cotação do dólar: 5.6025 | Resultado: __________________________________ |
| **04**  | Quantidade de dólares: 0.50 | Cotação do dólar: 5.50254 | Resultado: __________________________________ | 
| **05**  | Quantidade de dólares: 1000.00 | Cotação do dólar: 5.5089 | Resultado: __________________________________ |
| **06**  | Quantidade de dólares: 75.50 | Cotação do dólar: 5.45 | Resultado: __________________________________ | 
| **07**  | Quantidade de dólares: 154.80 | Cotação do dólar: 5.5062 | Resultado: __________________________________ | 
| **08**  | Quantidade de dólares: 1.50 | Cotação do dólar: 5,60 | Resultado: __________________________________ | 
| **09**  | Quantidade de dólares: 0.50 | Cotação do dólar: 5.5095 | Resultado: __________________________________ | 
| **10**  | Quantidade de dólares: 1000.00 | Cotação do dólar: 5,50 | Resultado: __________________________________ | 
```python
dolares = float(input("Quantos dólares você quer converter? US$ "))
# float - Armazena e processa números reais com casas decimais
# input() - Recebe dados digitados pelo usuário através do teclado
# variável - Armazena temporariamente dados na memória do computador para reutilização

cotacao = float(input("Qual é a cotação do dólar? R$ "))
reais = dolares * cotacao
# operador * - Multiplica dois valores para calcular o produto entre eles

print(f"Você terá o equivalente a: R$ {reais:.2f}")
# print() - Exibe textos, variáveis e resultados na tela do computador
# f-string - Interpola e encaixa variáveis diretamente dentro de um texto de forma simples
# formatação .2f - Limita a exibição de um número decimal para apenas duas casas após a vírgula
```

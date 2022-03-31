# app-de-vendas-desconto-unidade
# Código python para um app de vendas com aplicação de desconto progressimo por unidades adquiridas

print('Bem vindo à loja')
valorProduto = float(input('Entre com o valor do produto: ')) #  produto pode ser trocado pelo nome(s) do item(s)
quantidadeProduto = int(input('Entre com a quantidade: '))
subtotal = valorProduto * quantidadeProduto
#  descontos escalonados de acordo com a quantidade de unidades do produto
if quantidadeProduto <= 9:
    valorFinal = subtotal
elif 10 <= quantidadeProduto <= 99:
    valorFinal = subtotal- subtotal * 0.05
elif 100 <= quantidadeProduto <= 999:
    valorFinal = subtotal - subtotal * 0.10
else: #  aqui é o desconto é não é mais progressivo qualquer compra de 1001 ou mais unidades terão 15% de desconto
    valorFinal = subtotal - subtotal * 0.15

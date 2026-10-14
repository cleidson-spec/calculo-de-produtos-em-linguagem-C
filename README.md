algoritmo "Preços_de_cesta_basica"

var
  Nome_do_produto: caractere
  Preco_no_mes_anterior: real
  Preco_no_mes_atual: real
  variacao: real

inicio
  escreva("Digite o nome do produto: ")
  leia(Nome_do_produto)
  escreva("Digite o preço no mês anterior: ")
  leia(Preco_no_mes_anterior)
  escreva("Digite o preço no mês atual: ")
  leia(Preco_no_mes_atual)

  variacao <- ((Preco_no_mes_atual - Preco_no_mes_anterior) / Preco_no_mes_anterior) * 100

  se variacao > 0 entao
    escreval("Situação: AUMENTO")
  senao
    se variacao < 0 entao
      escreval("Situação: BAIXA")
    senao
      escreval("Situação: ESTÁVEL")
    fimse
  fimse

      escreval("Produto: ", Nome_do_produto)
      escreval("Preço anterior: ", Preco_no_mes_anterior)
      escreval("Preço atual: ", Preco_no_mes_atual)
      escreval("Variação: ", variacao, "%")

    fimalgoritmo

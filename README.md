# ProjetoBD
## **Grupo:** 
* Henrique Neves Costa 
* Elisa Nascimento Mesquita
* Ricardo Vitor Pereira Martins
* Aline Pereira Brandão

## **Descrição do cenário**
 Gabi, dona de uma loja de doces gourmet, contratou uma empresa para desenvolver um banco de dados que se relacionaria com as vendas das faliais, quadro de funcionários e o controle do estoque. <br>
 Sabe-se que cada uma das faliais possui um corpo de funcionários especializados, sendo eles: confeiteiro e vendedor. <br>
 Cada filial emite semestralmente relatórios com diversas informaçoes sobre o índice de vendas de cada doce, do qual indica qual produto deve ser substituído. As filiais possuem estoques abastecidos por fornecedores diversos, diariamente, para manter a qualidade do produto os ingredientes precisam estar sempre em dia e com uma boa quantidade em estoque por isso deve sempre saber quando reabastecê-lo, garantido sempre o bom funcionamento.

## **Entidades**
* Vendas
* Funcionários: Confeiteiro e vendedor *(herança)*
* Estoque
* Produtos
* Relatórios
* Fornecedores
* Cliente
* Filial

## **Quadro de relações**

|              | Filial | Cliente | Fornecedor | Relatório | Produto | Estoque | Funcionário | Confeitero | Vendedor | Venda |
| :----------: | :----: | :-----: | :--------: | :-------: | :-----: | :-----: | :---------: | :--------: | :------: | :---: |
| Filial       | -      |         |            |    x      |     x   |   x     |    x        |     x      |    x     |       |
| Cliente      | -      | -       |            |           |         |         |             |            |          |  x    |
| Fornecedor   | -      | -       | -          |           |         |    x    |             |            |          |       |
| Relatório    | -      | -       | -          | -         |         |         |             |            |          | x     |
| Produto      | -      | -       | -          | -         | -       |    x    |             |      x     |    x     |       |
| Estoque      | -      | -       | -          | -         | -       | -       |             |            |          |       |
| Funcionário  | -      | -       | -          | -         | -       | -       | -           |        x   |   x      |       |
| Confeitero   | -      | -       | -          | -         | -       | -       | -           | -          |          |       |
| Vendedor     | -      | -       | -          | -         | -       | -       | -           | -          | -        |  x    |
| Venda        | -      | -       | -          | -         | -       | -       | -           | -          | -        | -     |

## **Modelo Conceitual**

![3 0](https://user-images.githubusercontent.com/62437015/78948324-41779980-7a9e-11ea-9bd4-f9c08c54f99b.JPG)



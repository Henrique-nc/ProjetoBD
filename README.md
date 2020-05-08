# ProjetoBD
## **Grupo:** 
* Henrique Neves Costa 
* Elisa Nascimento Mesquita
* Ricardo Vitor Pereira Martins
* Aline Pereira Brandão

## **Descrição do cenário**
 Gabi, dona de uma loja de doces gourmet, contratou uma empresa para desenvolver um banco de dados para gerenciar as vendas das faliais, quadro de funcionários e o controle do estoque. <br>
 Sabe-se que cada uma das faliais possui um corpo de funcionários especializados, sendo eles: confeiteiro e vendedor. <br>
 Cada filial emite semestralmente relatórios com diversas informaçoes sobre o índice de vendas de cada doce, do qual indica qual produto deve ser substituído. <br>
 As filiais possuem estoques abastecidos por diversos fornecedores diariamente. Para manter a qualidade do produto os ingredientes precisam estar em dia e com uma boa quantidade em estoque, por isso, deve-se sempre saber quando reabastecê-lo, garantido seu bom funcionamento.

## **Entidades**
* Vendas
* Funcionários: Confeiteiro e vendedor *(herança)* substituir?
* Insumo
* Produtos
* Relatórios
* Fornecedores
* Cliente
* Filial

## **Atributos**

| Confeiteiro | Vendedor    | Insumo     | Cliente    | Fornecedores| Produtos       | Relatórios   | Filial      | Vendas         |
| :---------: | :---------: | :--------: | :--------: | :---------: | :------------: | :----------: | :---------: | :------------: |
| Nome *      | Nome *      | Validade * | Nome *     | CNPJ #      | Nome *         | ID #         | CNPJ *      | Nota Fiscal #  |
| CPF #       | CPF #       | Entrega *  | CPF #      | Empresa *   | Validade *     | Semestre #   | Endereço #  | Data *         |
| Telefone *  | Telefone *  | Item *     | Telefone * | Marca *     | Ingredientes o | Resultado *  | Gerente *   | Valor total *  |
| Email o     | Email o     | Marca *    | Email o    | Data *      | ID #           |              | Email o     |                |
| Endereço *  | Endereço *  | ID #       |            |             |                |              | Telefone *  |


## **Quadro de relações**

|              | Filial | Cliente | Fornecedor | Relatório | Produto | Insumo  | Funcionário | Confeitero | Vendedor | Venda |
| :----------: | :----: | :-----: | :--------: | :-------: | :-----: | :-----: | :---------: | :--------: | :------: | :---: |
| Filial       | -      |         |            |    x      |     x   |   x     |    x        |     x      |    x     |       |
| Cliente      | -      | -       |            |           |         |         |             |            |          |  x    |
| Fornecedor   | -      | -       | -          |           |         |    x    |             |            |          |       |
| Relatório    | -      | -       | -          | -         |         |         |             |            |          | x     |
| Produto      | -      | -       | -          | -         | -       |    x    |             |      x     |    x     |       |
| Insumo       | -      | -       | -          | -         | -       | -       |             |            |          |       |
| Funcionário  | -      | -       | -          | -         | -       | -       | -           |        x   |   x      |       |
| Confeitero   | -      | -       | -          | -         | -       | -       | -           | -          |          |       |
| Vendedor     | -      | -       | -          | -         | -       | -       | -           | -          | -        |  x    |
| Venda        | -      | -       | -          | -         | -       | -       | -           | -          | -        | -     |

## **Modelo Conceitual**

![Capturar](https://user-images.githubusercontent.com/62437015/79284732-ed035e00-7e91-11ea-8487-f3b62ff6cee6.PNG)

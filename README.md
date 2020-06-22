# ProjetoBD
## **Grupo:** 
* Henrique Neves Costa 
* Elisa Nascimento Mesquita
* Ricardo Vitor Pereira Martins
* Aline Pereira Brandão

## **Descrição do cenário**
<p>Gabi, dona de uma loja de doces gourmet, contratou uma empresa para desenvolver um banco de dados para gerenciar as vendas das filiais, quadro de funcionários e o controle do estoque. <br>
 Cada filial emite semestralmente relatórios com diversas informações sobre o índice de vendas de cada doce, do qual indica qual produto deve ser substituído (o mesmo produto é substituído em todas). <br>
 As filiais possuem estoques abastecidos por diversos fornecedores diariamente. Para manter a qualidade do produto os ingredientes precisam estar em dia e com uma boa quantidade em estoque, por isso, deve-se sempre saber quando reabastecê-lo, garantido seu bom funcionamento.

## **Entidades**
* Venda
* Funcionário: Confeiteiro, gerente e vendedor *(herança)*
* Insumo
* Produto
* Relatório
* Fornecedor
* Cliente
* Filial

## **Atributos**

| Confeiteiro | Vendedor    | Insumo     | Cliente    | Fornecedor  | Produto        | Relatório       | Filial      | Venda          |
| :---------: | :---------: | :--------: | :--------: | :---------: | :------------: | :-------------: | :---------: | :------------: |
| Nome *      | Nome *      | Validade * | Nome *     | CNPJ #      | Nome *         | UID #           | CNPJ *      | Nota Fiscal #  |
| CPF #       | CPF #       | Entrega *  | CPF #      | Empresa *   | Validade *     | Semestre *      | CEP *       | Data *         |
| Telefone *  | Telefone *  | Item *     | Telefone * | Marca *     | Ingredientes o | Indice venda *  | Gerente *   | Valor total *  |
| Email o     | Email o     | Marca *    | Email o    | Data *      | UID #          | Resultado    *  | Email o     |                |
| Endereço *  | Endereço *  | UID #      |            |             |                |                 | Telefone *  |
|             |             |            |            |             |                |                 | UID #       |

Obs.: Resultado = Produto a ser substituído.

## **Modelo Conceitual**

![2034385b-d98d-4384-ac92-fbe7bbb05c60](https://user-images.githubusercontent.com/62437015/85328915-f4ee0880-b4a7-11ea-9d75-d8d8f0784758.jpg)

## **Modelo Lógico**

![WhatsApp Image 2020-06-09 at 20.40.04.jpg]


## **Banco de dados no site da Oracle Live SQL**


[Gabriel Ziegler]: https://github.com/gabrielziegler3
[Cleber Júnior]: https://github.com/cjjcastro
[Lucas Hiroshi]: https://github.com/hiroshi
[Vinicius Ferreira]: https://github.com/ViniciusBernardo
[Pablo Silva]: https://github.com/pablodiegoss

### Histórico de Revisões

| Data       | Versão | Descrição            |         Autor             |
|:----------:|:------:|:--------------------:|:-------------------------:|
| 10/10/2018 | 0.1 | Criação do Documento | [Lucas Hiroshi] |
| 12/10/2018 | 0.1 | Criação do Documento | [Vinicius Ferreira], [Pablo Silva] |

# Vinicius F. & Pablo D.
## Tabela de Inspeção

| ID| Defeito  | Criticidade | Proposta de reparo | Prazo sugerido p/ reparos | Observações |
|:-:|:--------:|:-----------:|:------------------:|:-------------------------:|:-----------:| 
| 1 |    Sim   |      1      |Mudar atributos e nomes de entidades para o padrão Oracle de nomenclatura definido no projeto|0.5 h|| 
| 2 |Não existe|             |                    |                           |             | 
| 3 |Não existe|             |                    |                           |             | 
| 4 |Não existe|             |                    |                           |             | 
| 5 |Não existe|             |                    |                           |             | 
| 6 |    Sim   |      2      |Decompor a entidade VENDA para adequa-lá a 2° FN já que essa entidade possui informações referentes ao cliente da venda|1.5 h|Cliente deveria ser uma entidade a parte já que os requisitos pedem para armazenar o nome do cliente seu cpf e id| 
| 7 |Não existe|             |                    |                           |             | 
| 8 |    Sim   |      2      |Deve-se decompor a entidade VENDA criando uma nova entidade, no caso, CLIENTE, e relaciona-lá a VENDA.|1.5 h|O atributo "não-chave" "nome_cliente" na entidade Venda não é dependente da chave primária da entidade VENDA.| 
| 9 |Não existe|             |                    |                           |             | 
| 10|    Sim   |      2      | Remova o atributo "preço_total" da entidade venda a partir do Diagrama Lógico e implemente uma regra de negócio que calcule o valor total de uma venda a partir dos preços unitários de cada produto relacionado a essa venda|3 h|O atributo "preco_total" é derivado no relacionamento da VENDA com PRODUTO. Como PRODUTO possui o atributo "preço_unitario", não é necessário armazenar o somatório desses valores.| 
| 11|Não existe|             |                    |                           |             | 
| 12|Não existe|             |                    |                           |             | 
| 13|Não existe|             |                    |                           |             | 
| 14|Não existe|             |                    |                           |             | 
| 15|Não existe|             |                    |                           |             | 
| 16|   Sim    |      1      | Referencie essas implementações no texto em linguagem natural do requisito|1 h|Os relacionamentos das entidades e as cardinalidades não possuem referência para o requisito.| 
| 17|   Sim    |      2      |Crie novos modelos com diferentes perspectivas para escolher a melhor opção de modelo|4 h|| 
| 18|   Sim    |      1      | Mude o nome do relacionamento e indique a direção|0.5 h|O relacionamento entre produto e venda não possui uma direção definida e seu nome não esclare o papel do produto sobre a venda e vice-versa.| 
| 19|Não existe|             |                    |                           |             | 
| 20|Não existe|             |                    |                           |             | 
| 21|   Sim    |      2      | Defina uma PK para a entidade RECEITA|1 h|A entidade Receita não possui uma Primary Key definida.| 
| 22|Não existe|             |                    |                           |             | 
| 23|   Sim    |      3      |A cardinalidade entre as entidades MEDICAMENTO e RECEITA no DE-R está definida como 1:1, já no Diagrama Lógico, como 1:n. Verifique os requisitos e o domínio da aplicação para decidir qual cardinalidade usar e faça as devidas alterações onde estiver presente a inconsistência.|2.5 h|| 

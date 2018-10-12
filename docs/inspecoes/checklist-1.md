[Cleber Júnior]: https://github.com/cjjcastro
[Igor Araujo]: https://github.com/zero101010

### Histórico de Revisões

| Data       | Versão | Descrição            |         Autor             |
|:----------:|:------:|:--------------------:|:-------------------------:|
| 12/10/2018 | 0.1 | Criação do Documento | [Cleber Júnior] e [Igor Araujo] |
| 12/10/2018 | 0.2 | Inserindo as inpeções | [Cleber Júnior] e [Igor Araujo] |

# Cléber & Igor
## Inspeções

| ID| Defeito | Não se aplica | Criticidade | Proposta de reparo | Prazo sugerido p/ reparos | Observações |
|:-:|:-------:|:-------------:|:-----------:|:------------------:|:-------------------------:|:-----------:|
| 1 |         | x             |             |                    |                           |             |
| 2 | A tabela comercializa não está no dicionário de dados. |               | 2           | Acrescentar a tabela comercializa ao dicionário de dados| 3 horas ||
| 3 |         | x             |             |                    |                           |O arquivo não possui nenhum comentário de tabela ou coluna.|
| 4 |         | x             |             |                    |                           |O arquivo não possui comentários de tabela|
| 5 |         | x             |             |                    |                           |O arquivo não possui comentários de tabela |
| 6 |Não está na terceira forma normal, pois a segunda e, logicamente, a terceira não foram satisfeitas.|| 3 | Solucionar os itens [8] e [9] da inspeção. | 15 horas | |
| 7 |         | X             |             |                    |                           |Todos os atributos são baseados em domínios simples, não contendo grupos ou valores repetidos.|
| 8 | A tabela RECEITA possui um atributo crm_medico que não depende da chave primária id_medicamento.| | 3 | Criar uma tabela para o médico e inserir uma chave estrangeira na tabela RECEITA. | 72 horas || 
| 9 | Na tabela VENDA o atributo preco_total pode ser obtido pela soma de todos os atributos preco_unitario da tabela PRODUTO, assim, esse atributo é dependente de outro atributo.        |               | 3 | Remover o atributo preco_total e utilizar o preco_unitario para conseguir esse dado. | 12 horas | |
| 10| O atributo preco_total da tabela VENDA é desnecessário, pois pode ser obtido utilizando outros atributos. || 3 | Remover o atributo preco_total para obter o dado pelo preco_unitario. | 12 horas |  |
| 11|         |               |             |                    |                           | |
| 12|         |x              |             |                    |                           | |
| 13|         |x              |             |                    |                           | |
| 14|         |x              |             |                    |                           | |
| 15|         |x              |             |                    |                           | |
| 16|         |x              |             |                    |                           | |
| 17|         |x              |             |                    |                           | |
| 18| Não fica clara a relação entre  MEDICAMENTO e  RECEITA, pois "necessita" não necessáriamente é a relação mais clara. Uma medição não necessita de uma receita, mas sim, para comprar uma medicação, em alguns casos, é necessário uma receita. || 3 | Repensar a relação da receita com as outras entidades | 120 horas | |
| 19|         |x             |             |                    |                           | Apesar de alguns erros na implementação a modelagem é clara e objetiva. |
| 20|         |x              |             |                    |                           | A modelagem está clara e de fácil entendimento. |
| 21| A tabela RECEITA não possui chave primária.|| 1 | Inserir uma chave primária para a tabela RECEITA. | 1 hora | |
| 22| Deixar a chave primária por último na tabela não é o padrão utilizado no projeto. ||1|Alterar a posição das chave primária em todas as tabelas| 1 hora||
| 23| A relação entre MEDICAMENTO e RECEITA está diferente do diagrama DER para o diagrama lógico ||1|Alterar a cardinalidade para o valor correto.| 1,5 horas| |
 

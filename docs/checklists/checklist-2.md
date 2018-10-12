[Gabriel Ziegler]: https://github.com/gabrielziegler3
[Gabriel Alves]: https://github.com/gitgabiru
[Lucas Hiroshi]: https://github.com/hiroshi

# Histórico de Revisões

| Data       | Versão | Descrição            |         Autor             |
|:----------:|:------:|:--------------------:|:-------------------------:|
| 10/10/2018 | 0.1 | Criação do Documento | [Lucas Hiroshi] |
| 12/10/2018 | 0.2 | Inspeção do Modelo de Dados | [Gabriel Ziegler], [Gabriel Alves] |

### Gabriel Z. & Gabriel A.
## Tabela de Inspeção

| ID| Defeito | Criticidade | Proposta de reparo | Prazo sugerido p/ reparos | Observações |
|:-:|:-------:|:-----------:|:------------------:|:-------------------------:|:-----------:| 
| 1 | Sim     | 1           | Checar documentação do guia de estilo e ajustar conforme os padrões Oracle | 0.5h | Atentar para padrões em nomes de atributos | 
| 2 | Não     | - | - | - | - | 
| 3 | Não     | - | - | - | - | 
| 4 | Não     | - | - | - | - | 
| 5 | Não     | - | - | - | - | 
| 6 | Sim     | 3           | Retirar atributos derivados do modelo lógico | 1h | Atentar para o não uso de PKs em tabelas especializadas | 
| 7 | Não     | - | - | - | - | 
| 8 | Sim     | 3           | Adicionar chaves primárias à entidades que não possuem | 1h | Entidades RECEITA e PERFUMARIA | 
| 9 | Sim | 3 | Adicionar chaves primárias à entidades que não possuem | 1h | Entidades RECEITA e PERFUMARIA | 
| 10| Sim | 3 | Entidades sem chave primária possibilitam a inserção de dados duplicados | 1h | - | 
| 11| Sim     | - | É possível remover ajustando o item 10 | 1.5h | - | 
| 12| Não     | - | - | - | - | 
| 13| Não     | - | - | - | - | 
| 14| Sim     | 3           | As informações do cliente não estão sendo salvas no banco | 2h | Entidade CLIENTE não é tratada na solução apresentada. | 
| 15| Não se aplica | - | - | - | - | 
| 16| Sim     | 2           | Referenciar o porquê de cada cardinalidade assumida | 1h | Ex: Um fabricante produz um medicamento, onde foi encontrada essa regra de negócio? | 
| 17| Não     | - | - | - | - | 
| 18| Não     | - | - | - | - | 
| 19| Não     | - | - | - | - | 
| 20| Não     | - | - | - | - | 
| 21| Sim     | 3           | Mesmo problema descrito no item 8 | 1h         | - | 
| 22| Sim     | 1           | As PKs estão definidas sempre na primeira linha da tabela | 0.5h | - | 
| 23| Sim     | 3           | Receita ~ Medicamento possui cardinalidades distintas no nível lógico e DE-R | 0.5h | Checar cardinalidades em todos os níveis | 

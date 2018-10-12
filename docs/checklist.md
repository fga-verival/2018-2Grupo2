[Gabriel Ziegler]: https://github.com/gabrielziegler3
[Cleber Júnior]: https://github.com/cjjcastro

### Histórico de Revisões

| Data       | Versão | Descrição            |         Autor             |
|:----------:|:------:|:--------------------:|:-------------------------:|
| 10/10/2018 | 0.1 | Criação do Documento | [Gabriel Ziegler] |
| 11/10/2018 | 0.2 | Inserindo a primeira versão do checklist | [Cleber Júnior] |
| 11/10/2018 | 0.3 | Inserindo a tabela de inspeção e atualizando a tabela de checklist | [Cleber Júnior] |

## Checklist

| ID| Descrição do defeito | 
|:-:|:---------------------|
| 1 | **Os objetos do banco de dados seguem o padrão de nomenclatura definido?** |
| 2 | **O Dicionário de Dados foi criado ou atualizado?** |
| 3 | O Dicionário de Dados foi armazenado por meio de comentários de tabelas e colunas?|
| 4 | Todos os comentários explicam a função e necessidade de cada tabela? |
| 5 | Os comentários nos campos informam sua utilidade? |
| 6 | **A base de dados está na 3ª Forma Normal?** |
| 7 | Foi verificada a não existência de atributos multivalorados em todas as tabelas? Ou seja, todos os atributos devem ser baseados em domínios simples, não contendo grupos ou valores repetidos. |
| 8 | Cada atributo "não-chave" é dependente da chave primária inteira? |
| 9 | Foi verificada a não existência de dependência transitiva em todas as tabelas? Ou seja, atributo "não-chave" não deve possuir dependência para cada chave candidata na tabela. |
| 10 | **Foi verificada a existência de dados redundantes na base de dados?** |
| 11 | A base possui dados redundantes? É possível removê-los? |
| 12 | Caso haja a necessidade de uso de dados redundantes, existe algum mecanismo de controle dessa redundância? Esses mecanismos estão documentados na base de dados e no dicionário de dados? |
| 13 | Verificou-se o requisito que originou a necessidade de redundância e se realmente é a melhor solução? |
| 14 | **Foi verificada a existência de regras de negócio implementadas diretamente na base de dados e se as mesmas foram documentadas?** |
| 15 | Havendo regras de negócio implementadas diretamente na base de dados (via triggers, procedures, packages, etc), estas foram documentas no código-fonte correspondente? |
| 16 | Existe a referência para o requisito que gerou cada regra de negócio? |
| 17 | Foi analisada se esta forma de implementação é a melhor opção? |
| 18 | **O Modelo de Dados está claro e objetivo?** |
| 19 | Você, que não elaborou este modelo, consegue entender o que se pretende modelar ou o que foi implementado? |
| 20 | Você acredita que alguém, que não esteja familiarizado com o projeto, consegue entender o Modelo de Dados? |
| 21 | Os nomes dos objetos são intuitivos e seguem o padrão abaixo. Sendo que, o ORACLE só permite objetos com nomenclatura de até 30 caracteres.<br>Nome do check: CKC + Nome do Campo + Nome da tabela (Caso ultrapasse 30 caracteres, abrevie o nome da tabela e se o check for único no banco pode ser CKC + Nome do Campo).<br>Nome da PK: PK_+ Nome da tabela<br>Nome da FK:  FK+ Abreviação do módulo + próximo código da FK do módulo (5 dígitos, complementados com zeros a esquerda quando o número for menor) + nome da tabela referenciada<br>Nome dos índices: Todos os índices referentes a FKs sejam criados com a mesma nomenclatura da constraint, além disso, os índices que não forem referentes a FK’s deverão ser criados da seguinte forma: <br>NOMEDATABELA_XX, onde XX representa a quantidade de índices que já existem na tabela + 1 |
| 22 | Toda tabela deve ter PK. Sendo que, as novas tabelas devem conter apenas uma chave na PK. |
| 23 | Ao criar uma tabela, deixe sempre a PK por último. |
| 24 | A cardinalidade está definida de forma correta nos diagramas |



## Tabela de Inspeção

| ID| Defeito | Não se aplica | Criticidade | Proposta de reparo | Prazo sugerido p/ reparos |
|:-:|:-------:|:-------------:|:-----------:|-------------------:|:-------------------------:|

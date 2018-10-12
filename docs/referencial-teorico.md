[Gabriel Ziegler]: https://github.com/gabrielziegler3
[Lucas Hiroshi]: https://github.com/hiroshi18

### Histórico de Revisões

| Data       | Versão | Descrição            |         Autor             |
|:----------:|:------:|:--------------------:|:-------------------------:|
| 10/10/2018 | 0.1 | Criação do Documento | [Gabriel Ziegler] |
| 11/10/2018 | 0.2 | Adicionando Inspeções |  [Lucas Hiroshi] |
| 11/10/2018 | 0.3 | Adicionando Fagan |  [Lucas Hiroshi] |

# Referencial Teórico

## Inspeções

### Definição

Uma inspeção e umas das varias técnicas de revisões na garantia da qualidade elas são destacadas pelo modelo CMMI, que exige a realização de revisões como uma prática específica do processo de verificação. Sabe-se ainda que inspeções de software, em particular, capturam em torno de 60\% dos defeitos de artefatos (BOEHM e BASILI, 2001) o que deixa explícita a sua contribuição para a melhoria da qualidade.

* O processo de inspeção deve ter um orçamento definido, ser planejada e com um cronograma bem definido.

* Um processo deve ser adotado no inicio e mantido até o final.

* Os membros da equipe devem possuir conhecimento adequado para participar no processo de inspeção.

* Treinamentos devem ser providenciados caso necessário para os diferentes papeis no processo de inspeção.

* Para se ter uma avaliação da revisão um checklist é necessário, no qual o processo de inspeção deve seguir.


## Fagan

### Definição

A Inspeção de Fagan é um método para encontrar defeitos. Ela é estruturada em um processo que envolver detectar defeitos no desenvolvimento de produtos como código de programação, especificações, designs e etc.

O termo Fagan é nomeado pelo seu autor Michael Fagan que associou vários métodos formais de inspeção de software. Nesse método de inspeção uma atividade possui um critério de entrada e saída definido então para cada atividade Fagan possui um modo de validar se a saída esta de acordo com os critérios.

#### Papéis
Para que uma Inspeção de Fagan prossiga de forma correta e possua bons resultados é necessário que os seguinte papéis sejam preenchidos.

* Moderador: É a pessoa responsável pelo monitoramento do processo de inspeção. Ou seja é responsável por organizar as reuniões, relatórios, resultados, controle reuniões. Conduzir uma inspeção requer um moderador para garantir que não haja conflito entre as partes envolvidas e designar papéis de acordo com as habilidades.

* Autor: Responsável por manter o produto a que está sendo inspecionado. O autor pode responder as questões levantadas durante o processo de inspeção.

* Leitor: A responsabilidade do leitor é simplesmente descrever o que está escrito e auxiliar os membros da equipe no entendimento.

* Registrador: Responsável por anotar os defeitos sendo levantados durante o processo de inspeção.

* Inspetor: Função normalmente realizada por quase todo o time independente do papel que tenha sido designado a ele, com o objetivo de procurar por erros. Essa é uma atividade continua durante quase todo o processo de desenvolvimento do produto. 

* Planejamento
Ela começa pela preparação dos materiais, definição de equipe e preparação de um local de reunião. 

* Preparação individual
Os participantes da revisão revisam o item a ser inspecionado e os materiais de apoio necessários e se preparam para a reunião anotando as questões e possíveis defeitos.

* Reunião de Inspeção
Na qual os defeitos são expostos

* Retrabalho
Durante essa fase os defeitos encontrados durante a reunião são resolvidos pelo autor. Basicamente os defeitos são arrumados ate que as critérios de aceitação sejam atendidos.

* Continuação 
Nesta fase todos os defeitos encontrados devem ter sido arrumados. O moderador é responsável por verificar se todos os defeitos foram arrumados e que nenhum defeito novo foi inserido durante o processo de arrumar o item.

# Como o agendamento manual e automático afeta o cronograma?

É fundamental saber as diferenças entre tarefa agendada manualmente e tarefa agendada automaticamente para entender como o Project agenda o projeto.

Em geral, as tarefas agendadas manualmente deixam você controlar o cronograma. Quando você adiciona uma tarefa ao cronograma, ela fica no lugar. No entanto, nem sempre essa é a melhor maneira de criar um cronograma, especialmente conforme os projetos se tornam mais complicados e você quer usar tarefas agendadas automaticamente para tirar proveito do sofisticado mecanismo de agendamento do Project.

Dê uma olhada na imagem a seguir. Ela mostra os dois tipos diferentes de tarefas; as duas primeiras agendadas manualmente e as duas últimas, automaticamente.

Tarefas agendadas manualmente e automaticamente explicadas.jpg

Observe que para as tarefas agendadas manualmente, a duração é um valor de texto, além de um número. Como a duração pode ser um valor de texto, uma data de início não foi definida automaticamente pelo Project, e a barra de Gantt é exibida apenas parcialmente para refletir a incerteza do cronograma da tarefa neste momento.

Para a tarefa agendada automaticamente, a duração é um valor numérico com uma unidade de tempo acrescentada, como “12h” para uma duração de doze horas. Por definição, durações, datas de início e datas de término válidas de tarefas agendadas automaticamente e, portanto, as barras, são desenhadas automaticamente pelo Project.

Mas às vezes fica um pouco mais complicado com as informações que você fornece para tarefas agendadas manualmente. Para desenhar barras em uma tarefa agendada manualmente, o Project precisa apenas de três valores de tempo: duração, data de início e data de término. Se você definir dois desses valores para uma tarefa agendada manualmente, o terceiro valor será calculado automaticamente pelo Project e a tarefa permanecerá com o agendamento manual. Então, atenção com esse tipo de comportamento “inesperado” do Project.

> **Observação:** Por padrão, as tarefas são agendadas manualmente. Os gerentes de projeto acostumados com o agendamento automático das versões anteriores do Project podem desativar o recurso de agendamento manual de determinadas tarefas ou do projeto inteiro. Alguns projetos, especialmente os mais complicados, podem exigir que o sofisticado mecanismo de agendamento do Project cuide do agendamento. Para alterar todas as tarefas para o agendamento automático, clique em **Novas Tarefas: Agendar Automaticamente** na parte inferior da janela do aplicativo Project.

**Tarefas agendadas manualmente**
Você pode colocar uma tarefa agendada manualmente em qualquer local do cronograma e o Project não vai movê-la. Esse novo recurso oferece mais flexibilidade e controle sobre o planejamento e o gerenciamento do cronograma.

Por que você deveria se preocupar? Bem, frequentemente os cronogramas de projetos são bastante informais. Eles começam como simples listas de datas a partir de emails, reuniões com participante ou uma conversa no corredor. Muitas vezes, os gerentes de projeto não têm informações completas sobre os itens do trabalho. Por exemplo, talvez eles só saibam quando uma tarefa deve ser iniciada, mas não saibam sua duração até terem uma estimativa dos membros da equipe. Além disso, eles podem saber quanto tempo uma tarefa levará, mas não saberão que ela pode ser iniciada até receberem a aprovação do gerente de recursos.

Estes são alguns pontos que você deve lembrar em relação às tarefas agendadas manualmente.

* **Você nunca estará no escuro**. As tarefas agendadas manualmente têm seus próprios indicadores e barras de tarefas para ajudar a diferenciá-las das tarefas agendadas automaticamente "clássicas".

* **Tudo é possível.** Quando uma tarefa está no modo agendado manualmente, as colunas Início, Término e Duração podem estar em branco ou incluir valores de texto, além de datas reconhecíveis.

* **Alternando os modos de agendamento** Você pode alternar entre tarefas agendadas manualmente e automaticamente. Porém, tome cuidado. Quando você altera uma tarefa de agendada manualmente para uma agendada automaticamente, o Project precisa tomar algumas decisões. Se a duração da tarefa era "Uma quinzena", normalmente o Project define uma duração estimada de "1 dia?", caso a tarefa seja definida como agendada automaticamente. Afinal, você não pode esperar que ele saiba que uma quinzena tem duas semanas.

* **Controle o adiamento** Se uma tarefa agendada manualmente precisar ser atrasada devido a um adiamento, suas tarefas sucessoras não serão transferidas automaticamente. Os gerentes de projeto podem decidir manter as datas originais, caso seus recursos possam proceder conforme o planejado, ou atrasar as tarefas sucessoras, se houver dependências complicadas.

* **Impactos controlados pelo esforço**    As tarefas agendadas manualmente não podem ser definidas como controladas pelo esforço. A duração de uma tarefa agendada manualmente não mudará com a adição ou a remoção de recursos. Aprenda mais posteriormente neste artigo.

A tabela a seguir mostra como os atributos do Project são definidos e usados para agendar tarefas manualmente e automaticamente.

|   Item            |   Agendada manualmente            |   Agendada automaticamente        |
|-------------------|-----------------------------------|-----------------------------------|
|   **Duração**     |Podem ser informações de número, data ou texto, como "14d" ou "quinzena". Não usada pelo Project para ajudar a agendar o projeto, se o valor não estiver em um formato de duração que possa ser reconhecido.|É possível usar somente números que representam períodos e unidades de tempo, como "14d" ou "2 meses".|
|   **Trabalho**    |É possível usar somente números que representam períodos e unidades de tempo, como "14d" ou "2 meses".|É possível usar somente números que representam períodos e unidades de tempo, como "14d" ou "2 meses".|
|   **Recursos**    |Podem ser atribuídos a tarefas. Os calendários de recursos não são usados pelo Project para ajudar a agendar tarefas.|Podem ser atribuídos a tarefas. Usados pelo Project para ajudar a determinar o melhor cronograma. Mudarão a duração das tarefas, se elas forem definidas como controladas pelo empenho, diferentemente das tarefas agendadas manualmente.|
|   **Data de início**|Podem ser informações de número, data ou texto, como "30 jan" ou "Em breve". Não usada pelo Project para ajudar a agendar o projeto, se o valor não estiver em um formato de tempo que possa ser reconhecido.|É possível usar somente informações de data. No entanto, você pode usar os valores “hoje” e “amanhã”, que o Project reserva para tarefas agendadas automaticamente.|
|   **Data de término** |Podem ser informações de data ou texto, como "30 jan" ou "Em breve". Não usada pelo Project para ajudar a agendar o projeto.|É possível usar somente informações de data. No entanto, você pode usar os valores “hoje” e “amanhã”, que o Project reserva para tarefas agendadas automaticamente.|
|   **Restrições**  |Ignoradas pelo Project.|Usadas pelo Project para ajudar a determinar o melhor cronograma.|
|   **Dependências (vínculos)**|Podem ser usadas, mas não alterarão o agendamento da tarefa. Contudo, os vínculos da tarefa a reagendarão quando aplicados pela primeira vez.|Podem ser usadas e alterarão o agendamento da tarefa.|
|   **Calendários do projeto e de recursos**|Ignorados pelo Project.|Usados pelo Project para ajudar a determinar o melhor cronograma.|

**Tarefas agendadas automaticamente**
As tarefas agendadas automaticamente são a forma clássica usada pelo Project para agendar suas tarefas. O agendamento automático fornece um maio sistemático e altamente estruturado de gerenciar os cronograma do projeto. Com base na entrada dos usuários, como a duração da tarefa, o trabalho planejado, o número de recursos e as datas de restrição, o Project calcula as datas mais anterior e mais posterior para as tarefas em um cronograma ideal.

O Project agenda um projeto a partir das informações que você insere sobre:

* O projeto geral.

* Os itens de trabalho individuais (chamados de tarefas) necessários para realizar o projeto.

* Se necessário, os recursos exigidos para realizar essas tarefas.

Se algo no projeto mudar depois que você criar o cronograma, você poderá atualizar as tarefas ou os recursos, e o Project ajustará o cronograma para você.

Para cada tarefa, você pode inserir um ou todos os seguintes itens:

* Durações

* Dependências entre tarefas

* Restrições

Usando essas informações, o Project calcula a data de início e a data de término de cada tarefa.

Você pode inserir recursos no projeto e depois atribuí-los a tarefas para indicar qual recurso é responsável pela realização de cada atribuição. Além de ajudar a planejar sua equipe de projeto, isso também pode ajudar a calcular o número de máquinas necessárias ou a quantidade de material a ser consumido. Se você inserir recursos, os cronogramas de tarefas serão mais refinados de acordo com as seguintes informações dos recursos:

* Trabalho

* Unidades

* Períodos de trabalho e de folga inseridos em calendários.

Outros elementos, como tempo de avanço e tempo de retardo para vínculos, tipos de tarefa, disponibilidade de recursos e recurso de controle, podem afetar o agendamento. Assim, entender os efeitos desses elementos pode ajudar a manter e ajustar seu cronograma, conforme necessário.

> **Observação:** O Project calcula a duração de tarefas agendadas automaticamente com base nas definições das unidades de duração (clique em **Arquivo, Opções** e em **Agendar**). Da mesma forma que eu um calendário mensal normal, o ano começa em janeiro e cada semana começa no domingo ou na segunda-feira. Por padrão, quando o Project calcula as unidades de duração, um dia é igual a 8 horas, uma semana é igual a 40 horas e um mês é igual a 20 dias úteis. Se você inserir datas de início e de término para tarefas e não inserir as horas de início e de término, o Project usará 8h como hora de início padrão e 17h como hora de término padrão.

**Alterando os modos de agendamento de tarefas**
Você pode alternar o agendamento de uma tarefa de automático para manual (clique em **Arquivo, Opções** e em **Agendar**). Ao alterar os modos de tarefa, lembre-se do seguinte.

Uma tarefa que é alterada para o agendamento automático terá a duração e as datas definidas com as configurações padrão do Project. Por exemplo, o Project alterará uma tarefa agendada manualmente com uma duração de "Algumas semanas" para o padrão de "1 dia?". Uma tarefa com a data de início inserida manualmente como "amanhã" terá seu início alterado para a data de início do projeto quando ele for alterado para uma tarefa agendada automaticamente.

Uma tarefa que é alterada para agendada manualmente manterá sua duração e suas datas. No entanto, depois que a tarefa é definida para agendada manualmente, a duração e as datas podem ser qualquer valor de número, texto ou data.
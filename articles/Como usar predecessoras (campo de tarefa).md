# Predecessoras (campo de tarefa)

**Tipo de dados**     Lista de inteiros

**Tipo de Entrada**    inserida

Descrição     O campo Predecessoras lista os números de identificação da tarefa para as tarefas de predecessora quais a tarefa depende para poder começar ou terminar. Cada predecessora está vinculada à tarefa por um tipo específico de dependência entre tarefas e um tempo de avanço ou tempo de retardo.

**Uso recomendado**     Adicione o campo Predecessoras a uma visão de tarefas quando desejar exibir ou atualizar as predecessoras da tarefa. Cada tarefa predecessora é representada por seu número de identificação de tarefa, que pode ser seguido por um tipo de dependência e pelo tempo de espera ou de latência. Os tipos de dependência de predecessoras são TI (término-a-início), TT (término-a-término), II (início-a-início) e IT (início-a-término). Para inserir tempo de espera, digite um número negativo. Para inserir tempo de latência, digite um número positivo.

**Exemplo**     Você deseja revisar as predecessoras de tarefas do seu projeto para analisar e refinar o cronograma. No modo de exibição de Planilha de Tarefas, o campo Predecessoras contém a entrada "14TI+3d" para a tarefa "Escrever proposta". Isso significa que a tarefa  14 é uma predecessora dessa tarefa, com uma dependência término-a-início e um tempo de latência de três dias. Para poder começar, essa tarefa deve esperar três dias após o término da tarefa 14. O campo Predecessoras da tarefa "Conduzir reuniões com clientes" está em branco. Você digita "15TI" para vincular essa tarefa à tarefa  15 com uma dependência término-a-início.

**Comentários**     Se você inserir apenas o número de identificação da tarefa no campo Predecessoras, o Project assumirá uma dependência término-a-início com tempo de retardo igual a zero. Se houver mais do que uma predecessora, todas elas serão listadas e separadas pelo caractere separador de lista, que geralmente é a vírgula ou o ponto-e-vírgula.

Você pode usar o comando Vincular Tarefas do menu Editar para vincular as tarefas selecionadas com dependências término-a-início e tempo de retardo igual a zero. Também é possível vincular tarefas arrastando de uma tarefa para outra na parte de gráfico do Gráfico de Gantt ou do Diagrama de Rede. Você pode definir outros tipos de dependência na caixa de diálogo **Informações da Tarefa.**

Se uma predecessora for uma tarefa de um outro projeto, o campo Predecessoras contém também o caminho para o projeto vinculado, além da identificação da tarefa e do tipo de dependência. Um exemplo é: C:\Meus Documentos\Construcao.mpp\3TT.
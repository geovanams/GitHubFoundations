# Laboratório – Módulo 2: Trabalhando com repositórios GitHub

A atividade a seguir visa consolidar o conhecimento apresentado na aula, abordando os seguintes tópicos:

- Criação de repositório
- Adição de arquivos
- Adição de branch
- Clone de repositório

### Requisitos:

- Conta GitHub

## 1. Criando Repositório

1. Acesse [github.com](https://github.com) no seu navegador e faça login em sua conta (clique no botão “Sign In” localizado no canto superior direito).

2. Clique no botão sinalizado com “+”, posicionado na parte superior da tela e selecione “New Repository” ou no botão "New" do lado esquerdo.

![image](https://github.com/user-attachments/assets/dc710ede-0876-419e-8df5-797d9fd9e475)

3. Na página recém aberta, configure as seguintes informações:

Repository Owner
Repository Name
Description
Defina a visibilidade do repositório: público ou privado
Utilizando leitor de tela: O leitor indicará a presença do seguinte:

Grupo de Nome de Proprietário e de repositório, com os campos:
Repository Owner
Repository Name
Campo: Description
Grupo de Visibilidade do repositório com as seguintes opções: 
Público 
Privado

Figura 2 - Captura de tela indicando os campos a serem configurados nesse passo.


Observação:

Repare que na Figura 2 não existe a opção “Internal”, isso ocorre pois tal opção está disponível apenas nas contas Enterprise. 


4. Avançando na página temos a seção “Initialize this repository with”, nela, trabalhamos itens como os arquivos README e .gitignore e o licenciamento. Nessa etapa:

Marque a caixa de seleção “Add a README file”
Selecione a opção “None” na lista suspensa de GitIgnore
Selecione a opção MIT License na lista suspensa de licenças 
Captura de tela mostrando: 1. Caixa de seleção "Add a readme file" selecionada 2. Lista suspensa do gitignore com a opção "None" selecionada 3. Lista suspensa da licença com a licença MIT selecionada

 
Figura 3 - Captura de tela com as informações do passo 4  

5. Clique em “Create Repository”

Pronto, o novo repositório foi criado! 

Perceba que até essa etapa temos 2 arquivos no nosso repositório, são eles LICENSE e README.md, ambos localizados no ramo (branch) “main”.

2 Adicionando arquivos

Nesta etapa, adicionaremos novos arquivos, para isso abordaremos de duas maneiras distintas: através da interface e via linha de comando.

2. 1 Adicionando arquivos através da interface

1. Ainda no seu navegador (tela do repositório criado), clique no botão sinalizado com “+” ou “Add file”, posicionado na parte central da tela e selecione “Upload Files”

Utilizando leitor de tela: O leitor indicará a presença do menu “Add File”, acesse-o e em seguida selecione “Upload Files”  

Informação: 

Caso você não esteja na página do seu repositório, você poderá acessá-la através da url no seguinte padrão:

github.com/<proprietario>/<nomeRepositorio>

Ou acesse github.com, e busque pelo nome do seu repositório no campo de buscas denominado “Find a repository”

 


Figura 4 - Captura de tela sinalizando os cliques necessários  


2. Na tela que for apresentada, arraste arquivos para a região mostrada ou clique no botão “Choose your files” para buscar arquivos através do explorador de arquivos do Windows. Adicione um arquivo.  

Utilizando leitor de tela: O leitor indicará a presença do botão “Choose your files” selecione-o e adicione um arquivo para upload 

Figura da tela de upload mostrando a região para adição de arquivos e o botão para acessar os arquivos pelo explorador de arquivos do Windows

Figura 5 - Captura da tela para upload de arquivos

3. Na sequência, adicione informações pertinentes na seção “Commit Changes”, nos campos abaixo:

Resumo de commit
Descrição extendida de commit
Utilizando leitor de tela: O leitor indicará a presença dos campos “Commit summary” que é onde devemos inserir o resumo do commit e o campo “Optional extended description” onde devemos inserir detalhes adicionais do commit, se houver.

Captura da tela de upload explicitando os campos: Resumo de commit e Descrição extendida do commit E opção de commit direto na branch "main", que não está assinalada e opção para criar uma nova branch, que está assinalada


Figura 6 - Captura de tela de upload

4. Abaixo dos campos, devemos escolher se o commit será direto na branch “main” ou se haverá a criação de uma nova branch para esse commit. Escolha pela criação de uma nova branch e dê um nome adequado (informações sobre o passo 4 na Figura 6) 

Utilizando leitor de tela: O leitor indicará a presença do grupo “Commit choice” contendo duas possíveis escolhas: “Commit directly to the main branch” e “Commit a new branch for this commit and start a pull request” (antes de ler a segunda opção, o leitor falará o nome criado automáticamente para o novo branch que está em um campo editável junto da escolha)


Observação:

Essa ação, além de criar uma nova branch com o arquivo selecionado, criará também um pull request, não abordaremos em detalhes qual o impacto da criação de um pull request. Por ora, vamos focar apenas que estamos adicionando um arquivo e criando uma nova branch ao mesmo tempo no nosso repositório

5. A tela que temos agora é de abertura de um pull request. Adicione um título e uma descrição 

Utilizando leitor de tela: O leitor indicará a presença do campo “Add a title” onde devemos inserir o título da pull request e o controle de abas “Add a comment” que possui as abas “Write” e “Preview”. Selecionando a aba “write” podemos inserir o texto da descrição e navegar pelos controle para formatar o texto, já a aba de “preview” demonstra o estado final do texto.

Captura de tela mostrando os campos para preencher para criar a pull request

 Figura 7 - Captura de tela mostrando os campos para criação do pull request  

6. Clique no botão “Create pull request”, localizado logo abaixo da descrição e a direita 

Pronto, ao término desses passos temos: 

1 novo arquivo adicionado
1 nova branch 
1 pull request
Alternativamente, é possível criar uma nova branch separadamente e inserir arquivos diretamente nela, sem gerar um pull request.  

Explore essa possibilidade, acesse a página inicial, clique no link de branches, crie uma nova branch e adicione arquivos diretamente na branch (o procedimento é similar ao que já vimos nos passos acima).  

2.2 Adicionando arquivos através de linhas de comando

Requisitos: 

Um repositório criado no github.com
Software Git Bash já está instalado (Download aqui) 
Observação: 

Substitua os termos entre “<>” que estarão presentes nas instruções abaixo pelas informações do seu repositório/caso

Diversas vezes vamos nos referir a <proprietario> e <nomeRepositorio>, essas informações podem ser obtidas na url do seu repositório, conforme imagem abaixo:


Figura 8 - Captura da tela mostrando a url da página do repositório

Para este laboratório, os dados que serão utilizados como exemplo são:

Proprietário: jovisisa
Nome do repositório remoto (GitHub): gh4w
Antes de qualquer coisa, clonaremos o repositório do GitHub.  

2.2.1 Clone de repositório

Nesta etapa, clonaremos um repositório. A essência da clonagem de repositório é capturar um repositório remoto (criado no GitHub.com) e replicá-lo localmente. Ou seja, teremos um repositório git local igual ao existente remotamente, sendo esse repositório sua propriedade ou de outra pessoa.

Procedimento: 

Crie uma nova pasta em “Documentos”, essa será nossa pasta do repositório local git.
Abra o explorador de arquivos do Windows
Clique em “Documentos

Captura da tela do Explorador de arquivos mostrando a pasta Documentos

 

Figura 9 - Explorador de arquivos com a pasta Documentos selecionada


 3. Crie uma nova pasta  com o nome gh4w (botão direito do mouse, selecione new e depois Folder)


Figura 10 -  Tela do Explorador de arquivo windows com setas apontando para New e depois Folder para criação de uma pasta

2. Acesse a pasta e copie seu endereço

Captura de tela mostrando o clique na barra de endereço e a ação de copiar (control + c)


Figura 11 - Passos para captura do endereço da pasta


 3. Abra o Git Bash.  

Depois da instalação, vá até o menu iniciar e busque por Git Bash
Selecione Git Bash na lista de resultados, conforme figura abaixo:

Captura de tela com os passos: 1. Clique menu iniciar 2. Clique campo de busca 3. Digitação "Git Bash" no campo de busca 4. Clique na opção "Git Bash" na lista de resultados

Figura 12- Captura de tela mostrando os passos para abrir o Git Bash  


A tela que abrirá será semelhante a Figura 13, a seguir, mas o conteúdo em verde serão as informações relativas à sua própria maquina:

 Captura da tela inicial do Git Bash, que estamos chamando de terminal. Ela apresenta o seguinte conteúdo: "REDMOND+joasantos@DESKTOP-GV71ASL MINGW64 ~ $" (que é nossa localização) sendo que em verde temos "REDMOND+joasantos@DESKTOP-GV71ASL"

Figura 13 - Tela inicial do Git Bash


4. Com o terminal aberto, execute o comando a seguir para acessar a pasta criada anteriormente. Vide Figura 14

cd “<endereçoPasta>”

Dica: 

O endereço da pasta estará na área de transferência, pois foi copiado no passo 2. Então basta digitar cd e abrir aspas duplas, control+v e fechar aspas duplas

Captura de tela do terminal com o comando: cd 

Figura 14 - Captura de tela do terminal

5.Acesse github.com no seu navegador e vá até a página do seu repositório

6. Localize o botão “Code” e copie o link HTTPS


Utilizando leitor de tela: O leitor indicará a presença do menu “Code” (Code menu button), selecione-o. Dentro do menu, precisamos acessar o nível 2, onde existe a aba HTTPS e dentro desse contexto devemos acessar o botão “Copy URL to clipboard”.  

Captura de tela explicitando os cliques necessários na tela: menu Code, depois aba HTTPS e depois "Copy to clipboard"

Figura 15 - Captura de tela do repositório demonstrando onde está localizado o link a ser copiado 


 7. Execute o comando:  

      git clone <linkCopiado>

Dica: 

O link copiado já está na área de transferência, digite o comando git clone, depois control + v e depois enter

Imagem mostrando o comando: "git clone https://github.com/jovisisa/gh4w.git" e sua resposta: "Cloning into 'gh4w'... remote: Enumerating objects: 19, done. remote: Counting objects: 100% (19/19), done. remote: Compressing objects: 100% (15/15), done. remote: Total 19 (delta 2), reused 3 (delta 0), pack-reused 0 Receiving objects: 100% (19/19), 7.85 KiB | 2.62 MiB/s, done. Resolving deltas: 100% (2/2), done."


Figura 16- Comando git clone executado

Pronto, temos o clone do nosso repositório do GitHub em um repositório local. 

A pasta que criamos no passo 1 agora deve conter uma pasta, que é o nosso repositório clonado, contendo todos os arquivos do nosso repositório remoto. 

Pasta local com os arquivos clonados do repositório remoto. Perceba que dentro da pasta criada em Documentos, a ação de clone gera uma pasta que é o repositório remoto

Figura 17 - Pasta local com o clone feito

 
2.2.2 Adicionando arquivo através de linha de comando  

Procedimento: 

Voltando ao terminal, execute o comando:  cd <nomeRepositorio>
Informação: 

O comando acima nos levará até nosso repositório git local, que é o nosso repositório clonado. Perceba que o terminal indicará que agora estamos no nosso repositório e na branch “main”

2. Como boa prática, não devemos fazer alterações direto na “main”, execute o comando a seguir para criar uma nova branch:  git checkout -b <nomeBranchNova>

Informação: 

O comando acima realiza a criação da nova branch e já nos coloca nessa nova branch, ou seja, as alterações feitas nos passos seguintes estarão nesse escopo.

Captura de tela do terminal mostrando o comando: "$ git checkout -b BranchExemplo", a resposta: "Switched to a new branch 'BranchExemplo'" e a indicação da nossa nova localização: "REDMOND+joasantos@DESKTOP-GV71ASL MINGW64 ~/Documents/gh4w/gh4w (BranchExemplo)"

Figura 18 - Print do git bash com a execução do comando git checkout -b BranchExemplo  
3. Agora execute o comando:  touch <nomeDoArquivo>

Informação: 

Como exemplo, o nome do arquivo será “meu_novo_arquivo.txt”. Esse comando adicionará esse arquivo (que é um .txt vazio) ao meu repositório na branch “BranchExemplo”

4. Agora execute o comando: git add .

Informação: 

Utilizando o “.” aplicaremos o comando add a todos os arquivos da pasta, para selecionar arquivos específicos basta substituir o “.” pelo nome dos arquivos com suas extensões, exemplo: git add arquivo1.txt arquivo2.js

   Imagem mostrando o comando git add . (que não devolve nenhuma resposta)
Figura 19 - Comando git add

5. Em seguida, execute o comando: git commit -m "<Descrição>" 

Informação: 

Esse comando “comita” a alteração feita no repositório local, no nosso caso, a adição de 1 arquivo através do comando do passo 4 com o git add.

Perceba que o Git Bash detectará as alterações feitas e apontará que houve um arquivo alterado, ou seja, o arquivo que criamos na pasta no passo 3

Imagem mostrando o comando: "git commit -m"Meu novo commit" -m "Descrição do meu commit"" e sua resposta: " [BranchExemplo 7957ff0] Meu novo commit 1 file changed, 0 insertions(+), 0 deletions(-) create mode 100644 meu_novo_arquivo.txt"

Figura 20 - Comando git commit

6. Na sequência, execute o comando: git push --set-upstream origin <nomeBranchNova>
Imagem mostrando o comando: "$ git push --set-upstream origin BranchExemplo" e sua resposta: " Enumerating objects: 6, done. Counting objects: 100% (6/6), done. Delta compression using up to 8 threads Compressing objects: 100% (4/4), done. Writing objects: 100% (5/5), 635 bytes | 635.00 KiB/s, done. Total 5 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0) remote: Resolving deltas: 100% (1/1), done. remote: remote: Create a pull request for 'BranchExemplo' on GitHub by visiting: remote:      https://github.com/jovisisa/gh4w/pull/new/BranchExemplo remote: To https://github.com/jovisisa/gh4w.git * [new branch]      BranchExemplo -> BranchExemplo branch 'BranchExemplo' set up to track 'origin/BranchExemplo'."

Figura 21 - Comando git push

Informação: 

Note que o resultado até aqui é um pouco diferente da inserção de arquivos através da interface do GitHub, visto que não há uma criação automática de um pull request. Conforme já é sinalizado na resposta, que nos orienta a criar um pull request diretamente na interface do GitHub.

7. Acesse a página do seu repositório no navegador. Você receberá a indicação através de um banner de que ocorreram “pushes” na branch que foi criada no terminal, conforme a figura abaixo:  

Captura de tela da página inicial do repositório no GitHub, onde existe um banner com a inscrição: "BranchExemplo had recent pushes 6 minutes ago" ao lado de um botão com a inscrição: "Compare & pull request"

Figura 22 - Print do repositório


Utilizando leitor de tela: No contexto desse banner, o leitor indicará a presença de um link que terá o mesmo nome da sua branch e um outro link de “Compare & pull request”.

Conforme mencionado anteriormente, o foco nesta atividade não são os pull requests, isso será abordado mais a frente no curso. Com isso encerramos o passo-a-passo. 

Como sugestão final, busque explorar desafios mais complexos, como a edição de arquivos, como o README e o commit desses arquivos para suas branches originais ou novas branches. 

Parabéns por finalizar o conteúdo desta aula! 

Ao finalizar, utilize o template disponível abaixo. Clique no botão abaixo "Download" (lado direito) e  faça download do arquivo, preencha com as informações da atividade realizada, como print de telas e link do repositório. Após isso, faça o upload do arquivo clicando em "Selecionar arquivos para upload" (centralizado na tela embaixo de "Envie sua tarefa").

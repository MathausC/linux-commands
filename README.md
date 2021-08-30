# Primeiros comandos no linux (POP\_OS)

## Abrindo o terminal

Para rodarmos nosso comandos no terminal 'e necessario primeiro termos acesso a ele. Voce pode pressioar a tecla SUPER (Tecla Windows/command) e digitar terminal, ou usar o atalho SUPER+T.

Ao abrir o terminal vamos entender como ele se comunica conosco:

Perceba o que esta escrito na primeira linha do terminal. o nome antes da @ 'e o usuario que esta logado na sessao atual. A parte apos o @ a antes do espaco e o nome dado a maquina. Apos o espaco esta esquito em qual pasta o terminal pode interajir atualmente.

## Comandos

### *ls*

Lista os coteudos do diretorio atual. Se for acrescido a opcao *-l* apos o comando esse conteudo sera exibido em lista.

	ls -l

### *la*

Lista todo o conteudo do diretorio atual. Se for acrescido a opcao *-l* apos o comando esse conteudo sera exibido em lista.

	la -l

### *cd*

Muda para o diretorio indicada.

`cd ~` ou `cd`  para mudar para a home do sistema.

`cd /` para mudar para o diretorio root do sistema.

'cd ..` para voltar um diretorio acima.

### *touch*

Cria um arquivo dentro do diretorio atual com o nome informado.

`touch arquivo.txt` - para criar um aquivo txt vaxio com o nome *aquivo*.

### *rm*

Remove o aquivo informad.

'rm arquivo.txt` - para remover o arquivo criado.

Obs: o comando remover so consegue remover arquivos e nao diretorios. Para remover diretorios e necessario adicionar a opcao `-f -r` ou `-rf` onde o *-f* forca a remocao e o *-r* faz uma remocao recursiva, deletando todos os conteudos que estao contidos no diretorios filhos recursivamente (a ordem das opcoes nao e necessariamente importante).

	rm -fr pasta

### *mkdir*

cria um diretorio dentro do diretorio atual com o nome passado como parametro.

`mkdir pasta` - cria uma pasta com o nome pasta.

### *sudo*

Em alguns casos 'e necessario ter permissao de adminstrador para interagir com o sistema Linxux, entao o prefixo *sudo* cumpre esse papel de conceder ao usuario cadastrado no grupo *sudoers* o poder de acesso como *root*.

	sudo [comando]

### *apt* ou *apt-get*

O *apt-get*  e o gerenciador de pacotes do Ubuntu. 'E atraves dele que se instala aplicacoes contidas nos repositorios da canonical.

`sudo apt-get update` para atualizar os repositorios registados na sua maquina.

`sudo apt-get upgrade [programa]` para atualizar somente um programa ou mais.

`sudo apt-get full-upgrade` para atualizar todos os programas da maquina.

`sudo apt-get install [programa]` para instalar um programa ou mais. 

`sudo apt-get remove [programa]` para desinstar um ou mais programas.

`sudo apt-get install code` - instale o VSCode.

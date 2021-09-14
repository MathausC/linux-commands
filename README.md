# Primeiros comandos no linux (POP\_OS)

## Abrindo o terminal

Para rodarmos nosso comandos no terminal é necessário primeiro termos acesso a ele. Você pode pressionar a tecla SUPER (Tecla Windows/command) e digitar terminal, ou usar o atalho SUPER+T.

Ao abrir o terminal vamos entender como ele se comunica conosco:

Perceba o que está escrito na primeira linha do terminal. o nome antes da @ é o usuario que está logado na sessao atual. A parte após o @ a antes do espaço e o nome dado a máquina. Após o espaço está escrito em qual pasta o terminal pode interagir atualmente.

## Comandos

### *ls*

Lista os conteúdos do diretório atual. Se for acrescido a opção *-l* após o comando esse conteúdo sera exibido em lista.

	ls -l

### *la*

Lista todo o conteúdo do diretório atual. Se for acrescido a opção *-l* após o comando esse conteúdo sera exibido em lista.

`la -l`, `ls -a -l`, `ls -al` ou `ls -la`

### *cd*

Muda para o diretório indicado.

`cd ~` ou `cd`  para mudar para a home do sistema.

`cd /` para mudar para o diretório root do sistema.

'cd ..` para voltar um diretório acima.

### *touch*

Cria um arquivo dentro do diretório atual com o nome informado.

`touch arquivo.txt` - para criar um aquivo txt vazio com o nome *aquivo*.

### *rm*

Remove o aquivo informado.

'rm arquivo.txt` - para remover o arquivo criado.

Obs: o comando remover so consegue remover arquivos e não diretórios. Para remover diretórios e necessário adicionar a opção `-f -r` ou `-rf` (a ordem das opcoes não e necessariamente importante) onde o *-f* forca a remocao e o *-r* faz uma remocao recursiva, deletando todos os conteúdos que estáo contidos no diretórios filhos recursivamente.

	rm -fr pasta

### *mkdir*

Cria um diretório dentro do diretório atual com o nome passado como parametro.

`mkdir pasta` - cria uma pasta com o nome pasta.

### *sudo*

Em alguns casos é necessário ter permissao de adminstrador para interagir com o sistema Linxux, entao o prefixo *sudo* cumpre esse papel de conceder ao usuario cadastrado no grupo *sudoers* o poder de acesso como *root*.

	sudo [comando]

### *apt* ou *apt-get*

O *apt-get*  e o gerenciador de pacotes do Ubuntu. 'E atraves dele que se instala aplicacoes contidas nos repositórios da canonical.

`sudo apt-get update` para atualizar os repositórios registados na sua máquina.

`sudo apt-get upgrade [programa]` para atualizar somente um programa ou mais.

`sudo apt-get full-upgrade` para atualizar todos os programas da máquina.

`sudo apt-get install [programa]` para instalar um programa ou mais. 

`sudo apt-get remove [programa]` para desinstar um ou mais programas.

`sudo apt-get install code` - instale o VSCode.

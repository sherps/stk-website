---
title: Controlo da fonte
toc: true
---
O SuperTuxKart usa Git para o seu código fonte, e SVN para os arquivos de dados. Portanto, se tu não os tiveres, instale-os primeiro. Poderás encontrar instruções para os instalar na parte inferior da página.

## Núcleo do Jogo

O repositório do código principal está hospedado na nossa [página do GitHub](https://github.com/supertuxkart/stk-code). Exemplo de comando clone:

{%popup_code
git clone https://github.com/supertuxkart/stk-code.git stk-code%}

Tem aproximadamente 350 MB de tamanho.

Os arquivos de dados são hospedados no SourceForge e usam SVN. Exemplo de comando de checkout:

{%popup_code
svn checkout https://svn.code.sf.net/p/supertuxkart/code/stk-assets stk-assets%}

Tem aproximadamente 700 MB de tamanho.

Estes dois repositórios devem ser descarregados na mesma pasta, de modo a que as pastas `stk-code` e `stk-assets` estejam a beira uma da outra.

## Repositório da mídia

O repositório da mídia **não é necessário para jogar**. Contém os arquivos de origem para os recursos do jogo (ficheiros .blend, musica e sons sem perda de informação, etc.) e é destinado a artistas. Tem cerca de 3.2GB de tamanho em download.

O repositório da mídia está hospedado no SourceForge e usa SVN. Exemplo de comando de checkout:

{%popup_code
svn checkout https://svn.code.sf.net/p/supertuxkart/code/media/trunk stk-media-repo%}

Também vê [a página do repositório de mídia](Media_Repo).

## Diretrizes

Aqui estão algumas diretrizes para os desenvolvedores que têm acesso de gravação ao Git/SVN:

* Junta-te ao nosso canal de IRC ou Telegram (vê [Comunidade](Community)). Os desenvolvedores geralmente postam o que estão a trabalhar lá, para que a probabilidade de conflitos possa ser diminuída. Além disso, quaisquer bugs conhecidos em destaque também são discutidos lá.
* Talvez valha a pena inscreves-te na lista de e-mail de supertuxkart-commit (consulte [Comunidade](Community)) Todas as mensagens de commit são enviadas automaticamente para este endereço, para que tu estejas sempre ciente do que está a acontecer e se o teu trabalho interfere no que as outras pessoas fazem.
* A versão de desenvolvimento deve sempre compilar. Embora não seja possível testar em todas as plataformas, faça o possível para escrever código portátil. Outros desenvolvedores e testadores geralmente apontam (e corrigem) quaisquer problemas rapidamente.
* Faz commits com frequência. Commits frequentes têm a vantagem de atuarem como um backup, o que torna menos prováveis os ​conflitos de mesclagem demorados.
* Tenta incluir todas as alterações para um único recurso em um commit (ou seja, não faças um commit para cada arquivo separadamente) e tenta não misturar vários recursos num commit grande.

## Instalando o Git

### Linux
`sudo apt install git` ou o equivalente na tua distribuição escolhida.

### Windows
Instale o [Git para Windows](https://github.com/git-for-windows/git/releases/latest). Se quiseres uma interface gráfica para o Git, podes escolher a que te dá mais jeito. Caso contrário, se não souberes qual escolher, poderás instalar o [TortoiseGit](https://tortoisegit.org/download) após teres instalado o Git para Windows.

## Instalando o SVN

### Linux
`sudo apt install subversion` ou o equivalente na tua distribuição escolhida.

### Windows
Podes escolher entre vários clientes SVN e usar o que te dá mais jeito, mas se não souberes qual escolher, podes instalar o [TortoiseSVN](https://tortoisesvn.net/downloads.html).

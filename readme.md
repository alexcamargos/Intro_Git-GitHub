# Introdução ao Git e ao GitHub

Nesse curso vamos aprender um pouco da história do Git e como ele se tornou essencial para otimizar projetos dos desenvolvedores. Também vamos conhecer seus principais comandos, como funciona a plataforma e como ela pode simplificar o seu trabalho.

#### MRV .NET Developer
Bem-vindo ao bootcamp MRV .NET DEVELOPER é um programa gratuito para formação de desenvolvedores .NET com foco em soluções em C#, sendo a porta de entrada para conquistar uma oportunidade de contratação na MRV, a empresa parceira nos projetos da maior Construtora da América Latina.

​	Bootcamp ministrado [Otávio Reis](https://github.com/Perkles), na plataforma [Digital Innovation One](www.digitalinnovation.one).

<img src="/img/certificado.jpg" width="500px" align="center">

## Introdução ao Git

### SHA - Secure Hash Algorithm

A sigla **SHA** significa algoritmo de dispersão seguro (**s**ecure **h**ash **a**lgorithm em inglês), é uma função de dispersão criptográfica (ou função hash criptográfica) projetada pela Agência de Segurança Nacional dos Estados Unidos (NSA) sendo um Padrão Federal de Processamento de Informação dos Estados Unidos publicado pelo Instituto Nacional de Padrões e Tecnologia (NIST).

Os quatro algoritmos SHA são estruturados diferentemente e nomeados **SHA-0**, **SHA-1**, **SHA-2** e **SHA-3**. SHA-0 é a versão original da função de dispersão de 160 bits publicada em 1995 sob o nome "SHA". Publicada em 1995, SHA-1 é muito similar à SHA-0, mas altera a especificação de dispersão do SHA original para corrigir as fraquezas alegadas. SHA-2, publicada em 2001, é significantemente diferente da função de dispersão SHA-1. Em 2012, após uma longa competição, o NIST selecionou um algoritmo adicional, o Keccak, para padronização sob o título de [SHA-3](https://pt.wikipedia.org/wiki/SHA-3)

#### SHA-1

SHA-1 produz um valor de dispersão de 160 bits (20 bytes) conhecido como resumo da mensagem. Um valor de dispersão SHA-1 é normalmente tratado como um número hexadecimal de 40 dígitos. SHA-1 é a mais amplamente utilizada das funções de dispersão SHA existentes, sendo empregada em vários protocolos e aplicações amplamente utilizadas.

### BLOBS -> bolha

contém: tipo, tamanho, \0 e conteúdo

### TREES -> árvores

armazena e aponta para blobs diferentes e outras árvores diferentes, e também guarda o nome do arquivo. Tem sha1 conectados com as árvores, mudando um arquivo altera toda a estrutura

### COMMITS -> objeto que aponta para TREES

parente (último commit), autor, mensagem (exemplo "first commit") e timestamp (data e hora que foi criado) também possui hash sha-1.

## Navegação via Command Line Interface e instalação

### Interface de Linha de Comando - CLI

##### Windows Shell

O shell padrão no **Windows** é o _CMD.exe_ ou o Prompt de Comando (Command Prompt). De fato, a Microsoft tem usado o Prompt de Comando desde quando o MS-DOS era o principal sistema operacional da empresa.

###### Principais comandos

- cd 
- dir
- mkdir
- rmdir / del
- cls ou <ctrl + L>

##### Bourne Again Shell (Bash)

**Bash** é o acrônimo para **B**ourne **A**gain **Sh**ell. Ele foi desenvolvido pela Free Software Foundation. 

O Bash é um tipo de shell usado no MacOS e outras distribuições do Linux. No Linux, o Bash shell é só um dos muitos tipos de shell que o Linux pode usar. Outros tipos bem conhecidos são o Techs shell, Ksh shell e Zsh shell. Porém, você também pode usar o Bash Linux no Windows 10 (Subsistema Windows para Linux), se quiser.

###### Principais comandos

- cd
- ls
- mkdir
- rm -rf
- clear ou <ctrl + L>

## Primeiros comandos com Git

- **init** - Criar novo repositório.
- **clone** - obtém a cópia de um repositório Git existente.
- **add** - Adicionar arquivo/diretório ao staged area
  - *git add meu_arquivo* - para adicionar um arquivo específico.
  - *git add meu_diretorio* - para adicionar um diretório em específico.
- **rm** - Remover arquivo/diretório
  - *git rm meu_arquivo* - para remover um arquivo específico.
  - *git rm -r diretorio* - para remover um diretório em específico.
- **commit** - Comitar um arquivo.
- **push** - Atualizar os arquivos no branch atual.
- **pull** - Atualizar os arquivos no branch atual.
- **log** - Visualizar histórico
- **status** - Verificar estado dos arquivos/diretórios
- **remote** - Exibir os repositórios remotos.

## Ciclo de vida dos arquivos no Git

- **Traked** - git tem ciência deles (reconhecimento) subdividem-se em:
  - unmodified
  - modiefied
  - staged (arquivos que estão prontos fazer parte de outro tipo de agrupamento)

- **Untracked** - git tem ciência deles (reconhecimento), porem não controla suas alterações.

Ambiente de desenvolvimento:

- Working Directory
- Staging Area
- Local Repository 

## Introdução ao GitHub

**Remote Repository** - servidor remoto para centralizar o desenvolvimento, no nosso caso GitHub (https://github.com)

## Resolvendo conflitos

o que é um conflito?

Ocorre quando um mesmo arquivo possui versões diferente em dois ou mais repositórios.
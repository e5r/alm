Projeto de Especificação
========================

Um projeto de especificação é um projeto (repositório diferente, ou um diretório `doc` no projeto original)
que contém todos os elementos básicos da especificação em forma de arquivos textuais hiperligados. Dessa forma
pode evoluir (versões) junto ao próprio sowftware.

> Tanto o software quanto sua documentação são incrementais e evolutíveis.

Contento por exemplo:

* Funcionalidades
* Regras (de Negócio ou Apreasentação)
* Mensagens
* Protótipos
* Manuais
* Etc.

Regras que definem um projeto de especificação
----------------------------------------------

* Os arquivos devem ser textuais, portanto podem usar qualquer extensão de arquivo texto conhecido,
  mas todos devem usar a mesma extensão
  - Exemplos de extensão: `.txt`, `.md`, `.org`, `.rst`
* Deve haver um arquivo inicial chamado `index` ou `home`
  - Por não ser _case sensitive_, não importa se é `home` ou `Home, ou `HOME`, mas sugerimos usar
    tudo em minúsculo.
* Não devem haver os dois arquivos iniciais, `index` e `home`, somente um dos dois
* Os demais arquivos podem seguir qualquer estrutura, inclusive em subdiretórios aninhados, mas
  todos devem estar ligados de alguma forma ao arquivo inicial.

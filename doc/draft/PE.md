Projeto de Especificação
========================

Um projeto de especificação é um projeto (repositório diferente, ou um diretório `doc` no projeto original)
que contém todos os elementos básicos da especificação em forma de arquivos textuais hiperligados.
Dessa forma pode evoluir junto ao próprio sowftware.

> Tanto o software quanto sua documentação são incrementais e podem evoluir.

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
  mas todos devem usar a mesma extensão. Podem inclusive não ter nenhuma extensão
  - Exemplos de extensão: `.txt`, `.md`, `.org`, `.rst`
  - Recomendamos o uso da extensão `.md` [Markdown](https://pt.wikipedia.org/wiki/Markdown)
* Deve haver um arquivo inicial chamado `index` ou `home` na raiz do projeto
  - Por não ser _case sensitive_, não importa se é `home` ou `Home, ou `HOME`
  - Recomendamos usar `home`, com tudo em minúsculo
* Não devem haver os dois arquivos iniciais, `index` e `home`, somente um dos dois
* Os demais arquivos podem seguir qualquer estrutura, inclusive em subdiretórios aninhados, mas
  todos devem estar ligados de alguma forma ao arquivo inicial
* Você pode usar a estrutura que preferir e o fluxo que quiser, mas isso deve estar minimamente
  documentado e disponível em um arquivo chamado `workflow` também na raiz do projeto
* O seu processo documentado em `workflow` vai definir como a documentação deverá ser escrita,
  por isso você também deve fornecer na raiz do projeto um arquivo `template` contendo um exemplo
  de como os documentos devem ser escritos. Caso você use mais de um _template_ use um subdiretório
  chamado `template` e lá vários arquivos com os exemplos.

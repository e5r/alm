SEP - Software Evolution Proposal
=================================

**Em português:** PES - Proposta de Evolução de Software

> Nota: A nomenclatura ainda carece de revisão, mas a ideia por tráz é refletir os vários processos
> listados ao final dessa seção em sua base fundamental, ou seja, o fato de haver uma proposta
> inicial, uma revisão e aprovação, uma especificação (não necessariamente nesta ordem), uma
> implementação, uma avaliação e aprovação de tal implementação, e por fim uma integração e
> lançamento oficial.

## Resumo

Toda evolução de um software é __causada__ por uma ideia. E ideias devem ser explanadas
e aceitas, antes de serem implementadas.

## Motivação

Para complementar o que foi explanado no documento [PE], acreditamos que o software
sendo algo vivo que evolui naturalmente, a sua evolução deve ser bem organizada e
documentada.

Quando falamos de documentação, logo pensamos em [Casos de Uso][UC], [Regras de Negócio][RN]
e [Documentos de Especificação][SPEC], etc. Sim, estamos falando disso também, mas quando
falamos em _"bem organizada e documentada"_ queremos dizer que deve existir um processo
bem definido para que o software evolua.

Tudo deve iniciar em uma ideia (_eu já escrevi sobre isso em algum lugar, quando achar o link
coloco aqui_), seja a ideia para uma nova funcionalidade, ou a ideia de consertar
algo. Não importa o quê, mas tudo começa com uma ideia.

Essa ideia por sua vez deve ser expressada, para que com essa manifestação, outros tenham
conhecimento da mesma e que possam avaliá-la, ou simplesmente para que seja avaliada pelo
próprio individuo que a teve, pois o exercício da escrita nos força a estruturar melhor
as nossas ideias. Deve haver uma discussão, uma prototipação, uma exemplificação,
e por fim uma decisão de realmente considerá-la viável. Isso já ocorre normalmente em nossas
mentes e reuniões, e conferências remotas; mas queremos documentá-las.

Após considerada viável, deve-se especificá-la (aí sim entra os [Casos de Uso][UC],
[Regras de Negócio][RN] e [Documentos de Especificação][SPEC]), e por fim construí-la
causando a evolução do software. Mas agora, após o software evoluir temos documentado
inclusive os caminhos que levaram a sua evolução, sua motivação, e etc.

Lembremos das várias ferramentas para gestão de desenvolvimento de software que existem:

* [Azure DevOps][AZDEVOPS]
* [Trello]
* [Jira], e tantas outras

Essas ferramentas já nos permitem fazer isso seguindo inúmeros padrões de mercado já estabelecidos,
e, vale ressaltar, de forma excepcional.

Mas acabam, no fim, sendo _uma coisa_ totalmente à parte do nosso software propriamente dito;
porque você não consegue _enxergar_ esse processo no seu projeto (arquivos, códigos, etc). E o que
queremos aqui é tornar isso também parte de nosso projeto, de forma que seja _palpável_ e visível.

Imagine então a situação onde, você já iniciou o projeto usando uma ferramenta, e depois percebeu
que deveria mudar para outra, e depois para outra. Isso é uma realidade, e só quem já passou
por uma migração desse tipo sabe o quão pode ser problemático. Certo, existem maneiras de
fazer isso com ferramentas disponíveis, mas elas nunca farão o trabalho perfeito de forma automática,
pois sempre haverá a necessidade de ajustes manuais.

O que quero dizer é que até mesmo o processo de evolução, o gerenciamento de _vida_ de nosso
software pode ser _palpável_ em um projeto de **documentação viva** ([Isso foi tirado do texto da
Microsoft sobre as propostas para a linguagem C#][CSharpQuote]).

Até mesmo uma ideia que parecia boa a princípio e que depois foi rejeitada, deve ser documentada,
e servir para algo no futuro. Afinal, ela não foi aceita a princípio, mas foi considerada em
algum momento, e isso pode ser útil no futuro.

## Detalhamento

O que propomos é que toda mudança no software deve iniciar como uma proposta, e deve ser descrita
em um arquivo textual simples, que passa por um crivo de avaliação, e se aprovado, será documentado
com os padrões determinados pela equipe e por fim, implementado e liberado em uma nova versão do
software.

Então nosso diretório de documentação (_Projeto de Especificação_ - leia [PE] para mais informações) terá essa estrutura:

```
./project/
  ├─ doc/
  │  ├─ specs/
  │  │  ├─ feature-a/
  │  │  ├─ feature-b/
  │  │  ├─ feature-a.md
  │  │  └─ feature-b.md
  │  ├─ seps/
  │  │  ├─ sep-01-feature-a.md
  │  │  ├─ sep-02-feature-b.md
  │  │  ├─ sep-04-feature-d.md
  │  │  └─ rejected/
  │  │     └─ sep-03-feature-c.md
  │  └─ index.md
  └─ README.md
```

O arquivo **README.md** você já conhece, nele temos um link para as funcionalidades (que estão no
arquivo **doc/index.md**), nesse arquivo estão listadas todas as funcionalidades e as propostas
que estão sendo analisadas.

> Ainda temos alguns arquivos que foram omitidos aqui para simplificar o entendimento. Seriam eles: doc/global-messages.md (mensagens globais), doc/global-business-rules.md (regras de negócio globais) e doc/global-presentation-rules.md (regras de apresentação globais)

No exemplo acima, temos duas funcionalidades já aceitas (**doc/specs/feature-a.md** e
**doc/specs/feature-b.md**), essas são especificações das funcionalidades em si, e cada uma delas
pode conter outros arquivos de especificação auxiliares (nos subdiretórios **doc/specs/feature-a/**
e **doc/specs/feature-b/**) com regras de negócio, de apresentação, protótipos, etc.

Ao mesmo tempo podemos ver que elas foram originadas de **SEP's** (**doc/seps/sep-01-feature-a.md** e
**doc/seps/sep-01-feature-b.md**). Também podemos perceber que existe uma proposta que ainda está
em andamento (**doc/seps/sep-04.feature-d.md**), e sabemos que ela ainda está em andamento porque não
existe uma especificação para ela (uma especificação seria um arquivo de especificação em
**doc/specs/** e um subdiretório para a mesma). Por fim, percebemos que existe uma proposta que não foi aceita devido a existência do arquivo **doc/seps/rejected/sep-03-feature-c.md**.

Com isso, mesmo que você não tenha uma ferramenta para gerenciar o projeto, ainda o conseguirá fazer, e de forma ordenada com esse processo de evolução, usando apenas um simples editor de textos.

Não estamos reinventando a roda, muitos outros projetos importantes usam essa mesma técnica
(vejam os links úteis abaixo). O que estamos propondo aqui é uma forma prática de aplicá-la a nossos projetos do dia a dia.

### Modelos

* Um exemplo de arquivo de proposta pode ser visto em [sep-template.md][sep-template]
* Um exemplo de arquivo de especificação pode ser visto em [sep-spec-template.md][sep-spec-template]

## Links úteis

* [Python Enhancement Proposals][PEP]
* [PHP Standards Recommendations][PSR]
* [C# Language Proposals][CSLP]
* [Java Specification Requests][JSR]
* [Rust RFCs][RUST-RFC]
* [Tcl Improvement Proposals][TCL-TIP]

[PE]: PE.md
[UC]: https://pt.wikipedia.org/wiki/Caso_de_uso
[RN]: https://pt.wikipedia.org/wiki/Regras_de_neg%C3%B3cio
[SPEC]: https://pt.wikipedia.org/wiki/Engenharia_de_requisitos
[AZDEVOPS]: https://azure.microsoft.com/pt-br/services/devops
[Trello]: https://trello.com/
[Jira]: https://br.atlassian.com/software/jira
[CSharpQuote]: https://github.com/dotnet/csharplang/tree/master/proposals#c-language-proposals
[PEP]: https://www.python.org/dev/peps/
[PSR]: http://www.php-fig.org/psr/
[CSLP]: https://github.com/dotnet/csharplang/tree/master/proposals
[JSR]: https://www.jcp.org/en/jsr/all
[sep-template]: sep-template.md
[sep-spec-template]: sep-spec-template.md
[RUST-RFC]: https://github.com/rust-lang/rfcs
[TCL-TIP]: https://core.tcl-lang.org/tips/doc/trunk/tip/0.md

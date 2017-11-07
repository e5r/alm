E5R ALM (Application Lifecycle Management)
==========================================

> Versão __1.0.0-alpha1__

Este repositório contém um guia prático para implantação do Gerenciamento de Ciclo de Vida de Aplicativos (ALM - Application Lifecycle Management) em um time de desenvolvimento sem experiência no assunto, ou em um time experiente, porém, que precisa implantar ALM em uma fábrica com processos legados.O time de desenvolvimento E5R ([E5R Development Team][E5R]) usa esse guia prático como processo oficial de ALM.

## Motivação

Foi percebido que apesar de existir inúmeras especificações (veja o tópico _Referências_ abaixo), e que essas já são bastante consolidadas no mercado, inclusive com incontáveis casos de sucesso; é difícil a adoção de tais padrões em um contexto prático no meio corporativo de desenvolvimento de software.

É comum participar de equipes envolvidas em projetos que devem seguir uma ou mais das especificações citadas por força contratual. Seria algo bom o fato de ingressar em uma dessas equipes, se não fosse o fato de que as mesmas não conseguem ser __produtivas__. E não é uma questão de falta de especialização profissional, pois não é raro encontrar em tais equipes profissionais certificados (inclusive contratualmente se exigem tais profissionais certificados). Então porque a falta de produtividade? Será que os processos em si são falhos, ou os casos de sucesso são _maquiados_? Cremos que não é o caso.

Supomos que por tais padrões serem bastante flexíveis para uso de propósito geral, e que, para serem flexíveis prevêem extensões e customizações; essas extensões e customizações não recebem a devida atenção por parte dos gestores no momento da implantação.

Como resultado temos, por um lado, inúmeros contratos mal elaborados que inclusive replicam textos de modelo das especificações como sendo restrições, por parte de empresas contratantes de serviços de software; e por outro lado, empresas que aceitam tais contratos imaginando que poderão (e podem na verdade) adequar o processo em andamento mesmo que o contrato esteja com uma ___falha de elaboração___.

Acrescente a esse resultado, o fator da rotatividade profissional nas empresas de [TI][TI_WIKI], e ainda, a [lacuna que existe no mercado de profissionais dessa área][NOTICIA_FALTA_TI]; obrigando as equipes a diminuir o investimento em capacitação e troca de informações entre o time e priorizando o atendimento aos prazos em detrimento da qualidade da entrega. O que temos é um __caos__ na execução de tais contratos: Fases invertidas com artefatos de construção sendo entregues obrigatoriamente na fase de elaboração; engenharia reversa em protótipos não funcionais; desgaste entre as equipes multidisciplinares causado pelo fenômeno ___"toma que a bola tá contigo"___, onde o que importa é seguir o que está escrito no contrato independente se é certo ou errado e não atentando para o princípio da _razoabilidade_.

Enfim, não creio que o cenário acima seja algo desconhecido para a maioria dos profissionais de [TI][TI_WIKI] envolvidos do processo de desenvolvimento de softwares. Por isso resolvemos escrever este guia prático para implantação de processo ALM em uma fábrica de softwares, priorizando o entendimento de cada passo apresentado nos padrões um por vez, e, buscando elucidar os motivos que levaram os mesmos a serem escritos; ou seja, o problema que cada um resolve.

## O Guia

Este guia é desenvolvido e entregue de forma incremental, seguindo o próprio modelo de entrega de softwares. Você encontra uma primeira versão contendo apenas este texto introdutório, e depois pode ir navegando nos lançamentos de novas versões e acompanhando as mudanças.

Dessa forma, uma versão final e mais completa do processo estará sempre disponível abrangendo o maior número de cenários possíveis e com um maior número de projetos corporativos aderentes. Mas também, um processo mais simples sempre poderá ser seguido usando versões anteriores. E ainda, mesmo que a versão final e mais completa desse guia seja a mais adequada ao projeto requerido, sempre se poderá usar o incremento das versões como forma de capacitar os novos membros da equipe; atendendo desde aos menos experientes com o estudo à partir da primeira versão, quanto aos mais experientes à partir do ponto em que for mais adequado na linha de liberação de versões.

### Quer implantar este processo em seu projeto/corporação?

Para implantar o processo de ALM apresentado neste guia em um projeto e/ou corporação, siga os passos abaixo:

1. Publique em um canal oficial de sua corporação/equipe uma nota de aderência ao processo ALM deste guia,
   incluindo a versão adotada, e na nota a explícita aceitação aos termos da licença disponível no
   arquivo _LICENSE_;
2. Caso haja aceitação a novas versões, essa deve ser divulgada novamente no canal oficial;
3. Treinar sua equipe e seguí-lo.


# Referências

* [Definição ALM][ALM_WIKI]
* [Definição de Engenharia de Software][ENG_WIKI]
* [Definição de Qualidade de Software][QA_WIKI]
* [Definição de Teste de Software][TESTE_WIKI]
* [Definição de CMMI][CMMI_WIKI]
* [Definição de RUP][RUP_WIKI]
* [Definição de TI][TI_WIKI]

> Leia também [TGDS][TGDS] e [PE][PE]

[E5R]: https://e5r.github.io "E5R Development Team"
[ALM_WIKI]: https://pt.wikipedia.org/wiki/Application_lifecycle_management "Application Lifecycle Management"
[ENG_WIKI]: https://pt.wikipedia.org/wiki/Engenharia_de_software "Engenharia de Software"
[QA_WIKI]: https://pt.wikipedia.org/wiki/Qualidade_de_software "Qualidade de Software"
[TESTE_WIKI]: https://pt.wikipedia.org/wiki/Teste_de_software "Teste de Software"
[CMMI_WIKI]: https://pt.wikipedia.org/wiki/CMMI "CMMI"
[RUP_WIKI]: https://pt.wikipedia.org/wiki/IBM_Rational_Unified_Process "RUP"
[TI_WIKI]: https://pt.wikipedia.org/wiki/Tecnologia_da_informa%C3%A7%C3%A3o
[NOTICIA_FALTA_TI]: http://classificados.folha.uol.com.br/empregos/2014/06/1466085-faltam-45-mil-profissionais-de-ti-no-brasil.shtml
[TGDS]: TGDS.md
[PE]: PE.md

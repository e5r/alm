Notas sobre gestão ágil de projeto de software
==============================================

## Aplicar Scrum

Devemos usar Scrum como base para tudo que descrevemos aqui.

## Fluxos devem ser descritos

Todo fluxo deve ter uma documentação que o descreva, inclusive com gráficos.
Assim cada profissional pode focar no trabalho que o interessa.

> Exemplo de gráfico descrevendo um processo de iteração.
```mermaid
sequenceDiagram
    participant R as Requester
    participant O as Runtime Owners
    participant F as API review board <br> (FXDC)
    R ->> O: Files issue under dotnet/runtime
    note over O: Assigns owner
    
    note over R, O: Discussion

    O ->> F: Label api-ready-for-review
    
    note over F: Performs review

    alt is accepted
        F ->> R: Label api-approved
    else is work needed
        F ->> O: Label api-needs-work
    else is rejected
        F ->> R: Issue is closed
    end
```

## Processo de desenvolvimento descrito

O processo de desenvolvimento como um todo deve estar descrito (em uma Wiki por exemplo) e acessível a todos
para que seja transparente todo o processo.

### Roadmap

Deve dar visibilidade ao _Roadmap_ como um documento (wiki) que descreve o planejamento geral da equipe, com
links interativos, imagens e links para itens de trabalho na ferramenta usada. Deve explicar como é feito
o planejamento, quais os valores considerados, a duração, etc. do próprio _roadmap_ além de exibi-lo.

No _roadmap_ também é um bom local para apresentar os _temas_. Mesmo que não use temas como itens de
trabalho, eles devem ser exibidos no roadmap porque apontam onde o foco deve ser depositado.

Não há necessidade de guardar histórico do roadmap, ex: roadmap-2021, roadmap-2022, etc., basta manter
"o roadmap" atualizado para que todos o usem como bússola para todo o trabalho atual sendo executado.

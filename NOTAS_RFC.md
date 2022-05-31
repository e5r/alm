# SPECIFICATION

> Software Specification / Especificação de Software

* Produzida á partir de um requisito de software
* É a documentação para construção
* Produz alguns itens padronizados
  - Descrição funcional
  - Relação entre funcionalidades/subfuncionalidades
  - Descrição de cenários através de fluxos
    - FP - Fluxo Principal
    - FA - Fluxos Alternativos
    - FE - Fluxos de Exceção
  - Regras de Negócio
  - Protótipos e Regras de Apresentação
  - Mensagens

# REQUIREMENT

> Software Requirement / Requisito de Software

- É uma solicitação de construção formal
- Pode conter protótipos, fluxos negociais, apresentações

# RFC

> Request For Comments / Pedido de comentários

- É uma demanda
- É uma ideia
- Produz discussão entre os envolvidos
- Produz um requisito de software

# Grandes demandas
```
[doc:RFC] -> [doc:REQUIREMENT] -> [doc:SPEC] -> [branch:new.baseline] -> [code/deploy/test]
                                      |
                                      +-- [workitem]
```

# Demandas menores de mudanças e correções
```
[doc:SPEC] -> [branch:use.baseline] -> [code/deploy/test]
    |
    +-- [workitem]
```

# Notas

O processo de RFC nas comunidades open source vem para solucionar um problema específico:

* Evitar "ao máximo" que os seguintes problemas ocorram durante o desenvolvimento
  - Detectar inviabilidade técnica de construção
  - Detectar conflitos com outras funcionalidades
  - Detectar grandes mudanças e retrabalho de construção
  - Perder oportunidade de ser melhor ainda

Quando não usamos RFC os problemas são detectados já no momento do desenvolvimento, o que
gera mal uso dos recursos e da força de trabalho, e que gera desperdício.

Quando usamos RFC "damos uma chance" de evitar tais problemas antes que ocorram.

Usar RFC evita desperdícios e maximiza a força de construção.

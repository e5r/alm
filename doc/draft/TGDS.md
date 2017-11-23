Teoria Geral do Desenvolvimento de Software
===========================================

> Por Erlimar Silva Campos (erlimar@gmail.com)

1. O software é um organismo mecânico/digital engatilhado para
executar uma ação transformadora de um dado.

>	**Com isso temos:** 1. Por ser um organismo (seja mecânico,
	digital ou de outra  natureza), é formado por um sistema
	de órgãos, por isso, orgânico.

2. Por ser um sistema orgânico, há interação entre as peças,
nesse caso, órgãos. Essa interação, requer coerência entre os
pontos de conexão, ou seja, a interface deve ser definível.

> **Com isso temos:** 1. Peça, `com objetivo definido`, interfaces
	conhecidas (com formato `TO` e direção) e órgãos
	interligados. 2. Por cada órgão ser bem definido, é possível dizer
  que são independentes, ainda que não funcionem sozinhos, podem ser
  construídos sozinhos.

3. O órgão projetado, pode ser produzido em unidades menores,
ou seja, átomos (unidades indivisíveis).

> **Com isso temos:** 1. Para produzir um órgão com átomos,
	precisamos dos pré-requisitos do órgão. Sabendo que tipo
	de átomo, sabemos que materiais (tecnologias) são
	necessárias para concebê-lo. 2. Um átomo é uma peça que pode
  ser medida, portanto, precificada.
	
A Teoria Geral do Desenvolvimento de Software diz que:
"Um software é ORGÂNICO, tem CONEXÕES e é dividido em ÁTOMOS"

Para produzir um sóftware precisamos seguir o fluxo:

```
  +-------(1)-+     +-------(1)-+     +---------(1)-+     +-------(1)-+
  | Definir o | __\ |  Extrair  | __\ | Identificar | __\ |  Extrair  |
  | Sowftware |   / | os Órgãos |   / |  Conexões   |   / | os Átomos |
  +-----------+     +-----------+     +-------------+     +-----------+
        .                                                      |
       /|\                                                    \|/
        |                                                      '
        |                                               +---------(1)-+
        |                                               | Identificar |
        |                                               | Req. Átomos |
  +-----------+                                         +-------------+
  | Continua? |                                               |
  +-----------+           E5R ALM SYSTEM                     \|/
        .                                                     ' 
       /|\                                              +---------(1)-+
        |                                               |  Solucionar |
        |                                               | Req. Átomos |
        |                                               +-------------+
        |                                                     |
        |                                                    \|/
        |                                                     '
  +---------(1)-+     +------(1)-+     +-------(1)-+     +--------(1)-+
  | Categorizar | /__ | Entregar | /__ | Construir | /__ | Precificar |
  |   Órgãos    | \   |  Átomos  | \   |  Átomos   | \   |   Átomos   |
  +-------------+     +----------+     +-----------+     +------------+

```
	
 * Definir o Software: O que o software deve fazer
   > O software é um conjunto de funcionalidades categorizados
 * Extrair os Órgãos: Quais peças fundamentais (limite por ciclo)
 * Identificar Conexões: Definir interfaces, com ações e dados
 * Extrair os Átomos: Quais peças indivisíveis compõem o órgão?
 * Identificar Requisitos dos Átomos: Que técnicas serão necessárias para construir o átomo?
 * Solucionar Requisitos dos Átomos: Apontar soluções para atender cada requisito.
   > Uma tecnologia pode ser integrada, ou criada
   > Toda tecnologia criada, pode requerer outros requisitos
 * Precificar Átomos: Dar prazo para construção/integração de cada átomo
 * Construir Átomos: Construir artefatos em si NO PRAZO precificado
   > O prazo do mesmo se refere ao limite para construção de cada átomo
 * Entregar Átomos: Apresentar átomos prontos/não prontos
   > Não conseguiu construir NO PRAZO? É um átomo entregue como NÃO PRONTO
   > Empacotar e gerar versão da entrega
 * Categorizar Órgãos: Quanso se chega ao final, com o produto entregue é possível
   dizer a que categoria pertence cada órgão.
 * Decidir continuar: Um software nunca para de evoluir se alguém não para de produzí-lo.
   Se decidir continuar, é só começar novamente do princípio.

E5R ALM SYSTEM
==============

## Sugere:

1. Cada quadro acima representa um STATUS em um processo de desenvolvimento de software.
2. Cada ETAPA deve ter um tempo limite para execução.
   > Cada número acima de cada quadro representa o prazo para sua execução, em proporção de unidade
   
   > Esse tempo deve ser determinado por cada gestor de projeto
      
   > Porém, deve seguir uma proporção de uma mesma unidade
   
   > Se uma unidade foi definida para 10 minutos. O tempo limite para cada etape é a multiplicação
     de seu número x 10 minutos.
3. As etapas são sucessivas.
4. A execução de todas as etapas completa um CICLO.

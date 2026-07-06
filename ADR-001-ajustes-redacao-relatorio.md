# ADR 001: Ajustes de redação no relatório do ShopISEL

## Estado
Aceite

## Contexto
Durante a revisão do relatório, foram identificadas várias expressões consideradas vagas, pouco rigorosas ou demasiado subjetivas por parte do arguente. Os pontos assinalados concentravam-se no Resumo, na Introdução e na secção do List Service:

- Uso de expressões pouco precisas como "garantindo consistência e fiabilidade".
- Utilização de adjetivos genéricos, como "aparentemente simples" e "num ambiente mais confortável".
- Referência a "contas" sem explicitar que se trata de contas de utilizador.
- Necessidade de clarificar o significado de `claim` no contexto do `OwnerId`.
- Necessidade de explicar que os itens são tratados como coleção completa e não apenas como nomes isolados.
- Necessidade de ligar o campo `version` ao mecanismo de concorrência otimista e citar a referência académica correspondente.

## Decisão
Foram feitos os seguintes ajustes no texto do relatório:

- O Resumo foi reescrito para substituir formulações genéricas por linguagem mais técnica e verificável.
- A Introdução foi ajustada para remover adjectivos subjetivos e substituir "ambiente mais confortável" por "computador".
- A descrição da arquitetura foi afinada para referir "contas de utilizador" em vez de "contas".
- A secção do List Service foi atualizada para:
  - explicar que `OwnerId` é obtido a partir do claim `sub` do token JWT;
  - esclarecer que um `claim` é uma afirmação codificada no token com atributos do utilizador;
  - indicar que a API trabalha com a coleção completa de itens da lista;
  - explicitar que o campo `version` é a base do mecanismo de concorrência otimista;
  - associar esse mecanismo ao artigo de Kung e Robinson.
- Foi adicionada a referência bibliográfica para o artigo `On optimistic methods for concurrency control`.

## Consequências
- O relatório passa a usar linguagem mais objetiva e defensável em contexto académico.
- As secções afetadas ficam mais precisas do ponto de vista técnico.
- O mecanismo de concorrência otimista fica melhor justificado e suportado por literatura.
- O documento ganha consistência terminológica entre Resumo, Introdução e Trabalho Desenvolvido.

## Ficheiros Alterados

- `report/tex/5_resumo.tex`
- `report/tex/capitulo1.tex`
- `report/tex/capitulo4.tex`
- `report/bibdatabase.bib`


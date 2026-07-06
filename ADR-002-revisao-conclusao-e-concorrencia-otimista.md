# ADR 002: Revisão da conclusão e da concorrência otimista no relatório do ShopISEL

## Estado
Aceite

## Contexto
Na revisão do relatório, foram identificados novos pontos que exigiam maior rigor conceptual e maior honestidade descritiva:

- A expressão "dados heterogéneos" surgiu sem definição.
- A descrição da concorrência otimista precisava de ligação explícita ao artigo de Kung e Robinson.
- O uso de `Guid` como versão podia ser interpretado como inconsistente com modelos sequenciais clássicos de versionamento.
- A secção de Considerações Finais precisava de distinguir claramente o que foi realmente feito, o que ficou por fazer e o que seria necessário para aproximar o trabalho de um processo A-SDLC.
- A formulação "práticas de engenharia de software bem estabelecidas" era demasiado afirmativa sem explicitar quais práticas tinham sido efectivamente adoptadas.

## Decisão
Foram adoptados os seguintes ajustamentos:

- A expressão "dados heterogéneos" passou a ser explicitada como informação proveniente de fontes com estruturas, formatos e níveis de detalhe distintos.
- A secção sobre concorrência otimista passou a referir diretamente o artigo de Kung e Robinson como base conceptual.
- O texto passou a explicar que, embora o artigo de referência descreva mecanismos tipicamente sequenciais ou estruturados, o projeto usa `Guid` como token de versão no contexto do Entity Framework Core, por ser a opção concreta implementada no sistema.
- As Considerações Finais passaram a adotar um tom mais crítico e verificável:
  - o texto descreve o que foi feito de facto;
  - identifica o que não foi implementado;
  - enquadra o trabalho em relação ao paradigma A-SDLC;
  - refere que o uso de LLMs foi assistivo e não totalmente agentic.
- Em vez de uma afirmação genérica sobre "boas práticas", a conclusão passou a listar práticas concretas utilizadas no projeto, como decomposição por serviços, contratos explícitos, contentorização, \ac{CI/CD}, testes de integração e revisão iterativa.

## Consequências
- O relatório ganha precisão terminológica e evita afirmações excessivamente genéricas.
- A conclusão fica mais defensável em contexto académico, porque separa implementação real de ambição metodológica.
- O uso de `Guid` fica contextualizado como escolha de implementação, e não como regra universal de versionamento.
- O documento passa a alinhar melhor o discurso técnico com o grau real de adoção de práticas A-SDLC.

## Ficheiros Alterados

- `report/tex/capitulo4.tex`
- `report/tex/capitulo8.tex`
- `report/bibdatabase.bib`


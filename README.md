# ALCPA
Aplicação de Lista de Compras com Preços e Alertas

## Resumo

Neste projeto o teu grupo vai ser desafiado a fazer um sistema completo from start to finish, com a publicação em app stores e go live. Para isso vão usar LLMs para gerar o código enquanto garantem a qualidade de todos os componentes produzidos.
Propomos a criação de uma aplicação mobile para gestão de listas de compras, pensada para uso rápido em contexto real (ex.: supermercado) e respetivo ecossistema de microserviços formalizando APIs de backend e web app para backoffice.
A solução permite selecionar produtos, marcar itens durante a compra e consultar preços associados a diferentes lojas e localizações, com a possibilidade de definir alertas de preço para determinados produtos.
O sistema inclui mecanismos de gestão central de dados (produtos, preços, lojas) e uma componente de push notifications para alertas da alteração da lista.
Vão ainda demonstrar um conceito de White Label development, no qual o desenvolvimento das Apps mobile e web serão baseadas num Design System que será customizado num segundo pipeline.

Tecnologias
•	React Native
•	Leitura de códigos de barras através da câmara
•	Georreferenciação de preços
•	Aplicações web em React.
•	Backend com Serviços com API REST bem definidas e domínios bem delimitados construídos em dotnet.
•	Integração com o Keycloak como Identity Provider para configuração de utilizadores e integração com outros IdP.
•	Push Notifications integrado com Firebase Cloud Messaging
•	CI/CD 
	Dois pipelines de CI/CD:
	Build, deploy e testing da versão White Label
	Customize, build, deploy e testing da versão customizada.
o	Deploy em ambiente público
o	publicação para app stores (Android e IOS)
•	Uso de AI LLMs como apoio ao desenvolvimento e validação – Plataforma Github Copilot integrada com VS Code.

Este projeto cruza desenvolvimento mobile, web, backend e dados, obrigando a lidar com temas como performance, sincronização, modelação de dados e fiabilidade de alertas. É indicado para alunos que querem compreender como aplicações simples podem escalar para serviços digitais completos e sustentáveis.

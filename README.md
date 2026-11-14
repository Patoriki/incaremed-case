# InCareMed: Prontuário Eletrônico, App do Paciente e Extensão para Profissionais

> Estudo de caso. O código-fonte é privado e pertence à **RJF Consultoria**. Este repositório apresenta o projeto e a minha participação nele. As imagens usam **dados fictícios**.

## O problema
Os municípios precisam de um sistema único para registrar atendimentos, acompanhar o histórico de cada paciente e oferecer serviços digitais à população. Ao mesmo tempo, os **profissionais da ponta** (nas unidades e em campo) perdem tempo trocando de sistema para consultar dados e falar com pacientes e colegas.

## A solução
O **InCareMed** é uma plataforma de saúde para a gestão municipal:
- 📋 **Prontuário eletrônico** para os profissionais de saúde
- 📱 **App do paciente** para acompanhar a própria saúde e acessar os serviços
- 🧩 **Extensão de navegador para os profissionais** (veja abaixo)
- 🎙️ **Integração com o SOMA**: teleconsulta e prontuário preenchido automaticamente por IA no formato SOAP
- 🏷️ **White-label**: cada município pode exibir o sistema com o próprio nome

### A extensão de navegador (ideia minha)
Criei a ideia de uma extensão que acompanha o profissional da ponta enquanto ele trabalha no navegador:
- 👁️ **Visualização rápida dos dados do paciente**, sem sair da tela em que ele está
- 💬 **Comunicação** com o paciente e **entre os profissionais**
- 📹 **Criação de teleconsultas**
- 🔀 **Regulação**: encaminhamentos e solicitações direto pela extensão
- 🤖 **Ferramentas de IA** que automatizam processos do dia a dia

## Arquitetura
```
[ App do paciente / Painel do profissional ]  ←  Angular
[ Extensão de navegador ]                     ←  JavaScript
                    │
               API REST (.NET / C#)  ──►  Ferramentas de IA
                    │
               SQL Server
                    │
               [ SOMA: teleconsulta + SOAP por IA ]
```

## Minha participação
- **Idealizei a extensão de navegador** e desenvolvi a extensão
- Desenvolvimento do **front-end** em Angular
- **Participação no back-end** (.NET/C#), maior do que nos outros sistemas da empresa
- Implementação de **acessibilidade** no app do paciente: ajuste do tamanho da letra, leitor de tela, VLibras, navegação pelo teclado, entre outros


## Tecnologias
**Front-end:** Angular · TypeScript · Bootstrap · Font Awesome · SweetAlert2
**Back-end:** C# · .NET · SQL Server
**Extensão:** JavaScript · HTML · CSS


## Telas
![Prontuário](prints/01-prontuario.png)
![Extensão](prints/02-extensao.png)
![Chat](prints/03-chat.png)
![Responsividade](prints/04-responsividade.png)
![Acessibilidade](prints/05-acessibilidade.png)

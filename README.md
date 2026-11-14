# InCareMed: Prontuário Eletrônico e App do Paciente

> Estudo de caso. O código-fonte é privado e pertence à **RJF Consultoria**. Este repositório apresenta o projeto e a minha participação nele. As imagens usam **dados fictícios**.

## O problema
Os municípios precisam de um sistema único para registrar atendimentos, acompanhar o histórico de cada paciente e oferecer serviços digitais à população, como a teleconsulta, sem depender de vários sistemas desconectados.

## A solução
O **InCareMed** é uma plataforma de saúde para a gestão municipal com:
- **Prontuário eletrônico** para os profissionais de saúde
- **App do paciente** para acompanhar a própria saúde e acessar os serviços
- **Extensão de navegador** que cria teleconsultas direto do fluxo de atendimento
- **Integração com o SOMA**, a plataforma de teleconsulta
- **White-label**: cada município pode exibir o sistema com o próprio nome

## Arquitetura
```
[ App do paciente / Painel do profissional ]  ←  Angular
                    │
               API REST (.NET / C#)
                    │
               SQL Server
                    │
[ Extensão de navegador ] ──► [ SOMA (teleconsulta) ]
```

## Minha participação
- Desenvolvimento full-stack de funcionalidades (.NET + Angular)
- **Criei a extensão de navegador** que gera teleconsultas a partir do sistema
- Implementação de **acessibilidade** no app do paciente: ajuste do tamanho da letra, leitor de tela, VLibras, navegação pelo teclado, entre outros
  <!-- ajuste esta lista para o que já está pronto -->

## Tecnologias
C# · .NET · Angular · TypeScript · SQL Server · Extensão de navegador (JavaScript)

## Telas
<!-- Coloque prints com dados fictícios na pasta /prints e referencie aqui, por exemplo:
![Prontuário](prints/prontuario.png)
-->

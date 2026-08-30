# Brasileirão App - SDUI

<img width="200" alt="AppIcon_brasileirao" src="https://github.com/user-attachments/assets/6b64d4d1-5b27-4497-8d77-d84933691bf7" />

![Swift Version](https://img.shields.io/badge/Swift-5.5%2B-orange)
![Platform](https://img.shields.io/badge/Platform-iOS%2013%2B-lightgrey)
![Architecture](https://img.shields.io/badge/Architecture-MVVM-blue)
[![CI Build & Unit Test](https://github.com/SelecaoGlobocom/raquel-calazans/actions/workflows/ci.yml/badge.svg)](https://github.com/SelecaoGlobocom/raquel-calazans/actions/workflows/ci.yml)

Este repositório contém a implementação de um aplicativo para acompanhamento de jogos de futebol, consistindo em uma API backend e um aplicativo cliente para iOS. A solução foi desenvolvida com foco em arquitetura moderna, escalabilidade e qualidade de código.

### Arquitetura Geral

O projeto foi estruturado como um "monorepo" contendo dois subprojetos principais:

* **`./api`**: Uma API RESTful desenvolvida com **Java e Spring Boot**.
* **`./ios-app`**: Um aplicativo nativo para iOS desenvolvido com **Swift, SwiftUI e SwiftData**.

A decisão de arquitetura mais impactante foi a implementação de um modelo de **UI Guiada pelo Servidor (Server-Driven UI)**, onde a API define a estrutura de agrupamento dos jogos (ex: por status ou por rodada), e o cliente iOS apenas renderiza a estrutura recebida.

### Detalhes de Cada Projeto

Para informações detalhadas sobre a arquitetura, stack de tecnologias, instruções de setup, testes e decisões de design de cada parte do projeto, por favor, consulte seus respectivos `README`s:

* ➡️ **[Documentação da API (Backend)](./api/README.md)**
* ➡️ **[Documentação do App (iOS)](./ios-app/README.md)**

### Resultados

O agrupamento dos jogos depende de como os dados chegam. Ou seja, por status (ENCERRADOS, AO VIVO, AGENDADOS), ou por rodadas (1ª RODADA, 2ª RODADA, 3ª RODADA), ou de qualquer outra forma, bastantando ajustar o JSON.

| Por status | Por rodadas |
| :---: | :----: |
| ![por_status](https://github.com/user-attachments/assets/85ada342-622c-4f85-a50b-047056b6c6e1) | ![por_rodadas](https://github.com/user-attachments/assets/5564c4ad-f8ae-482b-9b98-2ce6d2fdd7e3) |




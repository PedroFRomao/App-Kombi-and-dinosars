# Kombi and Dinosaurs - App Informativo

O **Kombi and Dinosaurs** é um jogo desenvolvido como parte do nosso TCC, e este aplicativo tem como objetivo fornecer uma visão detalhada sobre o jogo. Através do app, os jogadores poderão explorar a história do jogo, conhecer os personagens, entender as mecânicas e como cada fase do jogo funciona.

## 📂 Divisão do Projeto

O aplicativo é dividido em 4 principais telas, cada uma com funcionalidades específicas que ajudam na navegação e interação do usuário.

### 1. **Home**
- **Objetivo**: Apresentar uma visão geral do jogo, com uma sinopse da história, uma imagem que leva o usuário para uma página contendo a HQ do jogo, e informações sobre os integrantes da equipe de desenvolvimento. Ao clicar na foto de cada integrante, o usuário é direcionado para uma página com a biografia, currículo e projetos anteriores.

### 2. **Personagens**
- **Objetivo**: Apresentar os personagens principais do jogo e suas características.
  
### 3. **Controles**
- **Objetivo**: Explicar as mecânicas e os controles utilizados durante o jogo.

### 4. **Fases**
- **Objetivo**: Detalhar as fases do jogo, explicando os desafios e objetivos de cada uma.

## 📂 Estrutura do Projeto

A estrutura do código está organizada da seguinte maneira:

``` bash
KombiAndDinosaursApp/
├── assets/                           # Imagens e ícones
├── lib/                              # Código fonte do app
│   ├── models/                       # Modelos de dados do jogo
│   │   ├── IntegranteCardData.dart
│   │   └── app_colors.dart
│   ├── screens/                      # Telas do app
│   │   ├── controles.dart
│   │   ├── fases.dart
│   │   ├── historia.dart
│   │   ├── main.dart
│   │   └── personagens.dart
│   ├── widgets/                      # Widgets personalizados para o app
│   │   ├── IntegrantePerfil.dart
│   │   ├── custom_bottom_nav.dart
│   │   ├── custom_footer.dart
│   │   └── integranteCard.dart
├── pubspec.yaml                      # Dependências e configurações do Flutter
└── README.md                         # Este arquivo README
```

## 🛠️ Funcionalidades no Código

Aqui estão algumas das funcionalidades implementadas no código para as seções mencionadas:

- **Navegação**: A navegação entre as páginas do app (História, Personagens, Controles, Fases) é feita utilizando o `Navigator` do Flutter, permitindo uma transição fluida entre as telas.
  
- **Carrossel de Personagens e Fases**: 
  - Utilização do widget `CarouselSlider` para implementar carrosséis interativos nas telas de **Personagens** e **Fases**, onde o usuário pode deslizar entre diferentes itens.
  
- **Listagem de Personagens e Fases**: 
  - Na tela de **Personagens**, usamos um `ListView` para exibir uma lista de personagens com suas descrições.
  - Na tela de **Fases**, outra lista é utilizada para mostrar as fases do jogo com informações sobre os desafios de cada uma.

- **Interface de Usuário (UI)**: 
  - Para organizar os elementos de forma clara e atraente, foram usados widgets como `Column`, `Row`, `Container` e `ListView` para exibir os conteúdos de maneira responsiva.
  
- **Estrutura de Dados**: 
  - O app utiliza classes para representar dados do jogo, como **Personagens** e **Fases**, permitindo que o conteúdo seja facilmente alimentado e modificado.


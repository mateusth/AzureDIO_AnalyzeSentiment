# Análise de Sentimentos com AI Foundry - Azure

Este repositório documenta minha experiência utilizando o **Azure AI Foundry** para realizar **Análise de Sentimentos** em textos de usuários, como avaliações de produtos ou acomodações. Além de identificar se uma revisão foi **positiva, neutra ou negativa**, o serviço também permite analisar o **conjunto de palavras** utilizadas para classificar cada sentimento.

Além disso, testei a funcionalidade de **detecção de idioma** e implementei um **chat baseado no GPT-4**, configurando um narrador personalizado para gerar histórias interativas.

---

## 📌 Sobre o Projeto

O objetivo deste projeto foi explorar os recursos do **AI Foundry no Azure**, focando em três principais funcionalidades:

1. **Análise de Sentimentos**: Classificação de textos como **positivos, neutros ou negativos**, juntamente com a análise detalhada das palavras-chave utilizadas no processo.
2. **Detecção de Idioma**: Identificação automática do idioma de uma determinada frase.
3. **Chat com GPT-4**: Implantação de um modelo GPT-4 personalizado para responder a perguntas e gerar histórias baseadas em um narrador com características específicas.

---

## ⚙️ Etapas do Processo

### 🔹 1. Configuração Inicial
- Acesse o **Azure AI Foundry** e crie um **recurso** para utilizar os serviços de Machine Learning.
- No menu à esquerda, clique em **Playground** e depois em **Language Playground**.

  ![Site AZURE FOUNDRY](1 - Azure AI Foundry.jpg)

  
  ![Create playground](2 - create playground.jpg)


### 🔹 2. Análise de Sentimentos  
- Dentro do **Language Playground**, selecione a opção **Classificar Texto** e depois **Analisar Sentimento**.
- Escolha o idioma do texto a ser analisado.
- **Habilite a mineração de opinião** para identificar as palavras-chave utilizadas na classificação do sentimento.
- Insira os textos de avaliação um por um e clique em **RUN** para processar a análise.
- O resultado exibirá:
  - 🔹 O **sentimento geral** da avaliação (**positivo, neutro ou negativo**).
  - 🔹 A análise detalhada de **termos-chave** usados para determinar o sentimento.


  ![Exemplo de Análise de Sentimentos](3 - classify.jpg)

  ![Exemplo de Análise de Sentimentos](4 - opinion.jpg)

---

### 🔹 3. Detecção de Idioma  
- Após a análise de sentimentos, testei a funcionalidade **Detect Language**.
- Insira uma frase em qualquer idioma e execute a análise.
- O sistema identificou corretamente o idioma, confirmando a eficácia do modelo.

  ![Linguage Idioma](5 - Detect Language.jpg)

---

### 🔹 4. Criação de um Chat com GPT-4  
- No **AI Foundry**, fui até a seção de **Deploy** e escolhi criar um novo **modelo de chat**.
- Selecionei o **GPT-4** como modelo base.
- Configurei as **características do narrador**, personalizando sua personalidade e tom de voz.
- Fiz um **input solicitando a geração de uma história**, conforme mostrado no print abaixo:

  ![Configuração do Chat com GPT-4](6 - chat.jpg)

- O chat gerou um texto baseado na configuração do narrador, mostrando a capacidade de personalização do modelo.

---

## 📊 Resultados  

### ✅ Análise de Sentimentos  
O **Azure AI Foundry** conseguiu identificar corretamente o **sentimento geral** das avaliações testadas e destacou palavras-chave que influenciaram a classificação. Isso permite uma análise mais profunda do feedback dos usuários.

### ✅ Detecção de Idioma  
O modelo identificou corretamente o idioma das frases inseridas, confirmando sua precisão.

### ✅ Chat com GPT-4  
O chat gerou uma história de forma coerente, seguindo as características do narrador configurado.

---

## 🛠️ Tecnologias Utilizadas

- **Microsoft Azure**: Plataforma de computação em nuvem utilizada para hospedar o projeto.
- **Azure AI Foundry**: Serviço de Machine Learning para processamento de linguagem natural.
- **Análise de Sentimentos**: Classificação de textos e mineração de opinião.
- **Detecção de Idioma**: Identificação automática do idioma de um texto.

---

## 🎯 Conclusão  

Este projeto foi uma ótima experiência para entender como o **AI Foundry** pode ser utilizado para análise de sentimentos, processamento de linguagem natural e criação de **modelos interativos** de texto.

A análise de sentimentos demonstrou como as palavras-chave influenciam na classificação de um texto, e a **mineração de opinião** mostrou detalhes valiosos sobre os termos mais relevantes.

O **modelo de chat com GPT-4** permitiu a criação de um narrador personalizado, mostrando como é possível ajustar a IA para diferentes tipos de interações.

No futuro, pretendo integrar esses modelos com outras APIs para criar aplicações mais robustas e interativas.

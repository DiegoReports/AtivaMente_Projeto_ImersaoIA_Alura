# 🏃🌳AtivaMente : Seu Coach de Bem-Estar Ativo ao Ar Livre

## Objetivo 🎯

O projeto AtivaMente tem como objetivo fornecer suporte e motivação para usuários interessados em atividades físicas ao ar livre. Através de uma série de agentes inteligentes 🧠, o sistema analisa o estado do usuário 🤔, oferece recomendações personalizadas ✨ e sugestões de locais seguros 🗺️, culminando em mensagens motivacionais 💪 para incentivar um estilo de vida ativo e saudável 🌱.

## Tecnologias e Ferramentas Utilizadas 🛠️

* **Google Agent Development Kit (ADK):** Framework para a construção e orquestração dos agentes inteligentes.
* **Google Gemini API:** Modelo de linguagem avançado 💬 utilizado pelos agentes para processamento de linguagem natural e geração de texto.
* **`transformers` Library (Hugging Face):** Utilizada para análise de sentimentos 😄🙁😐 nas mensagens do usuário, empregando o modelo pré-treinado `nlptown/bert-base-multilingual-uncased-sentiment`.
* **Python 🐍:** Linguagem de programação principal para o desenvolvimento do projeto.
* **Google Colaboratory 🧪:** Ambiente de desenvolvimento utilizado para prototipagem e execução do código.
* **Markdown 📝:** Formato utilizado para a criação deste README e para formatação de texto exibido ao usuário (via `IPython.display.Markdown`).

## Agentes Inteligentes 🤖

O sistema AtivaMente é composto por quatro agentes principais, cada um com uma função específica no fluxo de interação com o usuário:

### 1. Agente Analisador de Estado (`agente_analisador`) 🤔

* **Descrição:** Este agente é responsável por analisar a mensagem inicial do usuário para identificar seu estado físico 💪, emocional 😊🙁 e nível de motivação 🔥 em relação à prática de atividades ao ar livre. Utiliza análise de sentimentos (via `transformers`) para compreender o tom emocional da mensagem.

### 2. Agente Recomendador (`agente_recomendador`) ✨

* **Descrição:** Com base na análise do estado do usuário fornecida pelo `agente_analisador` e na mensagem original 💬, este agente gera recomendações de ações ou planos apropriados 💡. As recomendações consideram o estado físico 💪, emocional 😊🙁 e o nível de motivação 🔥 do usuário, buscando ser específicas e práticas.

### 3. Agente Sugestor de Rotas (`agente_sugestor_rotas`) 🗺️

* **Descrição:** Este agente tem como objetivo sugerir locais e rotas seguras ✅ para a prática de atividades físicas ao ar livre. Ele considera a proximidade 📍, a segurança dos locais 🛡️, a relevância para o estado do usuário 🤔 e suas preferências 💖, sempre incluindo avisos importantes sobre segurança (trânsito 🚦, condições climáticas ☀️🌧️, sinalizações locais ⚠️).


### 4. Agente de Mensagens (`agente_mensagens`) 💪

* **Descrição:** Este agente pega as recomendações geradas pelo `agente_recomendador` e as formata em uma mensagem final amigável 🤗, motivacional 🎉 e inspiradora 🌟 para o usuário. O objetivo é encorajar o usuário a seguir as recomendações e a se engajar em atividades ao ar livre 🌱.


## Fluxo de Interação 🔄

1.  O usuário envia uma mensagem descrevendo seu estado ou intenções 💬.
2.  O `agente_analisador` processa a mensagem e identifica o estado físico 💪, emocional 😊🙁 e nível de motivação 🔥 do usuário.
3.  O `agente_recomendador` utiliza essa análise para gerar recomendações de atividades ou planos 💡.
4.  O `agente_sugestor_rotas` (opcionalmente) sugere locais e rotas seguras ✅ para as atividades 🗺️.
5.  O `agente_mensagens` formata as recomendações (e a sugestão de rota, se disponível) em uma mensagem final motivadora 🎉 para o usuário.
6.  A mensagem final é apresentada ao usuário 📤.

## Considerações Futuras 🚀

* **Integração com APIs de Clima ☀️🌧️:** Implementar um agente ou uma ferramenta para obter informações climáticas em tempo real e considerá-las nas recomendações e sugestões de rotas.
* **Personalização Avançada 👤:** Coletar e utilizar mais informações sobre as preferências do usuário (tipos de atividades favoritas 💖, horários preferenciais ⏰, objetivos 🎯) para recomendações mais personalizadas.
* **Integração com Mapas/Localização 🗺️📍:** Utilizar APIs de mapas para fornecer sugestões de rotas mais precisas e informações sobre locais próximos.
* **Feedback do Usuário 👍👎:** Implementar um sistema para coletar feedback dos usuários sobre as recomendações e sugestões para melhorar a qualidade do sistema ao longo do tempo.
* **Suporte Multimodal 🗣️🖼️:** Expandir a capacidade do sistema para lidar com diferentes tipos de entrada (voz, imagens) e fornecer respostas mais ricas.

Este README fornece uma visão geral do projeto AtivaMente. Para detalhes de implementação e código 💻, consulte os arquivos fonte do projeto.
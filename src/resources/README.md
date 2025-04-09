# 🌐 Azure Language Service - Sentiment Analysis & Opinion Mining

Este documento descreve o processo de uso do **Azure Language Service** para realizar **Análise de Sentimentos** e **Extração de Opiniões** (Sentiment and Opinion Mining) sobre sentenças em linguagem natural. A atividade foi parte de um estudo prático para compreender as capacidades da IA na interpretação de emoções humanas e avaliações subjetivas em textos.

---

## 🚀 O que é o Azure Language Service?

O **Azure Language Service** é uma oferta de IA da Microsoft para análise de linguagem natural. Ele permite processar texto para extrair insights como:

- Sentimento geral (positivo, negativo, neutro)
- Mineração de opiniões (opiniões associadas a entidades específicas)
- Extração de frases-chave
- Detecção de linguagem
- Classificação de texto customizada

---

## 🔍 Como funciona a análise de sentimentos com mineração de opinião?

O serviço avalia cada sentença de forma individual, identificando:

- **Sentimento geral**: classificado como positivo, negativo ou neutro.
- **Confiança**: uma pontuação (score) de confiança associada a cada classificação.
- **Opiniões**: pares de **alvo** (target) e **opinião** (assessment), revelando sobre o que a pessoa está falando e o que ela acha disso.

---

## 🧪 Sentenças analisadas

### ✅ 1. "I loved that trip to Alaska five years ago, we went to that fantastic place to see the northern lights."

**Resultado da análise:**
- **Sentimento geral**: Positivo
- **Frases-chave extraídas**:
  - "trip to Alaska"
  - "fantastic place"
  - "northern lights"
- **Mineração de opinião**:
  - **Alvo**: trip → **Opinião**: loved
  - **Alvo**: place → **Opinião**: fantastic

**📌 Insight**: O modelo foi capaz de associar adjetivos positivos às experiências e locais mencionados, destacando a viagem como um evento memorável e prazeroso. Isso é útil, por exemplo, em avaliações de viagens, turismo ou análise de satisfação.

---

### ❌ 2. "I hate when people don't listen to me, I'm your customer, you should give me the opportunity to say whatever I'd like to say."

**Resultado da análise:**
- **Sentimento geral**: Negativo
- **Frases-chave extraídas**:
  - "people don't listen"
  - "customer"
  - "opportunity to say"
- **Mineração de opinião**:
  - **Alvo**: people → **Opinião**: don't listen (negativa)
  - **Alvo**: customer → **Opinião implícita**: exige respeito e voz

**📌 Insight**: O modelo capturou claramente o tom de frustração e exigência por empatia e escuta. Esse tipo de análise é extremamente valioso para **análise de feedback de clientes**, **suporte ao consumidor** e **monitoramento de reputação de marca**.

---

## 💡 Possibilidades de Uso

- Atendimento ao cliente: identificar automaticamente emoções em reclamações ou elogios.
- Análise de redes sociais: detectar menções negativas ou positivas em tempo real.
- Pesquisas de satisfação: automatizar a categorização de sentimentos em respostas abertas.
- Recursos Humanos: analisar feedbacks internos de forma agregada.

---

## 🛠 Tecnologias e Ferramentas

- **Azure Language Studio** (interface gráfica para testes rápidos)
- Linguagem: **Inglês**
- Tipo de análise: `SentimentAnalysis` com `OpinionMining = true`

---

## 🧠 Conclusão

A utilização do Azure Language Service com **opinion mining** revelou-se uma ferramenta poderosa para extrair não apenas o tom emocional de frases, mas também as **opiniões específicas ligadas a entidades relevantes**. Isso fornece contexto, tornando a análise mais rica e acionável.

> 💬 Mesmo em frases complexas ou emocionais, o serviço demonstrou precisão e sensibilidade à nuance humana, essencial para aplicações modernas de IA em NLP.

---
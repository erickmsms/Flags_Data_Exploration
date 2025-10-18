# 🌍 Análise Estatística das Bandeiras dos Países

Este projeto explora as relações entre os **elementos visuais das bandeiras nacionais** e fatores **geográficos, culturais e religiosos**, utilizando a base de dados *Flag Database* (UCI Machine Learning Repository).  
O objetivo foi identificar **padrões visuais, simbólicos e históricos** que refletem aspectos identitários das nações — desde influências coloniais até tendências ideológicas e religiosas.

---

## 📊 Principais Etapas

1. **Exploração e Limpeza de Dados**
   - Utilização da *Flag Database*, contendo 194 países e mais de 30 atributos.
   - Conversão e tratamento de variáveis categóricas, binárias e numéricas.
   - Verificação de correlações e consistência entre atributos.

2. **Análise Exploratória de Dados (EDA)**
   - Criação de **matriz de correlação** entre elementos das bandeiras e fatores geográficos.
   - Identificação de relações significativas, como:
     - 🇬🇧 *Crosses ↔ Saltires* (influência britânica)
     - 🐆 *Animate ↔ Colours* (bandeiras com animais tendem a ter mais cores)
     - 📏 *Population ↔ Area* (países maiores tendem a ter mais habitantes)
   - Estudo da **cor predominante por continente**, revelando influências políticas e culturais:
     - 🔴 Vermelho — Ásia, Europa e América do Sul (socialismo / revoluções)
     - 🟢 Verde — África (pan-africanismo / islamismo)
     - 🔵 Azul — América do Norte e Oceania (democracia / tradição ocidental)

3. **Criação de Métrica de Complexidade**
   - Definição de uma métrica própria para *complexidade da bandeira*, somando elementos visuais (estrelas, ícones, textos, etc.).
   - Avaliação da relação entre **área territorial e complexidade visual** (r = 0.369).

4. **Aplicação do Classificador Ingênuo de Bayes**
   - Estimativa de probabilidades condicionais, como:
     - `P(Muçulmano | Lua Crescente) = 72.73%`
     - `P(Marxista | Ásia e Vermelho) = 18.75%`
   - Implementação para verificar consistência entre análise empírica e probabilística.

5. **Testes de Hipótese**
   - Comparação de médias populacionais e número de estrelas em bandeiras.
   - Utilização de **teste t** e intervalos de confiança (95%):
     - População média ≠ 5 milhões (p = 0.0062)
     - Número médio de estrelas ≠ 5 (p = 0.0000)

---

## 🧠 Principais Insights

- **História e geopolítica moldam mais o design das bandeiras do que a geografia.**
- **Símbolos religiosos** são, na maioria, exclusivos a tradições específicas (cristianismo, islamismo).
- **Cores predominantes refletem ideologias**, especialmente durante o contexto da Guerra Fria.
- **Complexidade visual** está mais ligada à história e identidade nacional do que ao tamanho territorial.

---

## 🧰 Tecnologias Utilizadas

- Python (Pandas, NumPy, Matplotlib, Seaborn, Scipy)
- Jupyter Notebook
- CSV Data Handling
- Estatística Descritiva e Inferencial
- Visualização de Dados


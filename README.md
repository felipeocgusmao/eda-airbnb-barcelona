# Análise de Alojamentos Airbnb — Barcelona

## Descrição
Análise exploratória e modelo preditivo de preços de alojamentos Airbnb em Barcelona, com dashboard interativo.

## Objetivo
Identificar padrões de preço e qualidade para apoiar decisões no setor de turismo e hotelaria.

## Dataset
- Fonte: Kaggle — Comparative Analysis of Airbnb Prices in Barcelona
- 300 alojamentos com informação de preço, zona, tipo e valoração

## Como usar

### Dashboard interativo
```bash
pip install -r requirements.txt
streamlit run app.py
```

### Pipeline de análise
```bash
python src/analise.py   # gera gráficos em outputs/
python src/modelo.py    # treina modelo e exibe métricas
```

### Testes
```bash
pytest test.py -v
```

## Deploy no Streamlit Cloud

1. Acesse [share.streamlit.io](https://share.streamlit.io) e faça login com GitHub
2. Clique em **New app**
3. Selecione o repositório `felipeocgusmao/projeto_1`
4. Branch: `main` · Main file: `app.py`
5. Clique em **Deploy**

## Análises realizadas
- Preço médio por bairro (Top 10)
- Distribuição por tipo de alojamento
- Relação entre valoração e preço por noite
- Previsão de preço com Random Forest (MAE ≈ 10€ · R² ≈ 0.80)

## Conclusões
- Os bairros mais caros são Complejo Residencial, El Putxet i el Farró e Eixample
- A maioria dos alojamentos são quartos privados (~63%)
- Preço alto não garante melhor avaliação

## Tecnologias
- Python · Pandas · Matplotlib · scikit-learn · Streamlit

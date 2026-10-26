# Previsão da Precipitação e Classificação do Risco Pluviométrico na Província de Maputo

Comparação entre SARIMAX, Random Forest e XGBoost na previsão da precipitação diária e na classificação do risco pluviométrico, com dados ERA5 (1995–2024, 10.957 observações diárias).
[![DOI](https://zenodo.org/badge/1434180217.svg)](https://doi.org/10.5281/zenodo.23662484)
[Ler o preprint (PDF)](Previsao-Precipitacao-Maputo.pdf)

**Autor:** Gaio Cotane Joao Magaia, DARTA'ACOS, Maputo, Moçambique
**Contacto:** cotanegayo@gmail.com

## Principais resultados

- Tendência decrescente fraca mas significativa na precipitação diária (Mann–Kendall, p = 0,0104).
- O Random Forest optimizado superou o SARIMAX(1,0,1): MAE 2,3569 mm, RMSE 5,6975 mm, R² = 0,1567.
- Variáveis mais importantes: precipitação do dia, pressão média e precipitação acumulada em 7 dias.
- Classificação de risco: melhor resultado com XGBoost (acurácia balanceada 0,3159, F1 macro 0,3097); nenhum modelo identificou eventos de chuva extrema.
- Os modelos devem apoiar a decisão, e não funcionar como sistemas autónomos de alerta.

## Conteúdo do repositório

- `precipitacao.py`: código da análise e dos modelos
- `main.tex`: fonte LaTeX do preprint
- `Previsao-Precipitacao-Maputo.pdf`: versão em PDF

## Dados

ERA5 (Copernicus Climate Change Service). Os dados brutos não estão incluídos neste repositório e podem ser descarregados no Copernicus Climate Data Store.

## Como citar

Magaia, G. C. J. (2026). *Previsão da Precipitação e Classificação do Risco Pluviométrico na Província de Maputo*. Preprint. DOI: ([![DOI](https://zenodo.org/badge/1434180217.svg)](https://doi.org/10.5281/zenodo.23662484))

## Licença

Código: MIT.

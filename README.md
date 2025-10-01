#  Projeto de Previsão de Sucesso de Startups

**Mariana Lacerda Reis - T16**  
*Projeto de análise de dados para competição Kaggle*



## Sobre o Projeto

Este projeto desenvolve um modelo preditivo capaz de identificar startups com maior probabilidade de sucesso no mercado, utilizando dados históricos de financiamento, localização, setor e marcos alcançados.

**Objetivo:** Atingir acurácia mínima de 80% na previsão de sucesso de startups.



## Estrutura do Projeto

###  **Notebooks Principais**
- **`kaggleMariana.ipynb`** - Notebook principal com análise completa e modelo final

### **Submissões Kaggle**
```
submissões/
├── submission_final.csv              # Submissão principal (78.26%)
├── submission_800trees.csv           # RandomForest com 800 árvores (77.09%)
├── submission_ensemble_7seeds.csv    # Ensemble de 7 modelos
├── submission_80_percent.csv         # Tentativa de otimização
├── submission_calibrated_adjusted.csv # Modelo calibrado
└── submission_threshold_corrigido.csv # Ajuste de threshold
```

### **Tentativas e Experimentos**
```
tentativas/
├── tentativaInicial.ipynb    # Primeira abordagem, na qual tentei fazer uma exploração de dados bem básica conforme aprendido e minha primeira versão.
├── Tentativa2.ipynb          # Segunda iteração
├── tentativa3.ipynb          # Terceira tentativa
├── tentativa4.ipynb          # Quarta versão
├── tentativa5.ipynb          # Quinta iteração
└── tentativa6.ipynb          # Sexta tentativa
```

###  **Dados e Configuração**
- **`train.csv`** - Dataset de treino (646 exemplos)
- **`test.csv`** - Dataset de teste (277 exemplos)
- **`sample_submission.csv`** - Template de submissão
- **`requirements.txt`** - Dependências Python



## Resultados Alcançados

### **Performance do Modelo**
- **Acurácia Final:** 78.26%
- **Validação Cruzada:** 78.48% (10-fold)
- **Features Selecionadas:** 18 (via RFECV)
- **Modelo:** RandomForest com hiperparâmetros otimizados





## Metodologia

1. **Análise Exploratória** - EDA completa com visualizações
2. **Feature Engineering** - Criação de 18+ features derivadas
3. **Seleção de Features** - RFECV para otimização automática
4. **Modelagem** - RandomForest com validação cruzada
5. **Otimização** - Ajuste de hiperparâmetros e ensemble
6. **Validação** - Testes rigorosos com múltiplas estratégias



## Como Executar

1. **Instalar dependências:**
   ```bash
   pip install -r requirements.txt
   ```

2. **Executar notebook principal:**
   ```bash
   jupyter notebook kaggleMariana.ipynb
   ```

3. **Submissão no Kaggle:**
   - Usar `submission_final.csv` para melhor resultado
   - Acurácia esperada: 78.26%


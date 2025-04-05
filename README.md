# 🌸 Classificação de Espécies com o Dataset Iris

Este projeto tem como objetivo aplicar conceitos de algoritmos, lógica de programação e ciência de dados utilizando o clássico dataset **Iris**, muito conhecido em estudos de Machine Learning supervisionado.

## 📌 Objetivos

- Aplicar o modelo Gaussian Naive Bayes para classificação de espécies de flores.
- Explorar a relação entre variáveis preditoras do conjunto de dados.
- Avaliar a acurácia do modelo mesmo diante de variáveis correlacionadas.
- Discutir conceitos fundamentais de lógica de programação no contexto prático da ciência de dados.

## 🛠️ Tecnologias e Bibliotecas Utilizadas

- Python 3.x  
- pandas  
- numpy  
- seaborn  
- matplotlib  
- scikit-learn  

## ⚙️ Funcionalidades

- Leitura e análise exploratória do dataset Iris.
- Visualização estatística dos dados com gráficos.
- Treinamento do modelo GaussianNB.
- Teste com amostras personalizadas.
- Discussão sobre independência de variáveis e distribuição normal.

## 🧪 Exemplo de Uso

```python
from sklearn.datasets import load_iris
from sklearn.naive_bayes import GaussianNB

# Carregar dados
iris = load_iris()
X = iris.data
y = iris.target

# Treinar modelo
modelo = GaussianNB()
modelo.fit(X, y)

# Testar com uma nova flor
nova_flor = [[5.1, 3.5, 1.4, 0.2]]
predicao = modelo.predict(nova_flor)
print("Classe prevista:", predicao)
```

## 📚 Reflexões
Apesar das variáveis do dataset apresentarem interdependência, o modelo Gaussian Naive Bayes alcançou alta acurácia. Isso evidencia que, mesmo quando a suposição de independência não é plenamente atendida, a eficácia do modelo pode se manter se os dados forem bem distribuídos entre as classes.

## 🤝 Contribuições
Contribuições são bem-vindas! Fique à vontade para abrir uma issue ou pull request com melhorias, correções ou sugestões.

Desenvolvido por: Fernando Lima Filho


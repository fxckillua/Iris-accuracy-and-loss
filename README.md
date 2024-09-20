# Iris: Acurácia e Perda - Implementação de Rede Neural

Este projeto é uma implementação de uma **rede neural** em C, treinada com base no **conjunto de dados Iris**, utilizando o algoritmo de retropropagação para classificar as amostras em três espécies diferentes de flores. A rede calcula a acurácia e a perda do modelo durante as fases de treinamento e teste.

## Funcionalidades

- **Conjunto de dados:** O arquivo `iris_nr.txt` contém o conjunto de dados Iris com quatro características de entrada por amostra (como comprimento da sépala e largura da pétala) e três valores de destino correspondentes às possíveis espécies de flores.
- **Estrutura da Rede:**
  - **Camada de entrada:** 5 neurônios (4 características de entrada + 1 bias)
  - **Camada oculta:** 3 neurônios
  - **Camada de saída:** 3 neurônios (um para cada espécie de flor)
- **Algoritmo de Retropropagação:** A rede ajusta os pesos durante o treinamento usando o gradiente descendente, otimizando a saída ao minimizar o erro entre os valores previstos e os reais.
- **Processo de Treinamento:** 
  - Inicialização aleatória dos pesos.
  - Propagação dos dados pela rede.
  - Cálculo do erro utilizando a diferença quadrática.
  - Ajuste dos pesos via retropropagação.
- **Métricas de Desempenho:**
  - **Acurácia:** Calculada como a proporção de previsões corretas.
  - **Perda (Loss):** Medida utilizando a função de perda logarítmica.

## Arquivos

- `iris_nr.txt`: Contém o conjunto de dados Iris com valores randomizados usados para o treinamento.
- `iris.names`: Descreve as características e a estrutura do conjunto de dados Iris.
- `iris.data`: Conjunto de dados Iris bruto.
- `Iris.csv`: Arquivo CSV com o conjunto de dados original.

## Exemplo de Saída

- Durante o treinamento, os valores de acurácia e perda são exibidos, e ao final, os pesos ajustados da rede neural são impressos.

```bash
ACERTOS : 0.93
LOSS : 0.252
LOSS MEDIDO : 0.00168

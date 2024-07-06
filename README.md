# Reconhecimento de Expressões Faciais
Este projeto utiliza TensorFlow para construir e treinar um modelo de aprendizado profundo para reconhecimento de expressões faciais. O conjunto de dados utilizado é o FER_2013, contendo imagens faciais categorizadas em sete emoções: medo, raiva, desgosto, felicidade, neutro, tristeza e surpresa.

## Estrutura do Projeto

O projeto está estruturado da seguinte forma:

- **Manipulação de Dados:** Utiliza pandas para carregar e processar dados, e inclui visualização usando matplotlib e seaborn.
- **Arquitetura do Modelo:** Implementa uma arquitetura CNN personalizada usando a API Keras do TensorFlow, incorporando técnicas como Convolução Separável em Profundidade e Blocos de Residual Invertido.
- **Treinamento:** Treina o modelo usando a função `fit` do TensorFlow com técnicas de aumento de dados como rotação, deslocamento, espelhamento e zoom.
- **Avaliação:** Avalia o desempenho do modelo usando métricas de precisão e gera um relatório de classificação e matriz de confusão.
- **Visualização:** Visualiza a distribuição de dados, imagens de exemplo, progresso do treinamento e matrizes de confusão usando matplotlib e seaborn.

## Como Começar

### Pré-requisitos

- Python 3.x
- TensorFlow
- Pandas
- NumPy
- Matplotlib
- Seaborn
- PIL (Python Imaging Library)
- Google Colab (para montagem do Google Drive)


### Conjunto de Dados

- O conjunto de dados `FER_2013` está disponível no Kaggle. Você pode baixá-lo [aqui](https://www.kaggle.com/datasets/msambare/fer2013).

- Certifique-se de que o conjunto de dados está corretamente baixado e acessível em seu ambiente. O caminho para os dados pode precisar ser ajustado dependendo do seu sistema de arquivos.

## Downloads

- [Conjunto de Dados Pré-processado (FER_2013)](https://drive.google.com/file/d/1BAPtXM3Inac5GgoYGQuUdz58u-oY3_MI/view?usp=drive_link)
  - Arquivo contendo pixels das imagens, labels e informações de treino/teste.
### Treinamento

1. Execute o notebook `train_model.ipynb` no Google Colab ou qualquer ambiente Python com suporte ao TensorFlow.

2. Ajuste hiperparâmetros como tamanho do lote, número de épocas e taxa de aprendizado com base na experimentação.

### Avaliação

1. Após o treinamento, avalie o modelo usando o notebook `evaluate_model.ipynb` ou qualquer script Python.

2. Visualize as métricas de desempenho do modelo, como precisão, perda, relatório de classificação e matriz de confusão.

## Resultados

- Precisão alcançada: 69.36% após 100 épocas com tamanho do lote de 16.

### Saída de Exemplo

- ![Distribuição de Imagens](![Captura de tela 2024-07-03 155641](https://github.com/Thiago1alberto/Reconhecimento-de-emocoes-faciais/assets/71457360/067a2523-7ccd-48f8-bde8-ca709606c8b9)


## Licença

Este projeto está licenciado sob a Licença MIT - consulte o arquivo [LICENSE](LICENSE) para obter mais detalhes.

# Transfer Learning e Fine-Tuning com Keras

## Descrição

Este projeto é um tutorial em Python para demonstrar como utilizar **transfer learning** e **fine-tuning** para treinar classificadores de imagens de forma eficiente, mesmo com um número reduzido de amostras de treinamento. O tutorial utiliza o modelo **VGG16**, pré-treinado no dataset **ImageNet**, para extrair características ou ajustar pesos para uma nova tarefa de classificação de imagens.

A abordagem inclui a construção de um modelo a partir do zero como baseline, permitindo a comparação com os resultados obtidos por transferência de aprendizado.

---

## Conteúdo do Notebook

1. **Introdução ao Transfer Learning**
   - Explicação do conceito.
   - Diferença entre extração de características e fine-tuning.

2. **Carregamento do Dataset**
   - Uso do dataset **CalTech-101**.
   - Organização e preparação dos dados (divisão em `train`, `val` e `test`).

3. **Pré-processamento de Dados**
   - Normalização e formatação das imagens.
   - Conversão de rótulos para formato one-hot.

4. **Baseline: Modelo Construído do Zero**
   - Rede neural convolucional simples com:
     - 4 camadas convolucionais.
     - Camadas de pooling e dropout.
     - Classificador softmax.

5. **Transfer Learning com VGG16**
   - Extração de características.
   - Substituição da camada final do VGG16 por uma nova camada personalizada.
   - Congelamento de pesos das camadas iniciais.
   - Fine-tuning das camadas finais.

6. **Comparação de Resultados**
   - Avaliação de desempenho entre o modelo baseline e o modelo com transferência de aprendizado.

---

## Requisitos

- **Bibliotecas**: 
  - Keras
  - TensorFlow
  - NumPy
  - Matplotlib
  - Pillow

- **Ferramentas**:
  - Google Colab (ou um ambiente com suporte a notebooks Jupyter).

---

## Como Executar

1. **Clone ou Baixe o Projeto**  
   Certifique-se de ter o arquivo `transfer-learning.ipynb`.

2. **Abra o Notebook**  
   Execute o notebook em um ambiente como o [Google Colab](https://colab.research.google.com/).

3. **Execute as Células**  
   Siga as instruções do notebook para processar os dados, treinar os modelos e avaliar os resultados.

---

Este tutorial foi desenvolvido para ser um ponto de partida em transfer learning, permitindo ajustes e personalizações conforme necessário.

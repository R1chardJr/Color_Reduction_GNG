# 🎨 Redução de Cores em Imagens com Growing Neural Gas (GNG)

Este projeto aplica a rede neural não supervisionada **Growing Neural Gas (GNG)** para realizar **redução de cores em imagens**, de forma adaptativa e inteligente. O objetivo é compactar imagens coloridas, preservando suas principais características visuais com um número reduzido de cores — ideal para compressão, visualização simplificada ou processamento em dispositivos com recursos limitados.

---

## 📌 Motivação

Em um cenário atual dominado por **grandes volumes de dados visuais** e pela necessidade de executar tarefas de visão computacional em **dispositivos com hardware limitado**, a redução de complexidade se torna fundamental.

A GNG se destaca por:
- Aprender a **estrutura dos dados de forma incremental**;
- Adaptar sua topologia ao longo do tempo;
- Ser mais flexível que métodos tradicionais como K-Means, por não exigir o número fixo de clusters inicialmente.

---

## ⚙️ Funcionalidades

- Leitura de imagens a partir de URLs públicas
- Treinamento de uma rede GNG para representar as cores principais da imagem
- Reconstrução da imagem com paleta reduzida
- Variação de hiperparâmetros como:
  - `max_nodes` (neurônios máximos)
  - `lambda_insert` (frequência de inserção de neurônios)
  - Taxas de aprendizado (`eps_b`, `eps_n`)
- Cálculo de métricas como:
  - Número de cores únicas
  - Inércia média (distância média dos pixels aos neurônios)
  - Detecção de outliers (pixels mal representados)
- Visualização:
  - Imagens antes e depois
  - Paleta de cores aprendida
  - Projeção PCA dos neurônios e pixels no espaço RGB

---


## 🧠 Tecnologias utilizadas

- Python 3.x
- NumPy
- Matplotlib
- OpenCV
- Scikit-learn (PCA e métricas)

---

## 📁 Como executar

1. Clone o repositório ou abra o notebook no Google Colab:
   ```
   git clone https://github.com/seu_usuario/GNG_Images_Reduced.git
   ```

2. Execute o notebook `GNG_Images_reduced.ipynb`

3. Altere os parâmetros conforme desejado para explorar diferentes resultados.

---

## 📚 Referências

- Fritzke, B. (1995). *A Growing Neural Gas Network Learns Topologies*. NIPS.
- Quiles, M. G. — Material de apoio e formalização do algoritmo GNG.
- Kohonen, T. (2001). *Self-Organizing Maps*, Springer.

---

## 📌 Autor

Projeto criado por **Richard Jr**  

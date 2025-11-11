# 🌌 Galaxy10 – Classificação de Galáxias com LeNet-5

Este projeto realiza a **classificação de galáxias** do dataset **Galaxy10 DECals**, utilizando a **rede neural LeNet-5**.  
O objetivo é comparar o desempenho da rede ao aplicar diferentes métodos de **conversão para escala de cinza** nas imagens.

---

## 🧠 Sobre o Projeto

O dataset **Galaxy10 DECals** contém imagens coloridas de diferentes tipos de galáxias.  
Neste experimento, são utilizadas duas classes:

- **Classe 0:** Round Smooth (Classe 2)  
- **Classe 1:** Barred Spiral (Classe 5)

O modelo é treinado separadamente com quatro métodos de conversão para tons de cinza:

1. **Intensity** – média simples dos canais RGB  
2. **Luminance** – ponderação clássica dos canais RGB  
3. **Gleam** – média com correção gamma  
4. **Luma** – ponderação com correção gamma  

O objetivo é observar como cada método de conversão afeta a capacidade da **LeNet-5** em classificar as galáxias corretamente.

---

## ⚙️ Como Executar o Projeto

### 1️⃣ Abrir o notebook

Abra o arquivo **`galaxy10_gray_lenet5.ipynb`** no **[Google Colab](https://colab.research.google.com/)**  
ou em seu ambiente local (Jupyter Notebook, VS Code, etc.).

---

### 2️⃣ Instalar as dependências

Execute a célula abaixo no início do notebook:

```bash
!pip install astroNN tensorflow scikit-learn seaborn matplotlib plotly

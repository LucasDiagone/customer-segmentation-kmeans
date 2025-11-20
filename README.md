# 📊 Estudo de Caso Aplicado: Análise de Cluster (MBA USP/Esalq)

Este projeto faz parte das práticas aplicadas do **MBA em Ciência de Dados da USP/Esalq**.  
O objetivo é realizar uma **segmentação de clientes** utilizando técnicas de clusterização não supervisionada.

---

## 🎯 Objetivos do Projeto

Aplicar métodos de agrupamento para identificar padrões e segmentos distintos em um conjunto de clientes, utilizando:

- **K-Means**
- **Cluster Hierárquico** (com dendrograma)
- **Padronização Z-Score**
- **ANOVA** para validação estatística
- **Métodos para definição da quantidade ideal de clusters**

---

## 🔍 Definição da Quantidade Ideal de Clusters

Foram utilizados dois métodos complementares:

### **1. Método do Cotovelo (Elbow Method)**
- Analisa a redução da inércia (WCSS).
- O ponto de “cotovelo” indicou que **k = 4 clusters** seria uma boa escolha.

### **2. Dendrograma do Cluster Hierárquico**
- Permite visualizar as distâncias entre observações e como os grupos se formam.
- O corte visual sugeriu **aproximadamente 4 divisões naturais** nos dados.

---

## ✅ Conclusão

Ambos os métodos convergiram para **4 clusters**, reforçando a consistência da escolha.

---

## 📈 Validação Estatística com ANOVA

Para verificar se os clusters apresentam diferenças estatísticas relevantes, foi aplicado o **teste ANOVA de uma via**.

### 📋 Termos da Tabela ANOVA (simplificados)

- **Between Groups:** variância entre os clusters  
- **Within Groups:** variância dentro dos clusters  
- **F:** razão entre variância entre grupos e variância interna  
- **p-valor:** indica se as diferenças são estatisticamente significativas  

### 🧠 Interpretação

Se **p-valor < 0.05**, concluímos que os clusters são significativamente diferentes, validando a eficiência da segmentação.

---

## 🗂️ Fonte da Base de Dados

A base utilizada é o **Mall Customers Dataset**, disponível publicamente no Kaggle:

🔗 https://www.kaggle.com/datasets/shwetabh123/mall-customers

---

## 📁 Estrutura do Projeto

```
📦 analise-cluster
 ┣ 📂 data
 ┣ 📂 src
 ┃ ┣ 📜 clusterizacao.ipynb
 ┃ ┣ 📜 anova_validacao.ipynb
 ┣ 📜 README.md
```

---

## 👨‍💻 Autor

**Lucas Diagone**  
🔗 https://www.linkedin.com/in/lucas-diagone-691285104/

# 📊 Estudo de Caso Aplicado: Análise de Cluster (MBA USP/Esalq)

Este projeto faz parte das práticas aplicadas do **MBA em Ciência de Dados da USP/Esalq**.  
O objetivo é realizar uma **segmentação de clientes** utilizando técnicas de clusterização não supervisionada.

---

## 🎯 Objetivos do Projeto

Aplicar métodos de agrupamento para identificar padrões e segmentos distintos em um conjunto de clientes, utilizando:

- **K-Means**
- **Cluster Hierárquico** (com dendrograma)
- **Padronização Z-Score**
- **Heatmap de Correlação**
- **Método do Cotovelo (Elbow)**
- **Método Silhouette**
- **ANOVA** para validação estatística
- **Métodos para definição da quantidade ideal de clusters**

---

## 📈 Análise Exploratória – Correlação

Antes da clusterização, foi gerada uma **matriz de correlação** acompanhada de um **heatmap**, permitindo identificar relações entre variáveis, padrões ocultos e possíveis redundâncias importantes para o agrupamento.

---

## 🔍 Definição da Quantidade Ideal de Clusters

Foram utilizados métodos complementares:

### **1. Método do Cotovelo (Elbow Method)**
- Analisa a redução da inércia (WCSS).
- O ponto de “cotovelo” indicou que **k = 4** seria uma boa escolha.

### **2. Método Silhouette**
- Mede o quão bem cada observação está associada ao seu cluster.
- O maior valor de Silhouette também apontou para **k = 4**, reforçando a consistência da escolha.

### **3. Dendrograma do Cluster Hierárquico**
- Permite visualizar a formação dos grupos e as distâncias entre eles.
- O corte visual sugeriu **aproximadamente 4 divisões naturais**.

---

## ✅ Conclusão

Os métodos **Cotovelo**, **Silhouette** e **Hierárquico** convergiram para a mesma solução:  
**4 clusters** é a segmentação mais consistente para este conjunto de dados.

---

## 📈 Validação Estatística com ANOVA

Para verificar se os clusters apresentam diferenças estatísticas relevantes, foi aplicado o **teste ANOVA de uma via** para cada variável.

### 📋 Termos da Tabela ANOVA (simplificados)

- **Between Groups:** variância entre os clusters  
- **Within Groups:** variância dentro dos clusters  
- **F:** razão entre variância entre grupos e variância interna  
- **p-valor:** indica se as diferenças são estatisticamente significativas  

### 🧠 Interpretação

Se **p-valor < 0.05**, concluímos que os clusters são significativamente diferentes, validando a qualidade da segmentação.

---

## 🗂️ Fonte da Base de Dados

A base utilizada é o **Mall Customers Dataset**, disponível publicamente no Kaggle:

🔗 https://www.kaggle.com/datasets/shwetabh123/mall-customers

---

## 👨‍💻 Autor

**Lucas Diagone**  
🔗 https://www.linkedin.com/in/lucas-diagone-691285104/

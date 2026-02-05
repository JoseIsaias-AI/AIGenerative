# 🧠 AIGenerative — GAN para Geração de Números Manuscritos

Este repositório apresenta a implementação de uma **Generative Adversarial Network (GAN)** desenvolvida com **TensorFlow e Keras**, treinada sobre o dataset **MNIST** com o objetivo de gerar imagens realistas de números manuscritos.

O projeto tem foco **educacional e experimental**, explorando conceitos fundamentais de **Deep Learning Generativo** e **Visão Computacional**.

---

## 🚀 Visão Geral

Uma GAN é composta por duas redes neurais que competem entre si:

* **Gerador**: cria imagens artificiais a partir de ruído aleatório.
* **Discriminador**: avalia se uma imagem é real (dataset) ou falsa (gerada).

Durante o treinamento, o gerador aprende a produzir imagens cada vez mais realistas, enquanto o discriminador tenta não ser enganado. Esse processo adversarial permite que padrões complexos sejam aprendidos **sem supervisão direta**.

---

## 🏗️ Arquitetura do Modelo

### 🔹 Gerador

* Entrada: vetor de ruído aleatório (100 dimensões)
* Camadas densas + reshape
* Camadas **Conv2DTranspose** para upsampling
* **Batch Normalization** e **LeakyReLU**
* Saída: imagem 28×28 em escala de cinza (`tanh`)

### 🔹 Discriminador

* Entrada: imagem 28×28
* Camadas **Conv2D** com strides
* **LeakyReLU** e **Dropout**
* Saída: valor escalar indicando real ou falso

---

## 📊 Resultados

Durante os experimentos, o modelo apresentou melhor desempenho na geração de alguns dígitos específicos, com destaque para o **número 4**, que se tornou visualmente mais consistente ao longo do treinamento.

Esses resultados demonstram como GANs conseguem capturar padrões estruturais presentes em dados visuais simples.

---

## 🛠️ Tecnologias Utilizadas

* Python
* TensorFlow / Keras
* NumPy
* Matplotlib
* Jupyter Notebook

---

## 📂 Estrutura do Repositório

```text
AIGenerative/
├── generative.ipynb   # Notebook com a implementação da GAN
├── README.md          # Documentação do projeto
```

---

## 🎯 Objetivo do Projeto

Este projeto foi desenvolvido com o objetivo de:

* Consolidar conhecimentos em **Redes Neurais Convolucionais**
* Explorar **Modelos Generativos**
* Entender o funcionamento prático de **GANs**
* Servir como material de estudo e portfólio em IA

---

## 📌 Próximos Passos

* Salvamento de imagens geradas por época
* Avaliação visual comparativa
* Extensão para outros datasets
* Integração com aplicações educacionais

---

## 👤 Autor

**José Isaias**
Estudante e desenvolvedor em Inteligência Artificial e Machine Learning

🔗 GitHub: [https://github.com/JoseIsaias-AI](https://github.com/JoseIsaias-AI)

---

⭐ Se este projeto foi útil, considere deixar uma estrela no repositório!

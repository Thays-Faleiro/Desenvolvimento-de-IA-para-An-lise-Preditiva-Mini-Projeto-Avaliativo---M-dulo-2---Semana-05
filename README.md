# Classificação Multiclasse MNIST & Análise de Generalização Extrema (OOD)

> **Mini-Projeto Avaliativo - Módulo 2**  
> **Curso:** Desenvolvimento de IA para Análise Preditiva  
> **Instituição:** Senai/SC (SCTEC)  
> **Autora:** Thays Faleiro  

---

---

##  Apresentação em Vídeo
- 🔗 **Link do Vídeo Demonstrativo (Google Drive):** [COLE_AQUI_O_LINK_DO_SEU_VIDEO_NO_GOOGLE_DRIVE]

---

##  Visão Geral do Projeto
Este projeto implementa um pipeline completo de Machine Learning e Deep Learning em Python para a classificação de dígitos manuscritos ($28 \times 28$ pixels em escala de cinza) utilizando o dataset benchmark **MNIST**.

O objetivo principal consiste em comparar algoritmos de aprendizado estatístico clássico com redes neurais artificiais, avaliando métricas globais e por classe (Acurácia, Precisão, Recall e F1-Score), custo computacional de treinamento e o comportamento dos modelos sob entradas fora da distribuição (**Out-of-Distribution - OOD**), além de inferência em imagem real capturada manualmente.

---

##  Tecnologias e Bibliotecas Utilizadas
- **Linguagem:** Python 3.10+
- **Processamento de Dados:** NumPy, Pandas
- **Visualização de Dados:** Matplotlib, Seaborn
- **Visão Computacional:** OpenCV (`cv2`)
- **Machine Learning Clássico:** Scikit-Learn (`RandomForestClassifier`, `SVC`)
- **Deep Learning:** TensorFlow / Keras (`Sequential`, `Dense`, `Dropout`)

---

##  Estrutura do Repositório
```text
.
├── notebook_mnist.ipynb       # Notebook principal com EDA, Treinamento e Teste OOD
├── Mini_Projeto_Módulo_2.ipynb # Código complementar do projeto
├── requirements.txt           # Dependências e bibliotecas do projeto
└── README.md                  # Documentação detalhada

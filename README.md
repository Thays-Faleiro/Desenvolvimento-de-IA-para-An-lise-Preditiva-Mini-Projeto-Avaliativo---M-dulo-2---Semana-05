# Classificação multiclasse MNIST & análise de generalização extrema (OOD)

**Mini-projeto avaliativo - Módulo 2**  
**Curso:** Desenvolvimento de IA para Análise Preditiva  
**Instituição:** Senai/SC (SCTEC)  
**Autora:** Thays Faleiro  

---

## Apresentação em vídeo

🔗 **Link do vídeo demonstrativo (Google Drive):** [COLE_AQUI_O_LINK_DO_SEU_VIDEO_NO_GOOGLE_DRIVE]

---

## Visão geral do projeto

Este projeto implementa um pipeline completo de Machine Learning e Deep Learning em Python para a classificação de dígitos manuscritos ($28 \times 28$ pixels em escala de cinza) utilizando o dataset benchmark **MNIST**.

O objetivo principal consiste em comparar algoritmos de aprendizado estatístico clássico com redes neurais artificiais, avaliando métricas globais e por classe (Acurácia, Precisão, Recall e F1-Score), custo computacional de treinamento e o comportamento dos modelos sob entradas fora da distribuição (**Out-of-Distribution - OOD**), além da inferência em imagens reais capturadas manualmente via OpenCV.

---

## Tecnologias e bibliotecas utilizadas

- **Linguagem:** Python 3.10+
- **Processamento de Dados:** NumPy, Pandas
- **Visualização de Dados:** Matplotlib, Seaborn
- **Visão Computacional:** OpenCV (`cv2`)
- **Machine Learning Clássico:** Scikit-Learn (`RandomForestClassifier`, `SVC`)
- **Deep Learning:** TensorFlow / Keras (`Sequential`, `Dense`, `Dropout`)

---

## Estrutura do repositório

```text
.
├── data/
│   └── minhas_imagens/        # Imagens de dígitos manuscritos para o Desafio C
├── notebook_mnist.ipynb       # Notebook principal com EDA, Treinamento, OOD e Inferência
├── requirements.txt           # Dependências e bibliotecas do projeto
└── README.md                  # Documentação detalhada do projeto


git clone [https://github.com/SEU_USUARIO/SEU_REPOSITORIO.git](https://github.com/SEU_USUARIO/SEU_REPOSITORIO.git)
cd SEU_REPOSITORIO




git clone [https://github.com/SEU_USUARIO/SEU_REPOSITORIO.git](https://github.com/SEU_USUARIO/SEU_REPOSITORIO.git)
cd SEU_REPOSITORIO


python -m venv venv
# No Windows:
.\venv\Scripts\activate
# No Linux/Mac:
source venv/bin/activate

pip install -r requirements.txt

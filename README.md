# Classificação Multiclasse MNIST e Análise de Generalização Extrema (OOD)

> **Mini-Projeto Avaliativo — Módulo 2**  
> **Curso:** Desenvolvimento de IA para Análise Preditiva  
> **Instituição:** SENAI/SC (SCTEC)  
> **Autora:** Thays Faleiro  

---

## Apresentação em Vídeo

- Link do Vídeo Demonstrativo (Google Drive): [(https://drive.google.com/file/d/1jEGlMcka_hLpc2Ik83qnyiVi1qjvvoXl/view?usp=sharing)]

---

## Visão Geral do Projeto

Este projeto implementa um pipeline end-to-end de Machine Learning e Deep Learning em Python para a classificação de dígitos manuscritos (28 x 28 pixels em escala de cinza) utilizando o dataset benchmark MNIST.

O objetivo principal consiste em comparar algoritmos de aprendizado estatístico clássico com redes neurais artificiais, avaliando métricas globais e por classe (Acurácia, Precisão, Recall e F1-Score), custo computacional de treinamento e o comportamento dos modelos sob entradas fora da distribuição (Out-of-Distribution - OOD), além da inferência em imagens reais capturadas manualmente e tratadas via OpenCV.

---

## Tecnologias e Bibliotecas Utilizadas

- **Linguagem:** Python 3.10+
- **Processamento de Dados:** NumPy, Pandas
- **Visualização de Dados:** Matplotlib, Seaborn
- **Visão Computacional:** OpenCV (`cv2`)
- **Machine Learning Clássico:** Scikit-Learn (`RandomForestClassifier`, `SVC`)
- **Deep Learning:** TensorFlow / Keras (`Sequential`, `Dense`, `Dropout`)

---

## Tabela Comparativa de Desempenho

| Modelo | Algoritmo / Arquitetura | Acurácia | Precisão (Macro) | Recall (Macro) | F1-Score (Macro) | Tempo de Treino (s) |
|---|---|:---:|:---:|:---:|:---:|:---:|
| **Random Forest** | `RandomForestClassifier(n_estimators=100)` | ~96.8% | ~96.8% | ~96.8% | ~96.8% | ~15s |
| **SVM (RBF)** | `SVC(kernel='rbf', C=10)` | ~98.2% | ~98.2% | ~98.2% | ~98.2% | ~210s |
| **Rede Neural (MLP)** | `Keras Sequential (Dense + Dropout)` | ~98.0% | ~98.0% | ~98.0% | ~98.0% | ~25s |

---

## Principais Conclusões Técnicas

1. **Eficiência Computacional vs. Desempenho:**
   - O SVM obteve a maior acurácia absoluta (~98.2%), porém apresentou o maior tempo de treinamento.
   - A MLP (Keras) obteve desempenho equivalente (~98.0%), com tempo de treino drasticamente menor, mostrando-se superior para cenários de produção.
2. **Avaliação Out-of-Distribution (OOD):**
   - Ao ocultar certas classes durante o treino (como os dígitos 4 e 7), o modelo tendeu a classificar essas novas entradas em classes conhecidas com alto nível de incerteza/confiança excessiva, demonstrando a necessidade de limiares de rejeição em sistemas reais.
3. **Inferência em Imagem Real:**
   - O pré-processamento com OpenCV (conversão para escala de cinza, inversão de contraste e redimensionamento 28x28) garantiu a correta predição da foto do dígito manuscrito.

---

## Estrutura do Repositório

```text
.
├── data/
│   └── minhas_imagens/        # Imagens de dígitos manuscritos para o teste de inferência
├── notebook_mnist.ipynb       # Notebook principal (EDA, Treinamento, OOD e Inferência)
├── requirements.txt           # Dependências e bibliotecas do projeto
└── README.md                  # Documentação detalhada do projeto


git clone [https://github.com/Thays-Faleiro/Desenvolvimento-de-IA-para-An-lise-Preditiva-Mini-Projeto-Avaliativo---M-dulo-2---Semana-05.git](https://github.com/Thays-Faleiro/Desenvolvimento-de-IA-para-An-lise-Preditiva-Mini-Projeto-Avaliativo---M-dulo-2---Semana-05.git)
cd Desenvolvimento-de-IA-para-An-lise-Preditiva-Mini-Projeto-Avaliativo---M-dulo-2---Semana-05



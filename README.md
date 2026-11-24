Esteira de Aprendizado de Máquina — Coluna Vertebral
Descrição
Este projeto implementa uma esteira de aprendizado de máquina para classificação binária de pacientes como Normal ou Abnormal, utilizando a base Vertebral Column do UCI Machine Learning Repository.

A adaptação atende às etapas solicitadas no trabalho: estatísticas descritivas, transformação de linhas e colunas, divisão em treinamento/validação/teste, treinamento, avaliação e predição. 
O código usa execução local com scikit-learn, sem depender de AWS SageMaker, S3 ou credenciais de nuvem.

Base de dados
Nome: Vertebral Column Data Set.
Origem: UCI Machine Learning Repository.
Link: https://archive.ics.uci.edu/dataset/212/vertebral+column
Atributos: seis características biomecânicas.
Classes: Normal (0) e Abnormal (1).

Etapas do notebook
Importação das bibliotecas e carregamento da base.
Estatísticas descritivas e distribuição das classes.
Remoção de duplicatas e de linhas com valores ausentes.
Padronização das características numéricas com StandardScaler dentro de um Pipeline.
Divisão estratificada em 60% treinamento, 20% validação e 20% teste.
Treinamento de Random Forest.
Avaliação de validação e conversão de probabilidades usando threshold.
Avaliação no conjunto de teste, matriz de confusão e acurácia.
Métricas: sensibilidade, especificidade, precisão, NPV, FPR, FNR e FDR.
Curva ROC/AUC e comparação de thresholds.
Predição de uma amostra do conjunto de teste.
Como executar
Requisitos
Python 3.10 ou superior e conexão com a internet para baixar a base UCI na primeira execução.

1. Baixar/clonar o repositório
git clone URL_DO_SEU_REPOSITORIO
cd esteira-machine-learning
2. (Recomendado) Criar ambiente virtual
Windows:

python -m venv .venv
.venv\Scripts\activate
Linux/macOS:

python3 -m venv .venv
source .venv/bin/activate
3. Instalar dependências
pip install -r requirements.txt
4. Abrir o Jupyter
jupyter notebook
Abra notebook.ipynb e execute Kernel > Restart & Run All, do início ao fim.



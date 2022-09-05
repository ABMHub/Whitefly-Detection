# Whitefly Detection

Esse repositório diz respeito ao segundo trabalho da disciplina Fundamentos de Sistemas Inteligentes, ministrada na UnB (Universidade de Brasília), no semestre 2022.1.

- Aluno: Lucas de Almeida Bandeira Macedo
- Matrícula: 19/0047089

Link do repositório do projeto: [ABMHub/Whitefly-Detection](https://github.com/ABMHub/Whitefly-Detection)

## Setup

O arquivo [main](main.ipynb) faz todas as preparações que são necessárias, mas existem duas pastas que devem ser colocadas no lugar certo:

1. darknet
2. data

### Darknet

O repositório [AlexeyAB/darknet](https://github.com/AlexeyAB/darknet) está importado apenas como sub-módulo, portanto, é necessário seu git clone.

Caso você não tenha clonado o repositório ainda, rode o seguinte comendo:

```git
git clone --recurse-submodules https://github.com/chaconinc/MainProject
```

Caso você já tenha feito o clone, e não o fez recursivamente, rode estes comandos, na pasta do projeto

```git
git submodule init
git submodule update
```

Os comandos acima garantirão que a pasta do darknet seja importada do github junto com o projeto, no caminho correto.

### Data

A pasta de dados foi omitida do repositório para evitar que fique muito pesado.

Baixe o dataset do seguinte link: [Cassava Whitefly Dataset](https://data.mendeley.com/datasets/5g38399z9p/2);
e descompacte-o de modo que a path a seguir fique válida:

- `Whitefly-Detection/data/super_abundance/`

## Google Colab

Embora o projeto tenha sido feita em um ambiente local, ele é completamente compatível com o Google Colab. 

Para fazer funcionar, basta colocar a pasta inteira do projeto, com a pasta `data` e `darknet` dentro, assim como descrito na seção `Setup`

A única mudança será a necessidade de descomentar as linhas de código indicadas na primeira célula, assim como modificar a path indicada caso necessário.

## Análise de Resultados

A análise de resultados foi feita ao longo do notebook.

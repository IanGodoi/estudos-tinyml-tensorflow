# Estudos de TinyML com TensorFlow

Esse repositório reúne alguns exercícios e testes que venho fazendo enquanto estudo **TinyML**, **TensorFlow** e **TensorFlow Lite**.

A ideia é usar esse espaço para organizar meu aprendizado e ir acompanhando minha evolução, principalmente na parte de Machine Learning voltado para dispositivos com poucos recursos, como microcontroladores.

## O que tem aqui

Até agora, os estudos envolvem coisas como:

- classificação de imagens;
- uso de modelos pré-treinados;
- Transfer Learning;
- MobileNetV2;
- preparação de datasets;
- treinamento e validação de modelos;
- exportação de modelos;
- conversão para TensorFlow Lite;
- keyword spotting;
- primeiros passos pensando em aplicações embarcadas.

## Tecnologias que estou usando

- Python
- TensorFlow
- TensorFlow Lite
- TensorFlow Hub
- TensorFlow Datasets
- NumPy
- Matplotlib
- Jupyter Notebook

## Alguns exercícios

Um dos exercícios que fiz foi de classificação de imagens usando o dataset de **pedra, papel e tesoura**.

Nesse caso, trabalhei com imagens redimensionadas e usei **MobileNetV2** como base para fazer Transfer Learning.

A ideia, de forma simplificada, foi:

```text
imagem
  ↓
pré-processamento
  ↓
MobileNetV2
  ↓
extração de características
  ↓
classificação
```

Também fiz testes com exportação de modelos e conversão para o formato `.tflite`.

## TensorFlow Lite

Uma parte que tenho estudado bastante é a conversão dos modelos treinados para **TensorFlow Lite**.

O fluxo que estou seguindo é mais ou menos:

```text
modelo treinado
      ↓
SavedModel
      ↓
conversão
      ↓
arquivo .tflite
```

No repositório também deixei alguns modelos gerados durante esses testes.

## Keyword Spotting

Também comecei a estudar **Keyword Spotting**, que é o reconhecimento de palavras curtas ou comandos de voz.

Esse tipo de aplicação me interessa bastante porque é um exemplo clássico de TinyML e pode ser levado para sistemas embarcados.

Exemplos de comandos desse tipo:

```text
yes
no
up
down
go
stop
```

## Notebooks

Os estudos estão organizados principalmente nestes notebooks:

```text
exercicio18.ipynb
exercicio19.ipynb
exercicio20.ipynb
keyword_spotting.ipynb
tiny.ipynb
```

Cada um corresponde a algum exercício, teste ou etapa diferente do aprendizado.

## Estrutura do repositório

```text
estudos-tinyml-tensorflow/
│
├── exercicio18.ipynb
├── exercicio19.ipynb
├── exercicio20.ipynb
├── keyword_spotting.ipynb
├── tiny.ipynb
│
├── model_from_savedmodel.tflite
├── model_from_savedmodel2.tflite
│
├── .gitignore
└── README.md
```

Não estou versionando ambientes virtuais, datasets muito grandes e alguns arquivos temporários para evitar deixar o repositório pesado.

## Próximos passos

Quero continuar avançando principalmente em:

- quantização;
- modelos INT8;
- TensorFlow Lite for Microcontrollers;
- uso de memória RAM e Flash;
- latência de inferência;
- classificação de áudio e sinais de sensores;
- execução de modelos em microcontroladores.

Meu objetivo é sair do modelo treinado no computador e chegar até a inferência rodando em hardware embarcado.

## Sobre este repositório

Esse não é um projeto fechado ou pronto.

É mais um repositório de estudos, onde vou colocando exercícios e testes conforme avanço em TinyML.

## Autor

Ian Godoi

Graduando em Ciência da Computação na UFMG.


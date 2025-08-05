# 💻 Similaridade de Imagens usando Vision Transformers no python

Útima Atualização: 05.08.2025

<div align="center">
<img src="https://img.shields.io/badge/Python-%233776AB.svg?&style=for-the-badge&logo=python&logoColor=white" alt="Python">
<img src="https://img.shields.io/badge/Machine%20Learning-%23FF6F00.svg?&style=for-the-badge&logo=google-colab&logoColor=white" alt="ML">
<img src="https://img.shields.io/badge/Deep%20Learning-%230075A8.svg?&style=for-the-badge&logo=tensorflow&logoColor=white" alt="DL">
</div>

Esse repositório contém a apresentação e códigos do tutorial "Similaridade de Imagens usando Vision Transformers no python" que foi apresentado no RBRAS 2025.

![](apresentacao/images/logo_capa.png)

## Sobre o tutorial:


Neste tutorial, será utilizado uma abordagem para a correspondência de imagens utilizando o Vision Transformer (ViT) (<https://arxiv.org/abs/2010.11929>). O objetivo é demonstrar uma técnica de deep learning para realizar correspondência de imagens, que se refere ao processo de identificar e emparelhar partes semelhantes ou correspondentes em duas ou mais imagens. No entanto, devido a variações significativas de iluminação, ângulo de captura e qualidade da imagem, esta tarefa se torna complexa, especialmente em cenários do mundo real, como o reconhecimento de objetos, animais ou pessoas em diferentes imagens.

A arquitetura ViT adapta o modelo Transformer - originalmente desenvolvido para tarefas de Processamento de Linguagem Natural (NLP) - para o processamento de dados de imagem. Ela utiliza embeddings, que são vetores que capturam a informação semântica de palavras, frases ou imagens, permitindo mapear dados semelhantes para pontos próximos em um espaço vetorial de alta dimensionalidade. Na correspondência de imagens, o desafio está em como representar as imagens de forma eficaz como embeddings, capturando características relevantes. Ao aplicar técnicas de pré-processamento, como a remoção de fundo, buscamos isolar o objeto de interesse, o que auxilia em tarefas como reconhecimento de objetos, segmentação de imagens e correspondência.

A partir dos embeddings, a similaridade entre diferentes imagens é calculada utilizando a similaridade do cosseno. A imagem de interesse é comparada a uma base de dados de imagens, e os resultados são retornados com um score de similaridade. O score de similaridade do cosseno quantifica a semelhança entre duas imagens em termos de suas características extraídas. Esta métrica varia de -1 a 1, onde, quanto mais próximo de 1, mais alinhados estão os vetores que representam as imagens, indicando que elas compartilham muitas características comuns. Um valor de 0 indica que os vetores de embeddings das imagens são ortogonais, o que significa que as imagens têm pouco em comum, e quanto mais próximo de -1, mais opostos são os vetores, significando que as imagens são muito diferentes.

Assim, este tutorial tem com objetivo abordar as etapas de pré-processamento de imagens, geração de embeddings usando Vision Transformers e cálculo de similaridade através da similaridade do cosseno. Ao final, os participantes entenderão como aplicar esses métodos tanto em contextos acadêmicos quanto práticos.

*Link do modelo no Hugging-Face:* https://huggingface.co/google/vit-base-patch16-224

*Palavras-chave:*
Vision Transformers, similaridade de imagens, deep learning, embeddings, visão computacional


## Estrutura do Repositório

```
similarity_vit_python/
 ├── apresentacao/
 │   └── index.html
 └── Codigo_ViT/
     ├── Pre_processamento_ViT_com_dados_imagens_digitais.ipynb
     └── ViT_com_dados_imagens_digitais_Match_Images.ipynb
```
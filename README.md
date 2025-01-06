# modern-architectures-of-neural-networks
introduction to modern neural network architectures

## 1. CAE (Conditional Autoencoder) - см. `conditional_autoencoder.ipynb`
Был модифицирован автоэнкодер и добавлен к нему слой-условие. В качестве датасета использовался fashionMNIST.

## 2. Исследование латентного пространства VAE (Variational Autoencoder). Исследование codebook VQ-VAE (Vector Quantized VAE) - см. `VAE_and_VQ-VAE.ipynb`
VAE и VQ-VAE были обучены на датасете fashionMNIST.

## 3. WGAN (Wasserstein Generative Adversarial Network) и WGAN-GP (WGAN with Gradient Penalty)- см. `WGAN_and_WGAN-GP.ipynb`
Были реализованы WGAN и его модификация WGAN-GP и обучены на датасете [пицц](https://www.kaggle.com/datasets/ounimed/pizza-dataset-ready-to-use-with-yolo). 
Основа генератора и дискриминатора была выбрана свёрточная.

## 4. ViT (Vision Transformer) - `ViT.ipynb`
Был реализован ViT **с нуля**. В качестве датасета использовался [следующий](https://www.kaggle.com/datasets/gpiosenka/headgear-image-classification).

## 5. Fine-tune LLM with LoRA - `LLM_with_LoRA.ipynb`
Была дообучена LLM на датасете [ Stanford Question Answering Dataset (SQuAD)](https://www.kaggle.com/datasets/stanfordu/stanford-question-answering-dataset/data) для задачи 
question answering с использованием LoRA.
Для этого составлялись пары "контекст + вопрос" - "ответ" и дообучалась `AutoModelForCausalLM` модель `distilgpt2`.

## 6. DiT (Diffusion Transformer) - `DiT.ipynb`
Был запущен DiT из diffusers и сгенерировано несколько изображений. Было произведено исследование того, как поменяется генерация при варьировании гиперпараметров генерации.
Также представлен краткий обзор [статьи](https://arxiv.org/pdf/2212.09748). 

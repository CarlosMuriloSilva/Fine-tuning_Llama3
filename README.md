# Fine-tuning do modelo LLaMA 3 com Unsloth

## Descrição

Este projeto demonstra como realizar o fine-tuning do modelo `unsloth/llama-3-8b-bnb-4bit` utilizando dados personalizados. O objetivo é adaptar o modelo para tarefas específicas, como classificação de títulos de produtos da Amazon.

## Estrutura do Projeto

- **`prepare-data.ipynb`**: Notebook para pré-processamento dos dados, preparando-os no formato necessário para o fine-tuning.
- **`finetuning_amazon_titles.ipynb`**: Notebook principal que realiza o fine-tuning do modelo utilizando os dados preparados.
- **`inferencia_llama3.ipynb`**: Notebook para realizar inferências utilizando o modelo LLaMA 3 original.
- **`inferencia_modelo_treinado.ipynb`**: Notebook para realizar inferências utilizando o modelo após o fine-tuning.
- **`.gitignore`**: Especifica arquivos e pastas a serem ignorados pelo Git.

## Pré-requisitos

- Python 3.8 ou superior
- Conta na Hugging Face com acesso ao modelo `unsloth/llama-3-8b-bnb-4bit`
- Chave de API da Hugging Face configurada como variável de ambiente `HUGGINGFACE_API_KEY`

## Este Projeto pode ser executado através do Google Colab ou clonado e executado localmente

## Executando no Google Colab

Você pode executar este projeto diretamente no Google Colab sem a necessidade de instalação local. Basta abrir o notebook desejado a partir do repositório e seguir as instruções.

**Passos:**

1. Acesse o notebook principal:
   [finetuning_amazon_titles.ipynb](https://colab.research.google.com/github/CarlosMuriloSilva/Fine-tuning_Llama3/blob/master/finetuning_amazon_titles.ipynb)

2. Certifique-se de ativar o ambiente com GPU:
   - Vá em `Ambiente de execução` > `Alterar tipo de ambiente` > selecione **GPU**.

## Instalação

**Passos:**

1. Clone o repositório:
   ```bash
   git clone https://github.com/CarlosMuriloSilva/Fine-tuning_Llama3.git
   cd Fine-tuning_Llama3
   ```

2. Crie um ambiente virtual e ative-o:
   ```bash
   python -m venv venv
   source venv/bin/activate  # No Windows: venv\Scripts\activate
   ```

3. Instale as dependências necessárias:
   ```bash
   pip install -r requirements.txt
   ```

   *Nota: Certifique-se de que o arquivo `requirements.txt` contenha todas as dependências necessárias.*

## Uso

1. **Preparar os dados**:
   Execute o notebook `prepare-data.ipynb` para processar os dados e prepará-los para o fine-tuning.

2. **Realizar o fine-tuning**:
   Execute o notebook `finetuning_amazon_titles.ipynb` para treinar o modelo com os dados preparados.

3. **Realizar inferências com o modelo original**:
   Execute o notebook `inferencia_llama3.ipynb` para realizar inferências utilizando o modelo LLaMA 3 original.

4. **Realizar inferências com o modelo fine-tunado**:
   Execute o notebook `inferencia_modelo_treinado.ipynb` para realizar inferências utilizando o modelo após o fine-tuning.

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests.

## Licença

Este projeto está licenciado sob a [MIT License](LICENSE).

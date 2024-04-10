# Python: Avance na Orientação a Objetos e Consuma API

Este projeto exemplifica a utilização avançada da Orientação a Objetos em Python, juntamente com a implementação de um servidor web usando FastAPI para consumir uma API de restaurantes. O foco é criar endpoints que permitem visualizar mensagens e cardápios de restaurantes, aproveitando os dados fornecidos por uma API externa.

## Requisitos

Antes de iniciar, certifique-se de que possui o Python instalado em sua máquina. Este projeto foi testado com Python 3.8. Recomenda-se utilizar um ambiente virtual para instalar as dependências.

## Instalação

Para configurar o ambiente do projeto, siga os passos abaixo:

1. Clone o repositório para sua máquina local (ou baixe os arquivos do projeto).
2. Crie um ambiente virtual:

   Para Linux/macOS:
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```

   Para Windows:
   ```bash
   python -m venv venv
   .\venv\Scripts\activate
   ```

3. Instale as dependências do projeto utilizando o `pip`:

   ```bash
   pip install -r requirements.txt
   ```

## Estrutura do Projeto

O projeto contém os seguintes arquivos e diretórios principais:

- `main.py`: Arquivo principal que configura e executa o servidor FastAPI, incluindo a definição dos endpoints.
- `app.py`: Script que consome a API de restaurantes e gera arquivos JSON com os dados dos restaurantes.
- `requirements.txt`: Lista de todas as dependências necessárias para executar o projeto.

## Execução

Para executar o servidor FastAPI, utilize o seguinte comando no terminal:

```bash
uvicorn main:app --reload
```

Isso iniciará o servidor localmente na porta `8000`. Você pode acessar os endpoints através da URL `http://localhost:8000`.

## Endpoints

O servidor define os seguintes endpoints:

- `/api/hello`: Exibe uma mensagem de boas-vindas do mundo da programação.
- `/api/restaurantes/`: Permite visualizar os cardápios dos restaurantes, podendo filtrar por nome do restaurante.

## Consumindo a API de Restaurantes

O script `app.py` é utilizado para consumir a API de restaurantes e gerar arquivos JSON locais com os dados dos restaurantes. Ele é executado separadamente do servidor FastAPI.

## Contribuindo

Sinta-se livre para contribuir com o projeto. Pull requests são bem-vindos. Para grandes alterações, por favor, abra uma issue primeiro para discutir o que você gostaria de mudar.

## Licença

[MIT](https://choosealicense.com/licenses/mit/)

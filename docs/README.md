# Aplicativo Web para Predição de Espécies Iris 🌸

Este é um aplicativo web interativo construído com **Streamlit** que atua como **cliente** de uma **API RESTful** que classfica espécies Iris com base em suas características morfológicas.

### Pré-requisitos

Certifique-se de ter o Python 3.11 e o Poetry instalados em seu sistema.

Para instalar o Poetry, use o método oficial:

```bash
curl -sSL [https://install.python-poetry.org](https://install.python-poetry.org) | python3 -
```

### Instalação

Clone o repositório e instale as dependências listadas no pyproject.toml:

```bash
git clone https://github.com/jorgeplatero/preditor_especies_iris.git
cd preditor-iris
poetry install
```

O Poetry criará um ambiente virtual isolado e instalará todas as bibliotecas necessárias.

### Como Rodar a Aplicação

Execute o script Python:

```bash
poetry run streamlit run app.py
```

### Funcionalidades

* **Autenticação:** implementa interface para login e registro de usuários.
* **Predição:** permite a submissão interativa das quatro características da Iris (**comprimento/largura da sépala/pétala**) para serem processadas por um modelo de Machine Learning via API externa e retorna a classe predita.
* **Histórico de predições:** o usuário pode visualizar e paginar o histórico de predições persistido no banco de dados da API.

### Tecnologias

A aplicação atua como cliente que se comunica com a API externa.

| Componente | Tecnologia | Versão | Descrição |
| :--- | :--- | :--- | :--- |
| **Frontend/App** | **Streamlit** | `^1.51.0` | Framework utilizado para o desenvolvimento do aplicativo web |
| **Comunicação** | **Requests** | `^2.32.5` | Biblioteca para requisições HTTP e consumo de API |
| **Linguagem** | **Python** | `>=3.11, <4.0` | Linguagem para desenvolvimento de scripts |
| **Gerenciamento** | **Poetry** | `2.2.1` | Gerenciador de ambientes virtuais para isolamento de dependências |

### Integrações

O aplicativo web em produção faz requisições para uma API Flask.

Link para a API: https://postech-api-ml-fase-1.vercel.app/

Link para o repositório da API: https://github.com/jorgeplatero/postech-api-ml-fase-1

### Deploy

O deploy deste aplicativo foi realizado via Streamlit Cloud. 

Link para o aplicativo web: https://preditorespeciesiris.streamlit.app/

# Thales_alura_cloud
Project testing Cloud with Alura


Passos para subir o projeto
Faça o download do repositório: Clique aqui para realizar o download

Crie um ambiente virtual:

python3 -m venv ./venv
Ative o ambiente virtual:

No Linux/Mac:
source venv/bin/activate
No Windows, abra um terminal no modo administrador e execute o comando:
Set-ExecutionPolicy RemoteSigned
venv\Scripts\activate
Instale as dependências:

pip install -r requirements.txt
Execute a aplicação:

uvicorn app:app --reload
Acesse a documentação interativa:

Abra o navegador e acesse:
http://127.0.0.1:8000/docs

Aqui você pode testar todos os endpoints da API de forma interativa.

Autenticando no Google Cloud
gcloud auth login
gcloud config set project PROJECT_ID
gcloud run deploy --port=8000
Estrutura do Projeto
app.py: Arquivo principal da aplicação FastAPI.
models.py: Modelos do banco de dados (SQLAlchemy).
schemas.py: Schemas de validação (Pydantic).
database.py: Configuração do banco de dados SQLite.
routers/: Diretório com os arquivos de rotas (alunos, cursos, matrículas).
requirements.txt: Lista de dependências do projeto.
O banco de dados SQLite será criado automaticamente como escola.db na primeira execução.
Para reiniciar o banco, basta apagar o arquivo escola.db (isso apagará todos os dados).

Documentação de Instalação e Uso do Sistema de Gerenciamento de Tarefas

Requisitos:

Python 3.x
Pip (gerenciador de pacotes do Python)
SQLite (ou qualquer banco de dados suportado pelo SQLAlchemy)

Bibliotecas Python:

Flask
Flask-SQLAlchemy
Flask-WTF
Werkzeug (para hashing de senhas)
WTForms
Instalação
Passos para configurar o projeto:
Clonar o repositório:

git clone <https://github.com/Eduardopasdf/task_manager>
cd <pasta-do-repositório>
Criar um ambiente virtual (opcional, mas recomendado):

python -m venv venv
source venv/bin/activate  # Linux/macOS
venv\Scripts\activate  # Windows

Instalar as dependências:
Execute o seguinte comando para instalar as bibliotecas necessárias:

pip install Flask Flask-SQLAlchemy Flask-WTF Werkzeug

Para criar as tabelas no banco de dados, execute o seguinte comando dentro do terminal Python:

python from app import db, appwith app.app_context():  db.create_all() exit()
Para iniciar o servidor de desenvolvimento, use o seguinte comando:python app.py

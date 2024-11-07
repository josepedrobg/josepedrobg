Sistema de Gerenciamento de Registros Médicos
Este é um sistema simples de gerenciamento de registros médicos desenvolvido com Python e MongoDB, com funcionalidades de cadastro, login, autenticação de dois fatores (2FA), criação de registros médicos, visualização, atualização e exclusão dos registros. O sistema utiliza criptografia para garantir a segurança dos dados dos pacientes.

Funcionalidades
Cadastro e Login: Funcionalidade para cadastro de novos usuários e login de profissionais de saúde.
Autenticação de Dois Fatores (2FA): Utiliza o Google Authenticator para uma camada extra de segurança.
Criação de Registros Médicos: Permite a criação de registros médicos criptografados no banco de dados.
Acesso e Visualização de Registros: Profissionais de saúde podem acessar registros médicos de pacientes de forma segura.
Atualização e Deleção de Registros: Funcionalidades para atualizar ou deletar registros médicos já existentes.
Tecnologias Usadas
Python: Linguagem de programação utilizada para implementar o sistema.
MongoDB: Banco de dados NoSQL utilizado para armazenar as informações.
Cryptography (Fernet): Biblioteca para criptografia dos dados sensíveis.
bcrypt: Biblioteca para o hashing seguro de senhas.
pyotp: Biblioteca para geração e verificação de códigos de autenticação de dois fatores.
qrcode: Biblioteca para gerar QR Codes para a configuração do 2FA.
Requisitos
Python 3.8 ou superior
MongoDB (pode ser local ou MongoDB Atlas)
 Instalação
Clone este repositório para sua máquina local:

git clone https://github.com/SeuUsuario/SistemaGerenciamentoRegistrosMedicos.git
Navegue até o diretório do projeto:

cd SistemaGerenciamentoRegistrosMedicos
Crie um ambiente virtual (opcional, mas recomendado):

python -m venv venv
Ative o ambiente virtual:

No Windows:
venv\Scripts\activate
No macOS/Linux:


source venv/bin/activate
Instale as dependências:

pip install -r requirements.txt
Configure o MongoDB:

Se você estiver usando o MongoDB Atlas, crie uma conta e obtenha a URL de conexão para o seu banco de dados.
Substitua o valor da variável uri no código (uri = "mongodb+srv://user:password@cluster0.mongodb.net/...") pela sua string de conexão.
Uso
Execute o script principal para iniciar o sistema:

python main.py
Ao iniciar, o sistema permitirá que o profissional de saúde se cadastre, faça login, configure o 2FA e acesse as funcionalidades de gerenciamento de registros médicos.

Estrutura do Projeto

SistemaGerenciamentoRegistrosMedicos/
│
├── main.py             # Código principal do sistema
├── requirements.txt    # Arquivo de dependências do projeto
├── README.md           # Este arquivo
└── .gitignore          # Arquivo para ignorar arquivos não desejados no repositório
Dependências
Adicione as dependências do seu projeto no arquivo requirements.txt:

makefile
Copiar código
pymongo==4.0.0
cryptography==39.0.1
bcrypt==4.0.1
pyotp==2.6.0
qrcode==7.3.1
Contribuições
Contribuições são bem-vindas! Se você tiver ideias para melhorar o sistema ou encontrar problemas, sinta-se à vontade para abrir issues ou enviar pull requests.

Licença
Este projeto está licenciado sob a MIT License - veja o arquivo LICENSE para mais detalhes.


<!---
josepedrobg/josepedrobg is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

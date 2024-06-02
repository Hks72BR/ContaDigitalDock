# Digital Dock

## Instruções para Iniciar a Aplicação em Execução Local
- Abra CMD como administrador

- Use comando  CD "diretório raiz do projeto" 

- Execute o comando "venv\Scripts\activate" para habilitar ambiente de Desenvolvimento

- Instale as Dependencias "pip install -r requirements.txt"

- Inicializar e migrar base de dados (copie e cole o comando ):

flask db init 
flask db migrate -m "Initial migration."
flask db upgrade

- COnfigure variavel de ambiente "set FLASK_ENV=development"

- Inicie a aplicação "flask run".
  

### Requisitos

- Instalar dependencias do aquivo "requirements.txt".
- Postman instalado na ultima versão disponivel para fazer chamada de API

### Passos para teste da aplicação.

- Com o Postman aberto, faça a criação de chamadas com os metodos abaixo seguindo este ip 
http://127.0.0.1:5000/

- POST /portadores: Cria um novo portador.
- DELETE /portadores/<id>: Remove um portador.
- POST /contas: Cria uma nova conta.
- GET /contas/<id>: Consulta uma conta.
- POST /contas/<id>/fechar: Fecha uma conta.
- POST /contas/<id>/saque: Realiza um saque.
- POST /contas/<id>/deposito: Realiza um depósito.
- POST /contas/<id>/bloquear: Bloqueia uma conta.
- POST /contas/<id>/desbloquear: Desbloqueia uma conta.
- GET /contas/<id>/extrato: Consulta o extrato de uma conta por período. Usar o exemplo a seguir:
   http://127.0.0.1:5000/contas/1/extrato?inicio=2023-01-01&fim=2023-12-31







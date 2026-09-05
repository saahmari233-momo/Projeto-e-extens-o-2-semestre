# Modelagem Inicial — POO

## Projeto Fome 0

### Principais Entidades

O sistema Fome 0 possui as seguintes entidades:

- Usuario
- Instituicao
- Doacao
- Solicitacao
- PontoDistribuicao
- Notificacao

### Usuario

**Atributos:**
- id
- nome
- email
- telefone
- endereco
- tipoUsuario

**Métodos:**
- cadastrar()
- fazerLogin()
- solicitarAlimento()

### Instituicao

**Atributos:**
- id
- nome
- CNPJ
- endereco
- telefone

**Métodos:**
- cadastrarDoacao()
- receberSolicitacao()
- confirmarEntrega()

### Doacao

**Atributos:**
- id
- alimento
- quantidade
- validade
- dataCadastro
- status

**Métodos:**
- cadastrar()
- atualizarStatus()
- cancelar()

### Solicitacao

**Atributos:**
- id
- data
- quantidade
- status
- observacao

**Métodos:**
- criar()
- cancelar()
- acompanharStatus()

### PontoDistribuicao

**Atributos:**
- id
- nome
- endereco
- horarioFuncionamento
- capacidade

**Métodos:**
- cadastrarPonto()
- atualizarHorario()

### Notificacao

**Atributos:**
- id
- mensagem
- data
- lida

**Métodos:**
- enviar()
- marcarComoLida()

## Relacionamentos

- Usuario realiza Solicitacao.
- Instituicao realiza Doacao.
- Solicitacao pode ser atendida por uma Instituicao.
- Doacao pode ser encaminhada para um PontoDistribuicao.
- Usuario recebe Notificacao.

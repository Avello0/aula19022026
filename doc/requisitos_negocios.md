# Requisitos do Sistema – Biblioteca Digital

## 1. Requisitos Funcionais (RF)

### RF01 – Cadastro de Usuário
O sistema deve permitir que novos usuários realizem cadastro informando nome, e-mail e senha.

**Critério de Aceitação:**
- Deve ser possível criar conta com e-mail válido.
- O sistema deve impedir cadastro com e-mail já existente.
- Senha deve ter no mínimo 6 caracteres.

---

### RF02 – Login de Usuário
O sistema deve permitir que usuários autenticados realizem login.

**Critério de Aceitação:**
- Login deve ocorrer com e-mail e senha válidos.
- Mensagem de erro deve aparecer para credenciais inválidas.

---

### RF03 – Cadastro de Livro
O sistema deve permitir o cadastro de livros com título, autor, gênero e tempo estimado de leitura.

**Critério de Aceitação:**
- Todos os campos devem ser obrigatórios.
- O livro deve aparecer na listagem após cadastro.

---

### RF04 – Listagem de Livros
O sistema deve exibir todos os livros cadastrados.

**Critério de Aceitação:**
- A lista deve exibir título, autor e gênero.
- A lista deve atualizar após novo cadastro.

---

## 2. Requisitos Não Funcionais (RNF)

### RNF01 – Desempenho
O sistema deve carregar a página principal em até 3 segundos com até 1000 livros cadastrados.

**Critério de Verificação:**
- Teste de carregamento com base de dados populada.

---

### RNF02 – Segurança
As senhas dos usuários devem ser armazenadas de forma criptografada.

**Critério de Verificação:**
- Verificação de hash no banco de dados.
- Senhas não podem estar em texto plano.

---

## 3. Regras de Negócio (RN)

### RN01 – E-mail Único
Cada usuário deve possuir um e-mail único no sistema.

---

### RN02 – Tempo de Leitura Positivo
O tempo estimado de leitura de um livro deve ser maior que zero.

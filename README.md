# Projeto A3 Unisul primeira fase

# Objetivo:

# Requisitos funcionais
- RF01 - Cadastro de ferramentas: O software deve permitir que o usuário cadastre as
ferramentas, como nome, marca e custo.
- RF02 - Cadastro de amigos: O software deve permitir que o usuário cadastre os dados
dos amigos, como nome, e-mail e telefone.
- RF03 - Registro de empréstimos: O software deve permitir que o usuário registre os
empréstimos de ferramentas para os amigos, informando a ferramenta, o amigo, a
data do empréstimo e os dados previstos de devolução.
- RF04 - Registro de empréstimos: O software deve mostrar um aviso ao usuário a cada
novo empréstimo se a uma pendência de devolução.
- RF05 - Relatório de ferramentas: O software deve gerar um relatório com todas as
ferramentas cadastradas, informando a descrição e o valor de cada uma, bem como
o gasto total com a aquisição das ferramentas.
- RF06 - Relatório de empréstimos ativos: O software deve gerar um relatório com todos
os empréstimos que ainda não foram devolvidos, informando a ferramenta
emprestada, o amigo que pegou emprestado, a data de empréstimo e os dados
previstos de devolução.
- RF07 - Relatório de todos os empréstimos: O software deve gerar um relatório com
todos os empréstimos realizados, informando a ferramenta emprestada, o amigo que
pegou emprestado, a data de empréstimo e os dados de devolução e qual amigo faz
mais empréstimos.
- RF08 - Agenda integrada: O software deve compartilhar os lembretes de avisos dos
eventos por e-mail.
- RF09 - Verificação de ferramentas não devolvidas: O software deve verificar a cada
novo empréstimo se o amigo ainda tem ferramentas não devolvidas e informar ao
usuário.

# Requisitos não funcionais
- RNF01 - Localização: O software deve ser executado localmente no computador do
usuário, sem necessidade de conexão com a internet.
- RNF02 - Interface Amigável: O software deve ter uma interface fácil de usar e intuitiva,
adequada para usuários não técnicos, como o tio-avô.
- RNF03 - Segurança: O software deve garantir a segurança dos dados cadastrados,
protegendo informações pessoais e financeiras dos usuários.
- RNF04 - Integração com o Google agenda: O sistema deve integrar-se de forma eficaz
e confiável com a Google agenda, garantindo o compartilhamento correto de
lembretes de eventos.

# Banco de dados
- Abaixo o script para a criação do banco de dados e da tabela.
```
CREATE DATABASE IF NOT EXISTS db_A3;
USE db_A3;
DROP TABLE IF EXISTS tb_ferramentas;
CREATE TABLE tb_ferramentas (
id INTEGER NOT NULL,
ferramenta VARCHAR(100),
marca VARCHAR(50),
preco DOUBLE,
PRIMARY KEY(id)
);
USE db_A3;
DROP TABLE IF EXISTS tb_amigos;
CREATE TABLE tb_amigos (
id INTEGER NOT NULL,
nome VARCHAR(100),
telefone VARCHAR(50),
PRIMARY KEY(id)
);
```


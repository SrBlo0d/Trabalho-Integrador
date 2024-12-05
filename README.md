# Match Games

## Apresentação Breve

Este projeto é uma aplicação web desenvolvida em Python, com o objetivo de ajudar os usuários a verificar as configurações mínimas necessárias para rodar o jogo de sua escolha no computador. O usuário escolhe o jogo diretamente da interface web, e a aplicação compara as especificações mínimas do jogo com as configurações do sistema do usuário. Isso ajuda a evitar a compra de um computador que não consiga rodar o jogo desejado.

## Objetivo

O objetivo desta aplicação é fornecer aos usuários uma maneira simples de verificar se o computador possui a configuração mínima necessária para rodar o jogo selecionado. Isso evita problemas como adquirir um PC que não suporte o desempenho básico exigido pelo jogo, garantindo uma experiência de jogo funcional.

## Funcionalidades

- **Escolha de Jogo**: O usuário pode selecionar um jogo de uma lista já disponível na aplicação.
- **Verificação de Configuração Mínima**: A aplicação verifica as especificações mínimas do jogo selecionado em comparação com as configurações de hardware do computador do usuário.
- **Interface Web Interativa**: A aplicação oferece uma interface web simples e amigável, onde o usuário pode facilmente selecionar o jogo e inserir as configurações de seu computador para fazer a comparação.

## Instalação de Dependências

1. Certifique-se de ter o [Python](https://www.python.org/) instalado em seu sistema.
2. Clone este repositório:
   ```bash
   git clone https://github.com/SrBlo0d/Projeto-Integrador-Web.git

3. Navegue até o diretório do projeto:

cd Trabalho-Integrador

4. Crie um ambiente virtual para o projeto e ative-o:

python -m venv venv

*source venv/bin/activate  # no Linux/macOS

*venv\Scripts\activate     # no Windows

5. Instale as dependências necessárias com:

pip install -r requirements.txt

## Passo a Passo para Rodar a Aplicação

1. Configuração do Banco de Dados PostgreSQL:

A aplicação usa um banco de dados PostgreSQL. Certifique-se de que seu banco de dados está configurado corretamente. As configurações de acesso ao banco são as seguintes:

*Host: postgres-aula.cuebxlhckhcy.us-east-1.rds.amazonaws.com

*Nome do Banco de Dados: postgresaula

*Usuário: postgresaula

*Senha: PostgresAula123!

*Porta: 5432

2. Crie um arquivo de configuração para as variáveis de ambiente, caso necessário (exemplo: .env):

   *postgres_host= postgres-aula.cuebxlhckhcy.us-east-1.rds.amazonaws.com #Host
   
   *postgres_dbname= postgresaula # Nome do banco
   
   *postgres_user= postgresaula # Nome de usuário
   
   *postgres_password= PostgresAula123! # Senha
   
   *postgres_port= 5432

3. Execute as migrações do banco de dados, se necessário:

python manage.py migrate

4. Execute a aplicação localmente:

python app.py

5. Abra o navegador e acesse github.com/SrBlo0d/Trabalho-Integrador.

6. A interface será carregada, e você poderá selecionar o jogo desejado para verificar se a configuração do seu computador é compatível.

## Teste

Para testar se a aplicação está funcionando corretamente:

1. Acesse a interface web em http://localhost:5000.
2. Selecione um jogo da lista e insira as especificações do seu computador.
3. Verifique se a comparação entre a configuração do seu computador e os requisitos do jogo está sendo realizada corretamente.

Caso não consiga conectar ao banco de dados ou algum outro erro aconteça, confira a configuração das variáveis de ambiente e se as dependências foram instaladas corretamente.

## Observações

*A aplicação depende de um banco de dados para armazenar as especificações dos jogos e os dados dos usuários. Certifique-se de que o banco de dados está configurado e migrado corretamente.

*O projeto pode ser expandido com mais jogos e funcionalidades, como a integração com APIs externas para obter requisitos de jogos automaticamente.

# Match Games

## Apresentação Breve

Este projeto é uma aplicação web desenvolvida em Python, que tem como objetivo ajudar os usuários a verificar a configuração necessária para rodar o jogo de sua escolha no computador. Ele oferece uma maneira fácil de comparar as especificações recomendadas e mínimas de diferentes jogos com as configurações do sistema do usuário, ajudando a evitar a compra de um computador que não seja capaz de rodar o jogo desejado.

## Objetivo

O objetivo desta aplicação é fornecer uma ferramenta para os jogadores verificarem se seu computador tem a configuração necessária para rodar os jogos que eles desejam jogar. A aplicação ajuda a evitar problemas como a compra de um PC que não suporte o desempenho exigido por um jogo específico.

## Funcionalidades

- **Verificação de Configuração**: O usuário pode selecionar o jogo desejado e a aplicação verificará se a configuração do computador é compatível com os requisitos do jogo.
- **Comparação de Requisitos**: A aplicação compara as especificações mínimas e recomendadas do jogo com as configurações de hardware do computador do usuário.
- **Sugestões de Melhoria**: Caso o computador não tenha a configuração necessária, a aplicação sugere ajustes ou melhorias no hardware para garantir que o jogo seja jogável sem problemas.
- **Interface Web**: A aplicação oferece uma interface web simples e interativa para facilitar a consulta e a visualização das informações.

## Instalação de Dependências

1. Certifique-se de ter o [Python](https://www.python.org/) instalado em seu sistema.
2. Clone este repositório:
   ```bash
   git clone https://github.com/SrBlo0d/Projeto-Integrador-Web.git

3. Navegue até o diretório do projeto:

cd nome-do-repositorio

4. Crie um ambiente virtual para o projeto e ative-o:

python -m venv venv

*source venv/bin/activate  # no Linux/macOS

*venv\Scripts\activate     # no Windows

5. Instale as dependências necessárias com:

pip install -r requirements.txt

## Passo a Passo para Rodar a Aplicação

1. Certifique-se de ter um banco de dados relacional configurado. Este projeto usa [MySQL/PostgreSQL], então, crie o banco de dados e configure as credenciais.

2. Crie um arquivo de configuração para as variáveis de ambiente, caso necessário (exemplo: .env):

   *postgres_host= postgres-aula.cuebxlhckhcy.us-east-1.rds.amazonaws.com
   
   *postgres_dbname= postgresaula # Nome do banco
   
   *postgres_user= postgresaula # Nome de usuário
   
   *postgres_password= PostgresAula123! # Senha
   
   *postgres_port= 5432

4. Execute as migrações do banco de dados, se necessário:

python manage.py migrate

4. Execute a aplicação localmente:

python app.py

5. Abra o navegador e acesse http://localhost:5000 (ou a porta configurada no seu projeto).

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

# AGENTS.md

## Visão geral
<!-- 
Descreva brevemente o projeto: qual é o objetivo da aplicação, qual problema ela resolve e, se necessário, quem são os principais usuários. -->
A aplicação tem como objetivo apresentar informações sobre a história e curiosidades relevantes do filme Sociedade dos Poetas Mortos (1989), além de coletar dados sobre as preferências e os interesses dos usuários. O site é voltado tanto à comunidade de fãs quanto a pessoas interessadas em conhecer mais profundamente a obra.

## Tecnologias
<!-- Liste as principais tecnologias, frameworks, bibliotecas e serviços utilizados no projeto. -->
O site deve apresentar uma interface objetiva, acessível, intuitiva e visualmente organizada.

As tecnologias permitidas para o desenvolvimento são:
- HTML - para a estrutura das páginas
- CSS - para a estilização e responsividade
- JavaScript - para interações do sistema
- Node.js - para a execução do backend
- Chart.js - para a criação de gráficos e visualizações de dados

## Comandos

<!-- Informe os comandos necessários para trabalhar com o projeto. -->
- Os comandos de execução segue os que já estão definidos nas configurações package.json do projeto

## Arquitetura

<!-- Explique como o projeto está organizado e como uma funcionalidade deve ser implementada.
Inclua informações como: -->
- Estrutura das principais pastas 
    - public/
        - assets/
            - imgs/
        - css/
        - dashboard/
        - html/
    - src/
        - routes/
        - controllers/
        - models/
        - database/

- Responsabilidade de cada pasta
    - assets/ - (armazenar imagens e arquivos do site)
    - css/ - (estilização e resposividade das páginas)
    - html/ - (esqueleto do site)
    - dashboard/ - (Interface para vizualizar os dados coletados)
    - routes/ - (Rotas, caminhos por onde os dados serão enviados)
    - controllers/ - (Validações que o dado precisa passar antes de montar a query)
    - models/ - (Criação de toda query que será efetuada no banco de dados)
    - database/ - (Credenciais de banco de dados para efetuar a query )

- Fluxo de uma requisição
    - O usuário realiza uma ação
    - A requisição é encaminhada para a rota correspondente
    - O controller recebe a requisição e realiza o tratamento dos dados
    - O model executa a operação necessária no banco de dados
    - O resultado retorna ao controller
    - A API envia uma resposta podem ser uma apresentação/vizualização dos dados ou informar resultado da requisição

<!-- - Onde criar novos arquivos -->
Interface: diretórios de frontend dentro de public/
Estilos: public/css/
Rotas da API: src/routes/
Tratamento das requisições: src/controllers/
Consulta de dados: src/models/
Conexão do banco: src/database/

## Padrões de desenvolvimento

- Seguir um padrão de mensagens para commits no github
- Variáveis sempre com let e não var, se preciso, const também pode ser utilizado
- Nome das variáveis sempre devem estar em português

## Cuidados e restrições

<!-- Liste aquilo que o agente não deve fazer ou que exige atenção antes de realizar alterações. -->

- Não modificar a estrutura-base da API fornecida pela faculdade sem autorização
- Não adicionar tecnologias não autorizadas
- Não inventar informações aleatórias sobre o filme ou dados do usuário
- Pode implementar funionalidades desde que não altere a estrutura base da API ou que não tenha relação com a proposta da tarefa
- Verifique se já existe um arquivo responsável pela mesma funcionalidade. Evite duplicar responsabilidades ou criar novas pastas sem necessidade

## Regra geral: 
Antes de implementar uma alteração, siga as tecnologias, arquitetura, convenções e restrições descritas neste documento. Caso alguma informação esteja ausente, analise o código existente e siga os padrões já adotados no projeto.



 

<h1 align="center">Integração Gemini  com ServiceNow: Perguntas e Respostas</h1>
<p align="center">
 <a href="#objetivo">Descrição</a> • 
 <a href="#tecnologias">Funcionalidades</a> • 
 <a href="#contribuicao">Pré-requisitos:</a> • 
 <a href="#licenc-a">Demonstração</a> • 
 
</p>
<p align="center"> Descrição</p>

Esta integração conecta um modelo de linguagem avançado, o Gemini, ao ServiceNow, permitindo que os usuários façam perguntas em linguagem natural sobre dados do ServiceNow e recebam respostas precisas e informativas.

Funcionalidades:

Perguntas em linguagem natural: Os usuários podem fazer perguntas em linguagem natural sobre qualquer tópico relacionado ao ServiceNow, sem a necessidade de usar comandos ou sintaxe específicos.
Respostas abrangentes: O Gemini acessa e processa dados do ServiceNow para gerar respostas abrangentes e informativas às perguntas dos usuários.


Resposta: Este campo recebe a pergunta do usuário e a envia para o Gemini.
Pergunta: Este campo recebe a resposta do Gemini e a exibe para o usuário.
Exemplos de uso:

Um usuário pode perguntar: "O que é um client script?"
O Gemini acessa o ServiceNow e responde: "m client script, também conhecido como script do lado do cliente, é um tipo de programa usado no ServiceNow para automatizar tarefas e melhorar a experiência do usuário diretamente no navegador do cliente. Ele é escrito em JavaScript e executado no dispositivo do usuário, em vez do servidor do ServiceNow."
Benefícios:

Maior eficiência: Os usuários podem encontrar as informações que precisam com mais rapidez e facilidade, sem a necessidade de navegar por menus complexos ou pesquisar manualmente por dados.
Melhor experiência do usuário: A interface natural e intuitiva permite que os usuários façam perguntas de forma natural, como se estivessem conversando com um especialista.
Maior produtividade: Ao automatizar a busca por informações, os usuários podem dedicar mais tempo a tarefas mais importantes.
Tomada de decisões mais rápida: As respostas precisas e informativas do Gemini podem ajudar os usuários a tomar decisões mais rápidas e informadas.

Configuração:
Acesse sua conta Gemini:

Abra o navegador da web e acesse o site da Gemini: https://www.gemini.com/
Faça login em sua conta Gemini usando seu e-mail e senha.
2. Navegue até a página de configurações de API:

No canto superior direito da tela, clique no ícone de perfil (foto ou inicial do seu nome).
No menu suspenso, selecione "Configurações".
No painel esquerdo, clique em "API".
3. Crie uma nova chave API:

Na página de configurações de API, clique no botão "Criar nova chave API".
Digite um nome descritivo para sua chave API (por exemplo, "Chave API para integração ServiceNow").
Selecione o escopo de acesso desejado para sua chave API. O escopo define quais ações a chave API pode realizar em sua conta. Para integrações simples, como a integração com o ServiceNow, geralmente é suficiente selecionar o escopo "Somente Leitura".
Clique no botão "Criar chave API".
4. Copie sua chave API:

Uma mensagem pop-up será exibida contendo sua chave API e código QR.
Importante: Guarde sua chave API em um local seguro. Não a compartilhe com ninguém.
Você também pode baixar um arquivo CSV contendo sua chave API e código QR.
5. Use sua chave API:

Sua chave API agora está pronta para ser usada em sua integração ServiceNow.
Consulte a documentação da sua integração específica para obter instruções sobre como configurar a chave API.

Este guia detalhado irá te orientar passo a passo na configuração da API Gemini no ServiceNow, permitindo que você utilize o poder do Gemini para enriquecer suas aplicações e automatizar tarefas.

Pré-requisitos:

Uma conta Gemini com chave API criada (conforme instruções anteriores).
Uma instância do ServiceNow com acesso à integração Gemini.
Familiaridade básica com o ServiceNow e a criação de mensagens REST.
Passos:

1. Acessando sua Instância PDI:

Abra o navegador da web e acesse a sua instância pessoal do ServiceNow (PDI): https://developer.servicenow.com/
Faça login usando suas credenciais de desenvolvedor.
2. Localizando a Tabela "Rest Message":

No menu esquerdo, clique em "System UI".
Na barra de pesquisa, digite "Rest Message" e pressione Enter.
Selecione a tabela "sys_rest_message" na lista de resultados.
3. Criando uma Nova Mensagem REST:

Clique no botão "Novo" na parte superior da página.
Na seção "Nome", digite um nome descritivo para sua mensagem REST, como "Gemini API Integration".
Na seção "Descrição", forneça uma breve descrição da finalidade da mensagem REST.
Clique no botão "Salvar".
4. Configurando o Endpoint:

Na aba "Geral", localize o campo "Endpoint".
Insira o endpoint da API Gemini que você deseja utilizar. Por exemplo, para gerar texto, o endpoint seria: https://generativelanguage.googleapis.com/v1beta/models/gemini-pro:generateContent.
Clique no botão "Salvar".
5. Adicionando a Chave API na Aba HTTP REQUEST:

Mude para a aba "HTTP REQUEST".
Na seção "Cabeçalhos", clique no botão "Novo".
No campo "Nome", digite "Authorization".
No campo "Valor", digite "Bearer YOUR_API_KEY", substituindo "YOUR_API_KEY" pela sua chave API da Gemini.
Clique no botão "Salvar".
6. Criando um Novo Método HTTP:

Na aba "HTTP Methods", clique no botão "Novo".
No campo "Nome", digite um nome descritivo para o método, como "Generate Text".
No campo "Método HTTP", selecione "POST".
No campo "Endpoint", selecione o endpoint que você configurou anteriormente.
Clique no botão "Salvar".
7. Salvando as Alterações:

Clique no botão "Salvar" na parte superior da página para salvar todas as alterações.
8. Testando a Integração:

Na aba "HTTP Methods", selecione o método que você criou.
Clique no botão "Testar".
Se a integração for bem-sucedida, você receberá uma resposta com os resultados da sua solicitação.

![image](https://github.com/Rodrigocabo/GeminiNow/assets/84506268/f12494c9-4ed7-40d2-9826-a4b029549bd7)
![image](https://github.com/Rodrigocabo/GeminiNow/assets/84506268/a64519ed-125c-4513-b029-50cc5243f53d)

Demonstração

![image](https://github.com/Rodrigocabo/GeminiNow/assets/84506268/c89116ec-7bbc-42cb-87c6-797ad7118a4c)

![Blue Futuristic Artificial Intelligence Instagram Post](https://github.com/Rodrigocabo/GeminiNow/assets/84506268/46cab35f-a978-4616-96e3-61ef05e83e65)











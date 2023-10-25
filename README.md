_Usei, além do Laravel, duas API's, uma para o banco de dados e login+cadastro de usuário (Pusher) e outra para o chat (Chatify). É o PHP 7.2. Ficou simplificado, rápido e seguro por ser feito com uma API._ Eu só consegui terminar de fazer a API funcionar no último momento, eu preciso de mais tempo para implementar as outras funções como login com CPF, relação Cliente-Colaborador, apenas Clientes abrirem chamado. O que pude entregar para hoje foi a função de Login e Chat funcionais com banco de dados.

# Resultado

Login:
![Pasted image 20231024184523](https://github.com/NMarlon/Sistema-de-Suporte-_-ProConsult-Engenharia/assets/43282318/d00cb27f-6748-4a50-a8df-5fa0d5f615e8)
![Pasted image 20231024184640](https://github.com/NMarlon/Sistema-de-Suporte-_-ProConsult-Engenharia/assets/43282318/c2855be2-402f-4af4-90ae-3bd07ab523cd)



Cadastro:
![Pasted image 20231024184607](https://github.com/NMarlon/Sistema-de-Suporte-_-ProConsult-Engenharia/assets/43282318/f17d2820-8180-48e1-af0f-bbf623075680)


Pós-login:
![Pasted image 20231024184658](https://github.com/NMarlon/Sistema-de-Suporte-_-ProConsult-Engenharia/assets/43282318/d3bd908d-b241-4beb-8d3c-ee047b02137c)



Página de chat: http://localhost:8000/chatify
![Pasted image 20231024193958](https://github.com/NMarlon/Sistema-de-Suporte-_-ProConsult-Engenharia/assets/43282318/d0151655-5842-44c8-93e4-b815176696ec)





# Sobre
## Tecnologias
- Laravel
- PHP 7.2 com XAMPP
	- PhpMyAdmin
### De API
- PUSHER (https://pusher.com/)
- Chatify (https://www.chatify.com/)

## Detalhes
Por usar API, o sistema já vem com a segurança embutida nas transações das mensagens com cifra "AES-256-CBC".


# Como usar
- Instale o XAMPP com a versão antiga do PHP 7.2
- Instale o NodeJS
- Instale o PHP 7.2.4
- Baixe o diretório do projeto
- Com um prompt de comando na raiz do diretório: php artisan ser
- em outro prompt no mesmo diretório: npm run dev
- Abra: 
	- localhost:8000/
		- registre dois usuários
	- localhost:8000/chatify
		- Para abrir o chat




# Tratamento de erros
Foram diversos erros que ocorreram nesses dias que precisaram ser tratados.
- Um código na API estava nativamente errada na sintaxe (era uma vírgula que estava à mais) quebrando o código, removi a vírgula e resolveu.
- A versão do PHP mais atual (8.1) funciona com menos bugs e mais atualização do que a 7.2, por isso, algumas bibliotecas travavam na instalação e tive que recorrer à forçar a instalação dessas bibliotecas com PHP mais antigo.


# Funções que gostaria de implementar
Por conta do tempo, ficaram algumas funções ainda à implementar:
- Cadastro na página: ./cadastro-atendente/ para cadastrar os **atendentes**
- Página voltada para interação fechada apenas cliente-atendente, sem cliente-cliente.
- Redirecionamento automático pós login para a página do chat (chatify)

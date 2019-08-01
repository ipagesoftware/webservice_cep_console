# webservice_cep_console

Exemplo em aplicação em console de como consumir um Web Service da Empresa Ipage Software.

A que se destina este Web Service? Este Web Service tem por finalidade consultar Códigos de endereçamento Postal (CEP) de todo o Brasil de forma simples e descomplicada. As informações retornadas após a consulta ao Web Service possui diversos formatos, são eles: XML, JSON, JavaScript, formato texto PIPED, formato texto Querty. Definição dos parâmetros. O CEP informado deve conter apenas números com até 08 (oito caracateres), em caso de valores inválidos passados ao Web Service o mesmo realizará automaticamente um filtro, deixando passar apenas números. Se mesmo assim o valor do CEP informado não satisfazer o critério uma mensagem de erro será reportada.

# Configuração
No arquivo ws.ini você poderá configurar a chave de acesso do Web Service e o link do Web Service. O resultado da consulta será exibido no console e um arquivo será gerado no formato definido.

[DADOS]

KEY={chave}

[WEBSITE]

LINK_CEP=https://www.ipage.com.br/ws/v1/cep/

A chave de acesso ao Web Service é obrigatória e deve ser passada na URL junto com o CEP, formato de retorno e deve ser compatível com o esperado pelo Web Service. Caso não possua uma chave de acesso, solicite no site da ipage: https://www.ipage.com.br

# Comandos

Exemplo: ws <comando> <parâmetro(s)>

 [version ou -v] ................... Exibe a versão do console CLI
 
 config ............................ Exibe informações do arquivo ini do web service
 
 cep ............................... Exibe os dados do cep
 

   Parâmetro(s):
   
   num cep ......................... Número do cep
   
   Exemplo de uso:
   
   ws cep 54360080


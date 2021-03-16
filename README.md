# Projeto MITWAY

# Introdução
Para este projeto é necessário a seguinte configuração:
- [X] PHP >=7.4.
- [X] MYSQL >= 5.6
- [X] Apache 2
- [X] Composer >= 2.0.11
- [X] Laravel Passport = 9.2
 
# Instalação

Para instalar o projeto basta copiar o arquivo ```.env.example``` para um novo arquivo chamado ``` .env ``` abra o arquivo e mude as os parâmetros de configuração com o banco de dados
```  
DB_HOST={DATABASE HOST OR IP}
DB_PORT={DATABASE PORT}
DB_DATABASE={DATABASE NAME}
DB_USERNAME={DATABASE USER}
DB_PASSWORD={DATABASE PASSWORD}
```
# Database
Suba o arquivo  ```database.sql``` para alimentar a base de dados com as tabelas e estrutura inicial do projeto.

# Laravel 
Após as configurações de banco realiadas executar o comando :

```composer install``` na raiz do projeto

após concluída a instalação executar o comando:

```php artisan key:generate ```

será gerada uma chave criptografada única para o projeto

rode o comando ```php artisan passport:install``` para configurar o oauth.

rode o comando ```php artisan passport:client``` para gerar as chaves do oauth.

rode o comando ```php artisan migrate``` para gerar as bases de dados. (somente caso não tenha feito manualmente utilizando o arquivo  ```database.sql ```)
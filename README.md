<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://github.com/laravel/framework/actions"><img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## About Laravel

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable and creative experience to be truly fulfilling. Laravel takes the pain out of development by easing common tasks used in many web projects, such as:

-   [Simple, fast routing engine](https://laravel.com/docs/routing).
-   [Powerful dependency injection container](https://laravel.com/docs/container).
-   Multiple back-ends for [session](https://laravel.com/docs/session) and [cache](https://laravel.com/docs/cache) storage.
-   Expressive, intuitive [database ORM](https://laravel.com/docs/eloquent).
-   Database agnostic [schema migrations](https://laravel.com/docs/migrations).
-   [Robust background job processing](https://laravel.com/docs/queues).
-   [Real-time event broadcasting](https://laravel.com/docs/broadcasting).

Laravel is accessible, powerful, and provides tools required for large, robust applications.

## Learning Laravel

Laravel has the most extensive and thorough [documentation](https://laravel.com/docs) and video tutorial library of all modern web application frameworks, making it a breeze to get started with the framework.

You may also try the [Laravel Bootcamp](https://bootcamp.laravel.com), where you will be guided through building a modern Laravel application from scratch.

If you don't feel like reading, [Laracasts](https://laracasts.com) can help. Laracasts contains thousands of video tutorials on a range of topics including Laravel, modern PHP, unit testing, and JavaScript. Boost your skills by digging into our comprehensive video library.

## Laravel Sponsors

We would like to extend our thanks to the following sponsors for funding Laravel development. If you are interested in becoming a sponsor, please visit the [Laravel Partners program](https://partners.laravel.com).

### Premium Partners

-   **[Vehikl](https://vehikl.com)**
-   **[Tighten Co.](https://tighten.co)**
-   **[Kirschbaum Development Group](https://kirschbaumdevelopment.com)**
-   **[64 Robots](https://64robots.com)**
-   **[Curotec](https://www.curotec.com/services/technologies/laravel)**
-   **[DevSquad](https://devsquad.com/hire-laravel-developers)**
-   **[Redberry](https://redberry.international/laravel-development)**
-   **[Active Logic](https://activelogic.com)**

## Contributing

Thank you for considering contributing to the Laravel framework! The contribution guide can be found in the [Laravel documentation](https://laravel.com/docs/contributions).

## Code of Conduct

In order to ensure that the Laravel community is welcoming to all, please review and abide by the [Code of Conduct](https://laravel.com/docs/contributions#code-of-conduct).

## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell via [taylor@laravel.com](mailto:taylor@laravel.com). All security vulnerabilities will be promptly addressed.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).

# Comandos Essenciais para Projetos Laravel

Este guia apresenta os principais comandos utilizados no terminal para gerenciar projetos Laravel, abrangendo desde a instalação até a execução de tarefas comuns com o Composer e o Artisan.

## 🧰 Instalação de Dependências

Após clonar o projeto, instale as dependências PHP com o Composer:

```bash
composer install
```

Se desejar atualizar as dependências para as versões mais recentes permitidas pelas restrições definidas no `composer.json`, utilize:

```bash
composer update
```

## ⚙️ Configuração do Ambiente

Copie o arquivo de exemplo de variáveis de ambiente e gere a chave da aplicação:

```bash
cp .env.example .env
php artisan key:generate
```

## 📃 Migrações e Seeders

Execute as migrações para criar as tabelas no banco de dados:

```bash
php artisan migrate
```

Para popular o banco de dados com dados iniciais (seeders), utilize:

```bash
php artisan db:seed
```

Caso deseje resetar o banco de dados e executar as migrações e seeders novamente:

```bash
php artisan migrate:fresh --seed
```

## 🚀 Servidor de Desenvolvimento

Inicie o servidor de desenvolvimento integrado do Laravel:

```bash
php artisan serve
```

Por padrão, a aplicação estará disponível em [http://localhost:8000](http://localhost:8000).

## 🥪 Testes

Para executar os testes automatizados da aplicação:

```bash
php artisan test
```

## 📂 Outras Comandos Úteis do Artisan

-   Listar todos os comandos disponíveis:

    ```bash
    php artisan list
    ```

-   Obter ajuda sobre um comando específico:

    ```bash
    php artisan help migrate
    ```

-   Criar um novo controlador:

    ```bash
    php artisan make:controller NomeDoControlador
    ```

-   Criar um novo modelo:

    ```bash
    php artisan make:model NomeDoModelo
    ```

-   Criar um novo middleware:

    ```bash
    php artisan make:middleware NomeDoMiddleware
    ```

-   Criar uma nova migration:

    ```bash
    php artisan make:migration create_nome_da_tabela_table
    ```

Para mais detalhes sobre os comandos do Artisan, consulte a [documentação oficial do Laravel](https://laravel.com/docs/11.x/artisan).

---

<!-- <p align="center"><img src=".github/logo.png" width="200" alt="FreelanceHours Logo"></p> -->

<p align="center">
  <img alt="PHP version" src="https://img.shields.io/static/v1?label=php&message=8.2&color=18181B&labelColor=5354FD">
  <img alt="Laravel version" src="https://img.shields.io/static/v1?label=laravel&message=11.9&color=18181B&labelColor=5354FD">
</p>

# FreelanceHours

FreelanceHours é uma aplicação desenvolvida em PHP, Laravel e Livewire, permitindo que freelancers enviem propostas de horas para contribuir em projetos específicos.

<p align="center">
  <!-- <img alt="Preview do projeto desenvolvido." src=".github/preview.png" width="80%"> -->
</p>

## Tecnologias Utilizadas

- [**PHP**](https://www.php.net/): Linguagem de programação base do projeto.
- [**Laravel**](https://laravel.com/): Framework PHP que estrutura a aplicação.
- [**Livewire**](https://laravel-livewire.com/): Facilita a criação de interfaces dinâmicas e reativas sem sair do Laravel.
- [**Tailwind CSS**](https://tailwindcss.com/): Framework CSS para desenvolvimento de interfaces modernas e responsivas.

## Configuração e Execução

Siga os passos abaixo para configurar e executar o projeto localmente:

### Pré-requisitos

Certifique-se de ter as seguintes ferramentas instaladas:

- **PHP 8.2**
- **Composer**
- **Node.js** (para compilação de assets)
- **MySQL** ou **PostgreSQL** (banco de dados)

### Passo a Passo

1. **Clone o repositório:**
    ```bash
    git clone https://github.com/seu-usuario/freelance-hours.git
    cd freelance-hours
    ```
2. **Instale as dependências do PHP e do Node.js:**
    ```bash
    composer install
    npm install
    ```
3. **Configure o arquivo ```.env```:**
    - Copie o arquivo de exemplo ```.env.example```
        ```bash
        cp .env.example .env
        ```
    - Configure as variáveis de ambiente, incluindo as informações de conexão com o banco de dados.
4. **Gere a chave da aplicação:**
    ```bash
    php artisan key:generate
    ```
5. **Execute as migrações e seeds (se aplicável):**
    ```bash
    php artisan migrate --seed
    ```
6. **Configure o Tailwind CSS:**
    - Se o Tailwind CSS ainda não estiver instalado e configurado, adicione-o ao projeto:
    ```bash
    npm install -D tailwindcss postcss autoprefixer
    npx tailwindcss init -p
    ```
    - Compile os assets:
    ```bash
    npm run dev
    ```
7. **Instale o Livewire:**
    - Instale o Livewire com o Composer:
    ```bash
    composer require livewire/livewire
    ```
8. **Inicie o servidor de desenvolvimento:**
    ```bash
    php artisan serve
    ```
O projeto estará disponível em [localhost:8000](http://localhost:8000).

## Licença

Este projeto está licenciado sob a licença MIT - consulte o arquivo LICENSE para mais detalhes.

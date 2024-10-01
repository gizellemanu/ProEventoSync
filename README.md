<img align="right" height="30" width="40" src="https://www.svgrepo.com/show/508668/flag-us.svg" alt="English">

# ProEventoSync
## INTRODUCTION
<p style="text-align: justify;"><em>The ProEventos project was created to serve the event management sector. This repository presents the proposal for Front-End and Back-End for software designed to efficiently manage events such as conferences. The application’s Front-End was developed using Angular CLI (version >= 11.2.1), while the Back-End was built using C# and .NET, with the MySQL Server Express database.</em></p>

#### Completion Certificate
_This project was developed during the [Udemy](https://www.udemy.com/course/angular-dotnetcore-efcore/?utm_source=adwords&utm_medium=udemyads&utm_campaign=Angular_new_v.PROF_la.PT_cc.BR_ti.28016&campaigntype=Search&portfolio=Brazil&language=PT&product=Course&test=&audience=DSA&topic=&priority=&utm_content=deal4584&utm_term=_._ag_125593855828_._ad_658167638057_._kw__._de_c_._dm__._pl__._ti_dsa-1208106379807_._li_9101163_._pd__._&matchtype=&gad_source=1&gclid=CjwKCAjwvIWzBhAlEiwAHHWgvR0qg_-8gHWVcJa-msJdeLew6rm_wrc0B0bclkwZqUsOe7ikwpq79hoCnv0QAvD_BwE&couponCode=2021PM25) course, taught by [Vinícius de Andrade](https://www.udemy.com/user/vinicius-de-andrade/)._  
You can access the certificate directly [→ here ←](path/to/the/certificate.pdf).

## _Index_
- [_Project Features_](#project-features)
- [_How to Run the Project_](#how-to-run-the-project)
- [_Directory Structure_](#directory-structure)
- [_Authors_](#authors)

# _Project Features_
The application includes the following features:
- **1**. A Login Screen, containing a form with email and password fields.
  > - _The login form is only validated with the correctly filled fields._
  > - _The password must have 8 characters._
  > - _The speaker’s profile has three tabs: profile, speaker bio, and social networks._

- **2**. A Forgot Password Screen containing a simple form with the email field.
  > - _The Forgot Password form is only validated with the correctly filled email field._

- **3**. A top Menu with options for Dashboard, Events, Speakers, and Contact.

- **4**. A Speaker Registration Screen containing a form with name, company name, tax ID (CNPJ), and email fields.
  > - _The user registration form is only validated with the correctly filled fields._
  > - _The password must have 8 characters._
  > - _The password confirmation field also has validation; if the passwords do not match, registration is not possible._
  > - _The CNPJ must have 14 characters._

- **5**. An Event List Screen.
  > - _It has a search function by location, subject, or speaker._
  > - _You can collapse and expand the grid with the promotional images of already registered events._
  > - _You can edit or delete the desired event._

- **7**. An Event Registration Screen containing a form with event name, speaker, promotional image, social network, theme, location, time, date, attendee limit, and batch fields.
- **8**. An Event Edit Screen containing a form with the same fields as the Event Registration Screen.
- **9**. An Event Edit Screen containing a form with the same fields as the Event Registration Screen.

## _How to Run the Project_
Before using this application, you need to have Node.js and Angular CLI installed on your computer. This project was developed using Angular CLI version 11.2.1. Follow the steps below to install and configure the development environment:

#### Prerequisites
- Node.js (version >= 10.13.0)
- .NET (version >= 5.0.402)
- npm (version >= 6.11.0)
- Angular CLI (version >= 11.2.1)
- MySQL

### Installing Node.js
1. Go to the official Node.js website at [https://nodejs.org/en/download/](https://nodejs.org/en/download/).
2. Select the download option for your operating system.
3. Download and run the Node.js installer. Follow the installer instructions to complete the installation.

### Installing Angular CLI
1. Open your system's terminal.
2. Run the following command to install Angular CLI:
    ```bash
    npm install -g @angular/cli@11.2.1
    ```
3. Wait for the installation to complete.

### Installing Project Dependencies
1. **Clone the repository**:
    ```bash
    git clone https://github.com/your-username/your-repository.git
    ```

#### Running the Backend
1. **Navigate to the backend directory**:
    ```bash
    cd backend
    ```
2. **Start the backend server**:
    ```bash
    npm start
    ```
3. **Check the backend connection**:
   The server should be running at [http://localhost:3000/](http://localhost:3000/). You can verify if the backend is working properly by accessing this URL.

#### Running the Frontend
1. **Navigate to the frontend directory**:
    ```bash
    cd ProEventos/Front/ProEventos-App
    ```
2. **Install the frontend dependencies**:
    ```bash
    npm install
    ```
  After these commands, your project folder structure should look similar to this:
  ```plaintext
  ProEventos/
  ├── .vscode/
  ├── Back/
  ├── Front/
  │   └── ProEventos-App
  │       ├── e2e/
  │       ├── node_modules/
  │       ├── src/
  │       └── ...
  ├── .gitignore
  └── README.md
```

3. **Start the development server:**:
    ```bash
    ng serve
    ```

4. **Access the application**:
   Navigate to http://localhost:4200/. The application will reload automatically if you change any of the source files.


#### Running Frontend and Backend Together
**Start the backend**:
1. Make sure the backend server is running first. Navigate to the backend directory and run:
    ```bash
    cd ProEventos/Back/src
    npm start
    ```
**Start the Frontend**:
1. To start the development server, run:
    ```bash
    cd ProEventos/Front/ProEventos-App
    ng serve
    ```
2. Navigate to http://localhost:4200/. The application will automatically reload if you change any of the source files.

## _Directory Structure_
  ```plaintext
  ProEventos/
  ├── .vscode/
  │   ├──  launch.json
  │   └── tasks.json
  ├── Back/
  │   └── src
  │   │    ├──  ProEventos.API
  │   │    │     ├── bin/
  │   │    │     ├── Controllers/
  │   │    │     ├── Controllers/
  │   │    │     ├── Extensions/
  │   │    │     ├── Helpers/
  │   │    │     ├── Models/
  │   │    │     ├── obj/
  │   │    │     ├── Properties/
  │   │    │     ├── appsettings.Development.json
  │   │    │     ├── appsettings.json
  │   │    │     ├── ProEventos.API.csproj
  │   │    │     ├── Program.cs
  │   │    │     └── Startup.cs
  │   │    ├──  ProEventos.Application
  │   │    │     ├── bin/
  │   │    │     ├── Contratos/
  │   │    │     ├── Dtos/
  │   │    │     ├── Extensions/
  │   │    │     ├── Helpers/
  │   │    │     ├── obj/
  │   │    │     ├── AccountService.cs
  │   │    │     ├── EventoService.cs
  │   │    │     ├── LoteService.cs
  │   │    │     ├── PalestranteService.cs
  │   │    │     ├── ProEventos.Application.csproj
  │   │    │     ├── RedeSocialService.cs
  │   │    │     └── TokenService.cs
  │   │    ├──  ProEventos.Domain
  │   │    │     ├── bin/
  │   │    │     ├── Enum/
  │   │    │     ├── Identity/
  │   │    │     ├── obj/
  │   │    │     ├── Evento.cs
  │   │    │     ├── Lote.cs
  │   │    │     ├── Palestrante.cs
  │   │    │     ├── PalestranteEvento.cs
  │   │    │     ├── ProEventos.Domain.csproj
  │   │    │     └── RedeSocial.cs
  │   │    ├──  ProEventos.Persistence
  │   │    │     ├── bin/
  │   │    │     ├── Contextos/
  │   │    │     ├── Contratos/
  │   │    │     ├── Migrations/
  │   │    │     ├── Models/
  │   │    │     ├── obj/
  │   │    │     ├── EventoPersist.cs
  │   │    │     ├── GeralPersist.cs
  │   │    │     ├── LotePersist.cs
  │   │    │     ├── PalestrantePersist.cs
  │   │    │     ├── ProEventos.Persistence.csproj
  │   │    │     ├── RedeSocialPersist.cs
  │   │    │     └── UserPersist.cs
  │   │    ├──  global.json
  │   └──  └──  ProEventos.sln
  ├── Front/
  │   └── ProEventos-App
  │       ├── e2e/
  │       │   └── ...
  │       ├── node_modules/
  │       │   └── ...
  │       ├── src/
  │       │   ├── app/
  │       │   │   ├── components/
  │       │   │   │   ├── contatos/
  │       │   │   │   |   └── ...
  │       │   │   │   ├── dashboard/
  │       │   │   │   |   └── ...
  │       │   │   │   ├── eventos/
  │       │   │   │   |   └── ...
  │       │   │   │   ├── home/
  │       │   │   │   |   └── ...
  │       │   │   │   ├── palestrantes/
  │       │   │   │   |   └── ...
  │       │   │   │   ├── redesSociais/
  │       │   │   │   |   └── ...
  │       │   │   │   └── user/
  │       │   │   │       └── ...
  │       │   │   ├── guard/
  │       │   │   │   └── ...
  │       │   │   ├── helpers/
  │       │   │   │   └── ...
  │       │   │   ├── interceptors/
  │       │   │   │   └── ...
  │       │   │   ├── services/
  │       │   │   │   ├── account.service.ts
  │       │   │   │   ├── evento.service.ts
  │       │   │   │   ├── lote.service.ts
  │       │   │   │   ├── palestrante.service.ts
  │       │   │   │   └── redeSocial.service.ts
  │       │   │   ├── models/
  │       │   │   │   ├── identity/
  │       │   │   │   |   └── User.ts
  │       │   │   │   |   └── UserLogin.ts
  │       │   │   │   |   └── UserUpdate.ts
  │       │   │   │   ├── Evento.ts
  │       │   │   │   ├── Lote.ts
  │       │   │   │   ├── Pagination.ts
  │       │   │   │   ├── Palestrante.ts
  │       │   │   │   └── RedeSocial.ts
  │       │   │   ├── shared/
  │       │   │   │   ├── nav/
  │       │   │   │   └── ...
  │       │   │   │   └── titulo/
  │       │   │   │   └── ...
  │       │   │   ├── util/
  │       │   │   │   └── ...
  │       │   │   ├── app-routing.module.ts
  │       │   │   └── ...
  │       │   ├── assets/
  │       │   ├── environments/
  │       └── └── ...
  ├── .gitignore
  └── README.md
  ```

<br>
<hr>
<img align="right" height="30" width="40" src="https://www.svgrepo.com/show/405433/flag-for-flag-brazil.svg" alt="Portugues">

# ProEventoSync
## INTRODUÇÃO
<p style="text-align: justify;"><em>O projeto ProEventos foi criado para atender o setor de gestão de eventos. Este repositório apresenta a proposta de Front-End e Back-End para um software destinado a gerenciar eventos, como palestras, de maneira eficiente. O Front-End da aplicação foi desenvolvido com Angular CLI (versão >= 11.2.1), enquanto o Back-End foi construído usando C# e .NET, com o banco de dados MySQL Server Express.</em></p>

#### Certificado de Conclusão
_Este projeto foi desenvolvido durante o curso [Udemy](https://www.udemy.com/course/angular-dotnetcore-efcore/?utm_source=adwords&utm_medium=udemyads&utm_campaign=Angular_new_v.PROF_la.PT_cc.BR_ti.28016&campaigntype=Search&portfolio=Brazil&language=PT&product=Course&test=&audience=DSA&topic=&priority=&utm_content=deal4584&utm_term=_._ag_125593855828_._ad_658167638057_._kw__._de_c_._dm__._pl__._ti_dsa-1208106379807_._li_9101163_._pd__._&matchtype=&gad_source=1&gclid=CjwKCAjwvIWzBhAlEiwAHHWgvR0qg_-8gHWVcJa-msJdeLew6rm_wrc0B0bclkwZqUsOe7ikwpq79hoCnv0QAvD_BwE&couponCode=2021PM25), ministrado por [Vinícius de Andrade](https://www.udemy.com/user/vinicius-de-andrade/)._<br>
Você pode acessar o certificado diretamente [→ aqui ←](path/to/the/certificate.pdf).

## _Índice_
- [_Funcionalidades do Projeto_](#funcionalidades-do-projeto)
- [_Como Executar o Projeto_](#como-executar-o-projeto)
- [_Estrutura de Diretórios_](#estrutura-de-diretórios)
- [_Autores_](#autores)

# _Funcionalidades do Projeto_
A aplicação contém as seguintes funcionalidades:
- **1**. Uma Tela de Login, contendo um formulário com campos de email e senha.
  > - _O formulário de login só é validado com os campos preenchidos corretamente._
  > - _A senha deve conter 8 caracteres._
  > - _O perfil do usuario palestrante possui trêÊs guias: perfil, palestrante bio e redes sociais

- **2**. Uma Tela de Esqueci a Senha contendo um simples formulário com o campo de e-mail.
  > - _O formulário de Esqueci a Senha só é validado com o campo preenchido corretamente._

- **3**. Um Menu superior, contendo as opções Dashboard, Eventos, Palestrantes e Contanto

- **4**. Uma Tela de Cadastro de Palestrantes contendo um formulário com os campos de nome, nome da empresa, cnpj, e-mail.
  > - _O formulário de Cadastro de Usuário só é validado com os campos preenchidos corretamente._
  > - _A senha deve conter 8 caracteres._
  > - _No campo confirmação de senha, também possui validação, caso sejam divergentes não será possível o cadastro._
  > - _O cnpj deve conter 14 caracteres._

- **5**. Uma Tela de Listagem de Eventos.
  > - _Possui a funcionalidade de buscar um evento por localidade, assunto ou palestrante._
  > - _É possivel recolher e expandir o grid com as imagens de divulgação dos eventos já cadastrados._
  > - _É possivel editar ou excluir o evento desejado._

- **7**. Uma Tela de Cadastro de Evento, contendo um formulário com os campos nome do evento, responsável/palestrante, imagem de divulgação,  rede social, tema, local, hora, data, quantidade de pessoas e lote.
- **8**. Uma Tela de Cadastro de Eventos, contendo um formulário com os campos nome, responsável.
- **9**. Uma Tela de Edição de Eventos, contendo um formulário com os mesmos campos presentes no Cadastro de Evento.


## _Como Executar o Projeto_
Antes de utilizar esta aplicação, é necessário ter o Node.js e o Angular CLI instalados em seu computador. Este projeto foi desenvolvido usando Angular CLI versão 11.2.1. Siga os passos abaixo para instalar e configurar o ambiente de desenvolvimento:

#### Pré-requisitos
- Node.js (versão >= 10.13.0)
- .net (versão >= 5.0.402)
- npm (versão >= 6.11.0)
- Angular CLI (versão >= 11.2.1)
- MySQL

### Instalando o Node.js
1. Acesse o site oficial do Node.js em [https://nodejs.org/en/download/](https://nodejs.org/en/download/).
2. Selecione a opção de download correspondente ao seu sistema operacional.
3. Baixe e execute o instalador do Node.js. Siga as instruções do instalador para concluir a instalação.

### Instalando o Angular CLI
1. Abra o terminal do seu sistema operacional.
2. Execute o seguinte comando para instalar o Angular CLI:
    ```bash
    npm install -g @angular/cli@11.2.1
    ```
3. Aguarde o término da instalação. 

### Instalando Dependências do Projeto
1. **Clone o repositório**:
    ```bash
    git clone https://github.com/seu-usuario/seu-repositorio.git
    ```
#### Executando o Backend
1. **Navegar até o diretório do backend**:
    ```bash
    cd backend
    ```
2. **Iniciar o servidor backend**:
    ```bash
    npm start
    ```
3. **Verificar a conexão com o backend**:
   O servidor deve estar rodando em [http://localhost:3000/](http://localhost:3000/). Você pode verificar se o backend está funcionando corretamente acessando esta URL.

#### Executando o Frontend
1. **Navegar até o diretório do frontend**:
    ```bash
    cd ProEventos/Front/ProEventos-App
    ```
2. **Instalar as dependências do frontend**:
    ```bash
    npm install
    ```
  Após esses comandos, a estrutura de pastas do seu projeto deve ser semelhante a esta:
  ```plaintext
  ProEventos/
  ├── .vscode/
  ├── Back/
  ├── Front/
  │   └── ProEventos-App
  │       ├── e2e/
  │       ├── node_modules/
  │       ├── src/
  │       └── ...
  ├── .gitignore
  └── README.md
  ```
    
3. **Iniciar o servidor de desenvolvimento**:
    ```bash
    ng serve
    ```

4. **Acessar a aplicação**:
   Navegue para [http://localhost:4200/](http://localhost:4200/). A aplicação será recarregada automaticamente se você alterar qualquer um dos arquivos de origem.


#### Executando Frontend e Backend Juntos
**Iniciar o backend**:
1. Certifique-se de que o servidor backend está rodando primeiro. Navegue até o diretório do backend e execute:
    ```bash
    cd ProEventos/Back/src
    npm start
    ```
**Iniciar o Frontend**:
1. Para iniciar o servidor de desenvolvimento, execute:
    ```bash
    cd ProEventos/Front/ProEventos-App
    ng serve
    ```
2. Navegue para [http://localhost:4200/](http://localhost:4200/). A aplicação será recarregada automaticamente se você alterar qualquer um dos arquivos de origem.

## _Estrutura de Diretórios_
  ```plaintext
  ProEventos/
  ├── .vscode/
  │   ├──  launch.json
  │   └── tasks.json
  ├── Back/
  │   └── src
  │   │    ├──  ProEventos.API
  │   │    │     ├── bin/
  │   │    │     ├── Controllers/
  │   │    │     ├── Controllers/
  │   │    │     ├── Extensions/
  │   │    │     ├── Helpers/
  │   │    │     ├── Models/
  │   │    │     ├── obj/
  │   │    │     ├── Properties/
  │   │    │     ├── appsettings.Development.json
  │   │    │     ├── appsettings.json
  │   │    │     ├── ProEventos.API.csproj
  │   │    │     ├── Program.cs
  │   │    │     └── Startup.cs
  │   │    ├──  ProEventos.Application
  │   │    │     ├── bin/
  │   │    │     ├── Contratos/
  │   │    │     ├── Dtos/
  │   │    │     ├── Extensions/
  │   │    │     ├── Helpers/
  │   │    │     ├── obj/
  │   │    │     ├── AccountService.cs
  │   │    │     ├── EventoService.cs
  │   │    │     ├── LoteService.cs
  │   │    │     ├── PalestranteService.cs
  │   │    │     ├── ProEventos.Application.csproj
  │   │    │     ├── RedeSocialService.cs
  │   │    │     └── TokenService.cs
  │   │    ├──  ProEventos.Domain
  │   │    │     ├── bin/
  │   │    │     ├── Enum/
  │   │    │     ├── Identity/
  │   │    │     ├── obj/
  │   │    │     ├── Evento.cs
  │   │    │     ├── Lote.cs
  │   │    │     ├── Palestrante.cs
  │   │    │     ├── PalestranteEvento.cs
  │   │    │     ├── ProEventos.Domain.csproj
  │   │    │     └── RedeSocial.cs
  │   │    ├──  ProEventos.Persistence
  │   │    │     ├── bin/
  │   │    │     ├── Contextos/
  │   │    │     ├── Contratos/
  │   │    │     ├── Migrations/
  │   │    │     ├── Models/
  │   │    │     ├── obj/
  │   │    │     ├── EventoPersist.cs
  │   │    │     ├── GeralPersist.cs
  │   │    │     ├── LotePersist.cs
  │   │    │     ├── PalestrantePersist.cs
  │   │    │     ├── ProEventos.Persistence.csproj
  │   │    │     ├── RedeSocialPersist.cs
  │   │    │     └── UserPersist.cs
  │   │    ├──  global.json
  │   └──  └──  ProEventos.sln
  ├── Front/
  │   └── ProEventos-App
  │       ├── e2e/
  │       │   └── ...
  │       ├── node_modules/
  │       │   └── ...
  │       ├── src/
  │       │   ├── app/
  │       │   │   ├── components/
  │       │   │   │   ├── contatos/
  │       │   │   │   |   └── ...
  │       │   │   │   ├── dashboard/
  │       │   │   │   |   └── ...
  │       │   │   │   ├── eventos/
  │       │   │   │   |   └── ...
  │       │   │   │   ├── home/
  │       │   │   │   |   └── ...
  │       │   │   │   ├── palestrantes/
  │       │   │   │   |   └── ...
  │       │   │   │   ├── redesSociais/
  │       │   │   │   |   └── ...
  │       │   │   │   └── user/
  │       │   │   │       └── ...
  │       │   │   ├── guard/
  │       │   │   │   └── ...
  │       │   │   ├── helpers/
  │       │   │   │   └── ...
  │       │   │   ├── interceptors/
  │       │   │   │   └── ...
  │       │   │   ├── services/
  │       │   │   │   ├── account.service.ts
  │       │   │   │   ├── evento.service.ts
  │       │   │   │   ├── lote.service.ts
  │       │   │   │   ├── palestrante.service.ts
  │       │   │   │   └── redeSocial.service.ts
  │       │   │   ├── models/
  │       │   │   │   ├── identity/
  │       │   │   │   |   └── User.ts
  │       │   │   │   |   └── UserLogin.ts
  │       │   │   │   |   └── UserUpdate.ts
  │       │   │   │   ├── Evento.ts
  │       │   │   │   ├── Lote.ts
  │       │   │   │   ├── Pagination.ts
  │       │   │   │   ├── Palestrante.ts
  │       │   │   │   └── RedeSocial.ts
  │       │   │   ├── shared/
  │       │   │   │   ├── nav/
  │       │   │   │   └── ...
  │       │   │   │   └── titulo/
  │       │   │   │   └── ...
  │       │   │   ├── util/
  │       │   │   │   └── ...
  │       │   │   ├── app-routing.module.ts
  │       │   │   └── ...
  │       │   ├── assets/
  │       │   ├── environments/
  │       └── └── ...
  ├── .gitignore
  └── README.md
  ```

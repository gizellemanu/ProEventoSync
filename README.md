<img align="right" height="30" width="40" src="https://www.svgrepo.com/show/508668/flag-us.svg" alt="English">

# ProEventoSync

## Authors
```
Gizelle Emanuela da Silva
```

<br>
<hr>
<img align="right" height="30" width="40" src="https://www.svgrepo.com/show/405433/flag-for-flag-brazil.svg" alt="Portugues">

# ProEventoSync
## INTRODUÇÃO
<p style="text-align: justify;"><em>Named LAB Clothing Collection, the project aims to serve the fashion management sector, this repository presents the Back-End proposal for the software that aims to manage fashion collections and creation models in the clothing segment efficiently. This Back-End application was developed using C# and .NET utilizing the MySQL Server Express database.</em></p>

#### Completion Certificate
_This project was developed during the [Udemy](https://www.udemy.com/course/angular-dotnetcore-efcore/?utm_source=adwords&utm_medium=udemyads&utm_campaign=Angular_new_v.PROF_la.PT_cc.BR_ti.28016&campaigntype=Search&portfolio=Brazil&language=PT&product=Course&test=&audience=DSA&topic=&priority=&utm_content=deal4584&utm_term=_._ag_125593855828_._ad_658167638057_._kw__._de_c_._dm__._pl__._ti_dsa-1208106379807_._li_9101163_._pd__._&matchtype=&gad_source=1&gclid=CjwKCAjwvIWzBhAlEiwAHHWgvR0qg_-8gHWVcJa-msJdeLew6rm_wrc0B0bclkwZqUsOe7ikwpq79hoCnv0QAvD_BwE&couponCode=2021PM25) course, taught by [Vinícius de Andrade](https://www.udemy.com/user/vinicius-de-andrade/)._<br>
You can access the certificate directly [→ here ←](path/to/the/certificate.pdf).

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

- **2**. Uma Tela de Esqueci a Senha contendo um simples formulário com o campo de e-mail.
  > - _O formulário de Esqueci a Senha só é validado com o campo preenchido corretamente._

- **3**. Uma Tela de Cadastro de Palestrantes contendo um formulário com os campos de nome, nome da empresa, cnpj, e-mail.
  > - _O formulário de Cadastro de Usuário só é validado com os campos preenchidos corretamente._
  > - _A senha deve conter 8 caracteres._
  > - _No campo confirmação de senha, também possui validação, caso sejam divergentes não será possível o cadastro._
  > - _O cnpj deve conter 14 caracteres._

- **4**. Um Menu Lateral, contendo as opções .......

- **5**. Uma Tela de Dashboard.
  > - 

- **6**. Uma Tela de Listagem de Eventos.
  > - _._
  > - _._
  > - _._

- **7**. Uma Tela de Cadastro de Evento, contendo um formulário com os campos nome, responsável e hora e data.
  > - _._

- **8**. Uma Tela de Edição de Evento, contendo um formulário com os campos nome, responsável e hora e data.

- **9**. Uma Tela de Listagem de Eventos.
  > - _._
  > - _._
  > - _._

- **10**. Uma Tela de Cadastro de Eventos, contendo um formulário com os campos nome, responsável.

- **11**. Uma Tela de Edição de Eventos, contendo um formulário com os mesmos campos presentes no Cadastro de Evento.


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

## Autores
```
Gizelle Emanuela da Silva
```

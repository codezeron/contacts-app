# Contacts App

Este é um aplicativo de gerenciamento de contatos desenvolvido com Angular 17 no front-end e .NET 8 no back-end.

## Funcionalidades

- **Adicionar Contatos**: Formulário para adicionar novos contatos com nome, email, telefone e marcação de favorito.
- **Listar Contatos**: Exibição de todos os contatos salvos, mostrando nome, telefone e email.
- **Ligar para Contato**: Link direto para discar o telefone do contato.
- **Excluir Contatos**: Botão para remover contatos da lista.

## Tecnologias Utilizadas

- **Front-end**: Angular 17, TypeScript, Tailwind CSS
- **Back-end**: .NET 8 (ASP.NET Core Web API)

## Pré-requisitos

- Node.js (versão 18 ou superior)
- .NET 8 SDK
- Git

## Instalação e Inicialização

### 1. Clonagem do Repositório

```bash
git clone https://github.com/seu-usuario/contacts-app.git
cd contacts-app
```

### 2. Inicialização do Back-end (.NET 8)

Navegue até a pasta do back-end:

```bash
cd api/Contactly
dotnet restore
dotnet run
```

O servidor back-end será iniciado na porta 7158 (https://localhost:7158).

### 3. Inicialização do Front-end (Angular 17)

Navegue até a pasta do front-end:

```bash
cd ui/contactly.web
npm install
npm start
```

O aplicativo front-end será iniciado em http://localhost:4200.

### 4. Acesso ao Aplicativo

Abra o navegador e acesse http://localhost:4200 para usar o aplicativo.

Certifique-se de que ambos os servidores (back-end e front-end) estejam rodando simultaneamente.

## Estrutura do Projeto

```
contacts-app/
├── api/                    # Back-end .NET 8
├── ui/
│   └── contactly.web/      # Front-end Angular 17
│       ├── src/
│       │   ├── app/
│       │   │   ├── app.component.html
│       │   │   ├── app.component.ts
│       │   │   └── ...
│       │   └── models/
│       │       └── contact.model.ts
│       └── ...
└── README.md
```

## API Endpoints

- `GET /api/Contacts`: Lista todos os contatos
- `POST /api/Contacts`: Adiciona um novo contato
- `DELETE /api/Contacts/{id}`: Remove um contato pelo ID

## Desenvolvimento

Para desenvolvimento, execute os servidores em modo de desenvolvimento e faça alterações conforme necessário. O front-end usa Hot Module Replacement (HMR) para recarregamento automático.

## Contribuição

1. Fork o projeto
2. Crie uma branch para sua feature (`git checkout -b feature/nova-feature`)
3. Commit suas mudanças (`git commit -am 'Adiciona nova feature'`)
4. Push para a branch (`git push origin feature/nova-feature`)
5. Abra um Pull Request

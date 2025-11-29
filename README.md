# ApiEmpresas

API para cadastro de empresas e funcionários.

## Tecnologias Utilizadas

- C#
- .NET 8
- Entity Framework Core
- MySQL
- Swagger
- VSCODE

## Como Executar

1. **Clone o repositório:**

   ```bash
   git clone <url-do-repositorio>
   cd ApiEmpresas
   ```

2. **Configure o banco de dados:**

   - Certifique-se de ter o MySQL rodando na sua máquina.
   - Crie um banco de dados chamado `ApiEmpresasDb`.
   - A string de conexão no arquivo `appsettings.json` está configurada para:
     `"DefaultConnection": "Server=localhost;Port=3306;Database=ApiEmpresasDb;Uid=root;Pwd=12345678;"`
     Ajuste se necessário.

3. **Aplique as migrations:**

   ```bash
   dotnet ef database update
   ```

4. **Executar a aplicação:**

   ```bash
   dotnet run
   ```

5. **Passo-a-Passo se arquivo .zip:**
   1º primeiro descompacte, abra a pasta no vscode, abra o docker

   2º no windows explorer da pasta descompactada no caminho da url ditgite CMD preferencialmente modo administrador

   3º digite no CMD docker compose up --build
   depois de montada a imagem e conteinizar o servidor SQL (DEMORA UM POUCO)

   4º no VSCODE vá em Terminal (Ctl + " ) e digite: dotnet run

   5º Acesse Swagger UI
   http://localhost:5193/swagger/index.html

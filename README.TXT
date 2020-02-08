Criar api comandos dotnet
Criar pasta do projeto
dotnet new sln -n Api
dotnet new webapi -n Api -o Api.Application --no-https
dotnet sln add Api.Applicaiton
dotnet build

camadas 

dotnet new classlib -n Domain -f netcoreapp3.0 -o Api.Domain (Mudar o nome aqui para crosscutting, data, domain, service etc)
dotnet sln add Api.Domain
dotnet build
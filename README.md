Claro, aqui está a documentação no formato README com as informações fornecidas:

```markdown
# API-Rest-Netcon-dotnet

A API fornece um serviço simples de conversão de distâncias entre anos-luz e quilômetros. Ela permite que os usuários convertam distâncias de anos-luz para quilômetros e vice-versa usando o método GET.

## Recursos

- **Swagger**: Uma interface interativa para explorar e testar a API.
  - Acesse em `https://localhost:[porta]/swagger`.
- **Testes Unitários (NUnit)**

## Parâmetros na URL

- `km` (float):
- `anosLuz` (float)

## Exemplo de Uso

### URL de Requisição:

```
https://localhost:7119/api/converter?km=2
```

### Resultado:

```json
{
  "date": "2023-10-26T14:25:15.8575587-03:00",
  "statusCode": 200,
  "errorMessage": null,
  "value": 2.114e-13
}
```

### URL de Requisição:

```
https://localhost:7119/api/converter?km=0.5
```

### Resultado:

```json
{
  "date": "2023-10-26T14:27:10.0685161-03:00",
  "statusCode": 400,
  "errorMessage": "Valor inválido. O valor não pode ser < 1.",
  "value": 0
}
```

## Como Compilar e Executar

1. Abra o diretório "API Rest Netcon dotnet".

2. Execute:

```bash
dotnet run
```

3. Acesse a URL do Swagger:

```bash
https://localhost:[porta]/swagger
```

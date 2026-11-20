<<<<<<< HEAD
# SistemaInscricaoCursosBlazor

Projeto acadêmico de uma página interativa de inscrição em cursos, desenvolvido com Blazor Web App e C#.

## Requisitos

- .NET 8 SDK ou superior
- Visual Studio 2022 ou VS Code
- Navegador atualizado
- Git (para publicar no GitHub)

Confira a instalação do .NET com:

```bash
dotnet --version
```

## Como executar

1. Extraia o arquivo ZIP.
2. Abra a pasta `SistemaInscricaoCursosBlazor` no VS Code ou terminal.
3. Execute:

```bash
dotnet restore
dotnet watch run
```

4. O terminal exibirá o endereço local. Abra-o no navegador e acesse `/inscricao`.

## Funcionalidades implementadas

- Formulário com nome, e-mail, idade e curso.
- Validação com DataAnnotations:
  - Nome obrigatório (entre 2 e 100 caracteres).
  - E-mail obrigatório e validado com `[EmailAddress]`.
  - Idade obrigatória, entre 16 e 100 anos, com `[Range(16, 100)]`.
  - Curso obrigatório.
- `EditForm` com `FormName="InscricaoForm"`.
- Modelo recebido por `[SupplyParameterFromForm]`.
- `DataAnnotationsValidator`, `ValidationSummary` e `ValidationMessage`.
- `InputSelect` com três cursos e uma opção inicial vazia.
- Envio assíncrono simulado com `Task.Delay(2000)`.
- Botão desabilitado durante o envio e texto dinâmico.
- Mensagem de sucesso após o processamento.

## Testes solicitados

1. **Submissão vazia:** deixe todos os campos em branco e clique em Confirmar inscrição. As mensagens de obrigatoriedade devem aparecer.
2. **Dados inválidos:** informe um e-mail sem `@` e/ou idade menor que 16 ou maior que 100. O formulário deve impedir o envio e apresentar as mensagens correspondentes.
3. **Preenchimento correto:** informe nome, e-mail válido, idade entre 16 e 100 e selecione um curso. Ao enviar, o botão deve mostrar “Processando...” e ficar desabilitado por aproximadamente 2 segundos. Depois, deve aparecer a confirmação de sucesso.

## Publicar no GitHub

Na página do GitHub, crie um repositório chamado `sistema-inscricao-cursos-blazor`. Depois, na raiz do projeto, execute:

```bash
git init
git add .
git commit -m "Projeto de inscrição em cursos com Blazor"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/sistema-inscricao-cursos-blazor.git
git push -u origin main
```

Substitua `SEU-USUARIO` pelo seu usuário do GitHub.

## Observação

O `Task.Delay(2000)` simula o tempo de uma requisição assíncrona. O projeto não grava os dados em banco de dados nem envia e-mail; isso não foi solicitado no enunciado.
=======
# sistema-inscricao-cursos-blazor
>>>>>>> 4f33e8e533209ac5cad4688c824cc1b8f1bf3dc5

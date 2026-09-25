# n8n Product Category Router

Workflow desenvolvido em n8n para processamento de dados enviados por formulário, classificação de produtos por categoria e geração de arquivos.

## 🚀 Sobre o projeto

O workflow recebe informações de um produto através de um formulário:

- Nome
- Preço
- Categoria

Após o envio, o fluxo verifica o preço do produto e, de acordo com as condições definidas, direciona os dados para diferentes etapas de processamento.

## 🔄 Fluxo

```text
Formulário
    ↓
IF — verifica o preço
    ↓
Switch — identifica a categoria
    ├── Eletronicos
    ├── Roupas
    ├── Comida
    └── Outros
         ↓
   Convert to File
         ↓
   Write File to Disk
# Sistema-de-Manutencao-de-Contas
# Sistema de Manutenção de Contas em C

Este projeto foi desenvolvido em linguagem C com o objetivo de praticar manipulação de arquivos binários, utilizando funções como `fseek()`, `fread()`, `fwrite()` e `rewind()`.

O sistema simula um pequeno cadastro bancário, permitindo armazenar clientes em um arquivo binário com registros de tamanho fixo.

## Funcionalidades

O programa possui um menu com as seguintes opções:

1. Cadastrar um novo cliente em uma posição específica do arquivo
2. Consultar cliente pelo número da conta
3. Atualizar saldo de um cliente
4. Encerrar conta
5. Listar todos os clientes cadastrados
6. Reiniciar a leitura do arquivo usando `rewind()`
7. Encerrar o programa

## Estrutura do Registro

Cada cliente possui:

* Número da conta
* Nome
* Saldo
* Status da conta (ativa ou removida)

Os dados são armazenados em um arquivo binário chamado:

```text
clientes.dat
```

## Conceitos utilizados

Durante o desenvolvimento foram utilizados:

* Structs
* Arquivos binários
* Manipulação de registros fixos
* `fseek()`
* `fread()`
* `fwrite()`
* `rewind()`
* Menu interativo com `switch`

## Compilação

Para compilar:

```bash
gcc main.c -o sistema
```

## Execução

Para executar:

```bash
./sistema
```

## Observação

As contas removidas não são apagadas fisicamente do arquivo. O sistema apenas marca o registro como inativo.

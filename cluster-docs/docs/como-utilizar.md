# Como utilizar

## Solicitar acesso

Envie e-mail para:

`solicitacao.cluster@ufpr.edu.br`

Informando:

- Grupo de pesquisa
- Necessidade
- Nome dos pesquisadores
- E-mails dos pesquisadores

---

## Acesso

As instruções de acesso ao cluster são enviadas via e-mail, após o cadastro

## Organização de diretórios

Cada projeto de pesquisa está organizado no cluster da seguinte maneira:

```
/projetos/<projeto>/<membro>
```

Cada membro do grupo de pesquisa possui um diretório seu dentro do diretório do projeto. 

**Exemplo**
Considere o projeto `hidro`, que possui os membros `joao.santos` e `maria.souza`. Desta forma, a estrutura seria a seguinte:

```text
/projetos/
└── hidro/
    ├── joao.santos/
    └── maria.souza/
```

tanto `joao.santos` quanto `maria.souza` possuem acesso de **leitura** ao diretório dos outros membros do grupo. Porém, as permissões de escrita existem apenas nos diretórios dos próprios usuários.

## Slurm

O gerenciamento de execução das tarefas no cluster é realizado pela ferramenta `Slurm`.

### Filas

Para a execução, diferentes filas podem ser utilizadas. Estas são:

- `debug`: testes rápidos
- `short`: execuções curtas
- `long`: execuções longas
- `max`: execuções sem limite rígido

---

## Exemplo

```bash
#!/bin/bash
#SBATCH --job-name=teste
#SBATCH --output=saida.txt
#SBATCH --partition=debug

echo "Executando"
```

```bash
sbatch job.sh
```


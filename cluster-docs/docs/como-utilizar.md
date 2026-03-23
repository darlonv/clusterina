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

## Filas

- debug: testes rápidos
- short: execuções curtas
- long: execuções longas
- max: execuções sem limite rígido

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


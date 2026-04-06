# Cluster HPC — UFPR Campus Palotina

Bem-vindo à documentação oficial do **Cluster de Computação de Alto Desempenho (HPC)** da Universidade Federal do Paraná — Campus Palotina.

Esta plataforma é um recurso institucional dedicado à pesquisa científica, ao ensino e ao desenvolvimento de projetos que demandam processamento computacional intensivo.

## O que você encontra aqui

- [**Sobre**](sobre.md) — histórico, arquitetura e finalidade do cluster
- [**Arquitetura**](arquitetura.md) — especificações técnicas detalhadas dos nós
- [**Ferramentas**](ferramentas.md) — MPI, OpenMP, PLUTO e demais softwares disponíveis
- [**Como utilizar**](como-utilizar.md) — organização de diretórios, Slurm e exemplos práticos
- [**Solicitar Acesso**](solicitar-acesso.md) — procedimento para cadastro de projetos e usuários
- [**Grupos de Pesquisa**](grupos-pesquisa.md) — grupos que utilizam a infraestrutura
- [**Publicações**](publicacoes.md) — trabalhos produzidos com o apoio do cluster

## Início rápido

```bash
# Acesso via SSH (após cadastro)
ssh usuario@hpc.palotina.ufpr.br

# Consultar seus projetos
meus-projetos

# Submeter um job de teste
sbatch meu_job.sh

# Acompanhar a fila
squeue -u $USER
```

## Suporte

Em caso de dúvidas técnicas ou problemas de acesso, entre em contato com a equipe de administração:

**E-mail:** `hpc-admin@palotina.ufpr.br`

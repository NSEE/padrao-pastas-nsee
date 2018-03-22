# Padrão de pastas

## Descrição
Padronização de pastas para os projetos desenvolvidos no NSEE, para usar basta:

Qualquer dúvida, favor contactar:

Rodrigo França - rodrigo.franca@maua.br

## Organização das pastas

As pastas desse projeto devem ser organizadas conforme exemplo a seguir:

- Como : Toda documentação gerada e coletada que pode ser usada para compreenção e descrição do projeto

- Materiais : Todo formato de material desenvolvido no projeto, inclui softwares, esquemáticos, fotos, etc..

Árvore de arquivos :
```
├── Como
│   ├── Apresentações
│   ├── Datasheets
│   ├── Estudos
│   ├── Manuais
│   ├── Referências
│   │   └── Artigos
│   │       └── Bibliografia
│   └── Wiki
├── Materiais
│   ├── Arquivos
│   │   └── Orçamentos
│   ├── Códigos
│   │   ├── Altera
│   │   ├── Arduino
│   │   ├── Atmel
│   │   ├── C
│   │   ├── Comsol
│   │   ├── Labview
│   │   ├── Matlab
│   │   └── Xilinx
│   ├── Fotos
│   ├── Mecânica
│   └── PCB

```

## Exemplo de como usar

- Criar pasta do projeto (vazia)
- Clonar esse repositório para a pasta recente criada
- Adicionar arquivos 
- Adicionar o novo repositório remote
- Dar um push para o repositório

Criamos uma nova pasta do projeto:

```
--- ~ » mkdir novo_projeto
--- ~ » cd novo_projeto 
```

inicializamos um novo repositório, associamos o remoto com o link do rep. e atualizamos a pasta:

```
--- ~/novo_projeto » git init
Initialized empty Git repository in /home/corsi/novo_projeto/.git/
--- ~/novo_projeto ‹master› » git remote add origin https://github.com/corsiferrao/padrao-pastas-nsee
--- ~/novo_projeto ‹master› » git fetch
remote: Counting objects: 11, done.
remote: Compressing objects: 100% (6/6), done.
remote: Total 11 (delta 0), reused 11 (delta 0), pack-reused 0
Unpacking objects: 100% (11/11), done.
From https://github.com/corsiferrao/padrao-pastas-nsee
 * [new branch]      master     -> origin/master
```

Nessa etapa, alteramos o caminho do diretório remoto para o novo projeto:

```
--- ~/novo_projeto ‹master› » git remote set-url origin https://github.com/corsiferrao/novo-projeto
```

crio um novo objeto e atualizo o rep. remoto

```
--- ~/novo_projeto ‹master› » touch Como/EXEMPLO.TXT
--- ~/novo_projeto ‹master* ?› » git add 
--- ~/novo_projeto ‹master* A› » git commit -a -m "primeiro commit"
--- ~/novo_projeto ‹master➔› » git push origin master 
Username for 'https://github.com': corsiferrao
Password for 'https://corsiferrao@github.com': 
```


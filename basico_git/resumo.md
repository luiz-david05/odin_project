Git é como realmente um épico botão de save para os seus arquivos e diretórios. Oficialmente, Git é um sistema de controle de versão distribuído, ou seja, um sistema que registra alterações em um arquivo ou conjunto de arquivos ao longo do tempo de forma que você possa recuperar versões específicas mais tarde.


Git != GitHub

GitHub é um serviço de hospedagem de código-fonte com controle de versão usando o Git. Ele permite que programadores, utilitários ou qualquer usuário cadastrado na plataforma contribuam em projetos privados e/ou Open Source de qualquer lugar do mundo.


## Instalação

### Linux

#### Debian/Ubuntu

```bash
sudo apt-get install git
```

## Clonando um repositório

```bash
git clone link_do_repositorio
```

## Criando um repositório

```bash
git init
```

## Adicionando arquivos

```bash 
git add nome_do_arquivo
```

## Adicionando todos os arquivos

```bash
git add .
```

## Adicionando uma mensagem de commit

```bash
git commit -m "mensagem"
```

## Enviando para o repositório remoto

```bash
git push origin master
```
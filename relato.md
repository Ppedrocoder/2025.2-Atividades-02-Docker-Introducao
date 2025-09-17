# Atividade: Introdução ao Docker
**Nome:** [Pedro Ricardo]
**Data:** 15/09/2025

## Introdução
O objetivo deste exercício é compreender os conceitos básicos do Docker, incluindo a criação de containers, manipulação de imagens e execução de comandos essenciais para o desenvolvimento de aplicações em ambientes isolados.

## Relato
Durante a atividade, realizei os seguintes passos:

### 2.2.1. Iniciando o contêiner Fedora

Comando utilizado para baixar a imagem do Fedora e iniciar um contêiner interativo:

```bash
docker run -it --name fedora-tutorial fedora:latest /bin/bash
```

### 2.2.2. Navegação básica

```bash
pwd
cd ~
ls
mkdir atividades
cd atividades
cd ..
```

---

### 2.2.3. Manipulação de arquivos

```bash
cd ~
pwd
touch arquivo1.txt
mv arquivo1.txt documento.txt
cd atividades
mkdir backup
cp ~/documento.txt backup/
ls backup/
cd ~
pwd
rm documento.txt
ls atividades/backup/
```

---

### 2.2.4. Gerenciamento de pacotes

```bash
dnf update -y
dnf install nano -y
nano --version
dnf remove nano -y
```

---

### 2.2.5. Permissões de arquivos

```bash
touch script.sh
ls -l script.sh
chmod u+x script.sh
ls -l script.sh
```

---

### 2.2.6. Processos em execução

```bash
ps aux
sleep 60 &
ps aux | grep sleep
kill <PID>
```

---

### 2.2.7. Encerrando o contêiner

```bash
exit
docker rm fedora-tutorial
```

---

## Conclusão
Durante a atividade, aprendi a manipular arquivos, diretórios, permissões e processos dentro de um contêiner Linux, além de instalar/remover pacotes. As principais dificuldades foram entender a diferença entre caminhos absolutos e relativos, e lidar com permissões de arquivos. O uso do Docker facilitou a experimentação sem afetar o sistema principal.



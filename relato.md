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
![docker run](imagens/Primeira parte 1.png)

### 2.2.2. Navegação básica


```bash
pwd
```
![pwd](imagens/Primeira parte 2.png)

```bash
cd ~
```
![cd home](imagens/Primeira parte 3.png)

```bash
ls
```
![ls](imagens/Primeira parte 4.png)

```bash
mkdir atividades
```
![mkdir atividades](imagens/Primeira parte 5.png)

```bash
cd atividades
```
![cd atividades](imagens/Primeira parte 6.png)

```bash
cd ..
```
![cd ..](imagens/Primeira parte 7.png)

---

### 2.2.3. Manipulação de arquivos


```bash
cd ~
```
![cd home 2](imagens/Segunda Parte 1.png)

```bash
pwd
```
![pwd 2](imagens/Segunda Parte 2.png)

```bash
touch arquivo1.txt
```
![touch arquivo1.txt](imagens/Segunda Parte 3.png)

```bash
mv arquivo1.txt documento.txt
```
![mv arquivo1.txt documento.txt](imagens/Segunda Parte 4.png)

```bash
cd atividades
```
![cd atividades 2](imagens/Segunda Parte 5.png)

```bash
mkdir backup
```
![mkdir backup](imagens/Segunda Parte 6.png)

```bash
cp ~/documento.txt backup/
```
![cp documento.txt backup](imagens/Segunda Parte 7.png)

```bash
ls backup/
```
![ls backup](imagens/Segunda Parte 8.png)

```bash
cd ~
```
![cd home 3](imagens/Segunda Parte 9.png)

```bash
pwd
```
![pwd 3](imagens/Segunda Parte 10.png)

```bash
rm documento.txt
```
![rm documento.txt](imagens/Segunda Parte 11.png)

```bash
ls atividades/backup/
```
![ls atividades backup](imagens/Segunda Parte 12.png)

---

### 2.2.4. Gerenciamento de pacotes


```bash
dnf update -y
```
![dnf update](imagens/Terceira parte 1.png)

```bash
dnf install nano -y
```
![dnf install nano](imagens/Terceira parte 2.png)

```bash
nano --version
```
![nano --version](imagens/Terceira parte 3.png)

```bash
dnf remove nano -y
```
![dnf remove nano](imagens/Terceira parte 4.png)

---

### 2.2.5. Permissões de arquivos


```bash
touch script.sh
```
![touch script.sh](imagens/Quarta parte 1.png)

```bash
chmod u+x script.sh
```
![chmod script.sh](imagens/Quarta parte 2.png)

```bash
ls -l script.sh
```
![ls -l script.sh depois](imagens/Quarta parte 3.png)

---

### 2.2.6. Processos em execução


```bash
ps aux
```
![ps aux](imagens/Quinta parte 1.png)

```bash
sleep 60 &
```
![sleep 60](imagens/Quinta parte 2.png)

```bash
ps aux | grep sleep
```
![ps aux grep sleep](imagens/Quinta parte 3.png)

```bash
kill <PID>
```
![kill PID](imagens/Quinta parte 4.png)

---

### 2.2.7. Encerrando o contêiner


```bash
exit
```
![exit](imagens/Sexta parte 1.png)

```bash
docker rm fedora-tutorial
```
![docker rm fedora-tutorial](imagens/Sexta parte 2.png)

---

## Conclusão
Durante a atividade, aprendi a manipular arquivos, diretórios, permissões e processos dentro de um contêiner Linux, além de instalar/remover pacotes. As principais dificuldades foram entender como de fato alguns comando funcionavam e o impacto deles.



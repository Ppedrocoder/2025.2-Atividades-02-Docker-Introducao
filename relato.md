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
![docker run](imagens/primeiraparte1.png)

### 2.2.2. Navegação básica


```bash
pwd
```
![pwd](imagens/primeiraparte2.png)

```bash
cd ~
```
![cd home](imagens/primeiraparte3.png)

```bash
ls
```
![ls](imagens/primeiraparte4.png)

```bash
mkdir atividades
```
![mkdir atividades](imagens/primeiraparte5.png)

```bash
cd atividades
```
![cd atividades](imagens/primeiraparte6.png)

```bash
cd ..
```
![cd ..](imagens/primeiraparte7.png)

---

### 2.2.3. Manipulação de arquivos


```bash
cd ~
```
![cd home 2](imagens/segundaparte1.png)

```bash
pwd
```
![pwd 2](imagens/segundaparte2.png)

```bash
touch arquivo1.txt
```
![touch arquivo1.txt](imagens/segundaparte3.png)

```bash
mv arquivo1.txt documento.txt
```
![mv arquivo1.txt documento.txt](imagens/segundaparte4.png)

```bash
cd atividades
```
![cd atividades 2](imagens/segundaparte5.png)

```bash
mkdir backup
```
![mkdir backup](imagens/segundaparte6.png)

```bash
cp ~/documento.txt backup/
```
![cp documento.txt backup](imagens/segundaparte7.png)

```bash
ls backup/
```
![ls backup](imagens/segundaparte8.png)

```bash
cd ~
```
![cd home 3](imagens/segundaparte9.png)

```bash
pwd
```
![pwd 3](imagens/segundaparte10.png)

```bash
rm documento.txt
```
![rm documento.txt](imagens/segundaparte11.png)

```bash
ls atividades/backup/
```
![ls atividades backup](imagens/segundaparte12.png)

---

### 2.2.4. Gerenciamento de pacotes


```bash
dnf update -y
```
![dnf update](imagens/terceiraparte1.png)

```bash
dnf install nano -y
```
![dnf install nano](imagens/terceiraparte2.png)

```bash
nano --version
```
![nano --version](imagens/terceiraparte3.png)

```bash
dnf remove nano -y
```
![dnf remove nano](imagens/terceiraparte4.png)

---

### 2.2.5. Permissões de arquivos


```bash
touch script.sh
```
![touch script.sh](imagens/quartaparte1.png)

```bash
chmod u+x script.sh
```
![chmod script.sh](imagens/quartaparte2.png)

```bash
ls -l script.sh
```
![ls -l script.sh depois](imagens/quartaparte3.png)

---

### 2.2.6. Processos em execução


```bash
ps aux
```
![ps aux](imagens/quintaparte1.png)

```bash
sleep 60 &
```
![sleep 60](imagens/quintaparte2.png)

```bash
ps aux | grep sleep
```
![ps aux grep sleep](imagens/quintaparte3.png)

```bash
kill <PID>
```
![kill PID](imagens/quintaparte4.png)

---

### 2.2.7. Encerrando o contêiner


```bash
exit
```
![exit](imagens/sextaparte1.png)

```bash
docker rm fedora-tutorial
```
![docker rm fedora-tutorial](imagens/sextaparte2.png)

---

## Conclusão
Durante a atividade, aprendi a manipular arquivos, diretórios, permissões e processos dentro de um contêiner Linux, além de instalar/remover pacotes. As principais dificuldades foram entender como de fato alguns comando funcionavam e o impacto deles.



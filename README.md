# Quiz 2 Resolução

### Git

**1. Qual o comando utilizado para associar um repositório local a um remoto? (0,5 val)**  
a) **git remote add origin**  
b) git connect remote  
c) git attach origin  
d) git link origin  

---

**2. Qual dos seguintes estados de ficheiros indica que o Git ainda não está a monitorizar um ficheiro? (0,5 val)**  
a) Modified  
b) Staged  
**c) Untracked**  
d) Committed  

---

**3. Qual o comando utilizado para criar um novo repositório Git numa pasta local? (0,5 val)**  
a) git create  
**b) git init**  
c) git new  
d) git start  

---

**4. O que se utiliza para definir os ficheiros que devem ser ignorados pelo Git? (0,5 val)**  
a) git exclude  
b) git track --ignore  
**c) git add .gitignore**  
d) git create .ignore  

---

**5. Qual o comando utilizado para obter as últimas alterações do repositório remoto sem actualizar o repositório local? (0,5 val)**  
**a) git fetch**  
b) git pull  
c) git sync  
d) git merge  

---

**6. Qual o comando correto para modificar o nome de uma branch existente em Git? (0,5 val)**  
a) git branch -r [new-name]  
b) git rename branch [new-name]  
c) git branch --rename [new-name]  
**d) git branch -M [new-name]**  

---

**7. Qual é o comando usado para verificar o estado atual do repositório? (0,5 val)**  
a) git verify  
b) git check  
**c) git status**  
d) git inspect  

---

**8. Qual o comando utilizado para reordenar commits sem criar commits de merge? (0,5 val)**  
**a) git rebase**  
b) git reorder  
c) git merge --nocommit  
d) git rebase --merge  

---

**9. O que acontece ao executar a seguinte sequência de comandos no terminal Git? (0,5 val)**  
```
echo "Hello World" > file.txt  
git add file.txt  
git commit -m "text commit"  
git log --pretty=format:"%h - %an, %ar : %s"
```
**a) Cria um novo ficheiro, faz staging e commit, exibindo o log num formato reduzido.**   
b) Cria um novo ficheiro, adiciona e faz commit de um ficheiro, mas o log só mostrará commits de branches secundários.   
c) O comando git log falha porque ainda não há commits suficientes para gerar um histórico.   
d) O ficheiro file.txt é adicionado ao staging, mas o commit e o log só são aplicáveis se o ficheiro for enviado para o repositório remoto   

---

10. Qual o resultado dos seguintes comandos? (0,5 val)

```
git branch feature  
git switch feature  
echo "Nova funcionalidade" > feature.txt  
git add feature.txt  
git commit -m "Adiciona nova funcionalidade"  
git checkout main  
git merge feature
```
a) O Git criará um novo commit no branch main, mas o ficheiro feature.txt não será incluído até ser sincronizado com o repositório remoto.   
b) O merge falhará a menos que o ficheiro feature.txt seja movido manualmente para o branch main antes do merge.   
**c) As alterações do branch feature serão integradas ao main, mas o branch feature permanecerá intacto até ser excluído.**   
d) As alterações feitas em feature.txt serão descartadas após o merge, e o ficheiro permanecerá apenas no branch feature.   

---

11. O que ocorre ao executar estes comandos após clonar um repositório? (0,5 val)

```
git branch feature  
git switch feature  
echo "Nova funcionalidade" > feature.txt  
git add feature.txt  
git commit -m "Adiciona nova funcionalidade"  
git checkout main  
git merge feature
```

a) O commit será rejeitado pelo repositório remoto porque um pull foi executado antes de modificar o ficheiro update.txt.   
**b) O push falhará se houver commits no repositório remoto não incluídos no pull anterior.**   
c) O ficheiro update.txt será enviado para o repositório remoto, mas o histórico de commits locais será mantido separado.   
d) O comando git push sobrescreverá o conteúdo do repositório remoto, criando um novo commit com todas as alterações locais.   

---

12. Qual é o efeito da seguinte sequência de comandos? (0,5 val)

```
git rebase main  
git add .  
git rebase --continue
```

**a) O histórico de commits será reorganizado, aplicando as alterações do branch atual após o commit mais recente do main, mas novos conflitos podem surgir.**   
b) Todos os commits no branch main serão integrados ao branch atual, mas as alterações do branch atual serão preservadas no final do histórico.   
c) As alterações do branch atual serão movidas para o início do histórico, e o git rebase --continue faz skip na resolução de conflitos pendentes.   
d) O branch atual será rebaseado no main, mas apenas os commits não compartilhados serão reescritos, ignorando alterações recentes.

---

**13. Preencha o comando correto para adicionar um ficheiro ao staging e fazer commit: (0,5 val)**  

```
git add file.txt  
git commit -m “Adiciona o ficheiro file.txt”
```
---

**14. Complete a sequência de comandos para apagar uma branch local e remota: (1 val)**  

```
git branch -d feature-branch  
git push origin --delete feature-branch
```
---

**15. Preencha os comandos corretos para fazer o merge de alterações da branch bugfix com a branch main e atualizar o repositório remoto: (1 val)**  

```
git checkout main  
git merge bugfix  
git push (-u) origin main #(-u opcional)

```
---

**16. Complete a sequência de comandos para criar um repositório local, adicioná-lo ao GitHub e fazer push do conteúdo: (1,5 val)**  

```
git init
git add .  
git commit -m “First commit”  
git remote add origin https://github.com/exemplo/repo.git  
git push -u origin main
```

---

### Markdown e Mermaid

---

17.	Qual o comando correto para definir um título de nível 1 no Markdown? (0,5 val)   
a)	`## Título`   
**b)	`# Título`**   
c)	`### Título`  
d)	`- Título   `

---

18.	Como se insere um texto em bold no Markdown? (0,5 val)   
**a)	`**texto em bold**`**   
b)	`*texto em bold*`   
c)	`~~texto em bold~~`   
d)	`>>texto em bold<<`   

---

19.	Qual a sintaxe correta para adicionar um link no Markdown? (0,5 val)   
**a)	`[texto](URL)`**   
b)	`[URL](<texto>)`   
c)	`![texto](URL)`   
d)	`[URL](texto)`

---

20.	Como se cria uma lista não ordenada no Markdown? (0,5 val)   
a)	`> Item 1`   
    `> Item 2`   
b)	`1. Item 1`   
    `2. Item 2`   
**c)	`* Item 1`**   
    **`* Item 2`**   
d)	`# Item 1`  
    `# Item 2`

---

21.	Qual destes se refere a um bloco de código Mermaid no Markdown? (0,5 val)   
a)	```flowchart (...)```  
**b)	```mermaid (...)```**  
c)	```diagram (...)```  
d)	```code mermaid (...)```

---

22.	Qual é a sintaxe correta para criar um nó de decisão num fluxograma Mermaid? (0,5 val)   
a)	A(Decisão)  
b)	A((Decisão))  
c)	**A{Decisão}**  
d)	A[Decisão]  

---

23.	Qual é a sintaxe correta para criar uma decisão num fluxograma Mermaid? (0,5 val)  
a)	A -- Sim --> B -- Não --> C  
b)	A -- Sim --> B    
    B -- Não --> C   
c)	**A -- Sim --> B   
    A -- Não --> C**   
d)	A -->> B -->> C

---

24.	Como se define um nó com cantos arredondadas num diagrama Mermaid? (0,5 val)   
a)	[Texto]   
**b)	(Texto)**   
c)	((Texto))  
d)	{Texto}

---

### Git, Markdown e Mermaid
25.	Exercício prático

A partir de um repositório existente no GitHub de um grupo de trabalho, desenvolva um documento semelhante ao fornecido, escrevendo todo o código em Markdown e Mermaid.

Todos os passos de execução:

### No Git Bash:

**Criar uma instância local do repositório remoto**
```
git clone https://github.com/exemplo/repo.git
```
ou
```
git init
git remote add origin https://github.com/exemplo/repo.git
git branch -M main # Se a branch default for 'master' 
git pull origin main
```
---

**Criação e utilização de branch**

```
git branch [new_doc_branch]
git switch [new_doc_branch]
```
---

Código Markdown e Mermaid

### No Visual Studio Code:

**Jogo: This War of Mine**
```
# This War of Mine

**Developer** *and publisher* : 11 bit studios   
~~**Publisher**: 11 bit studios~~   
**Release Year**: 2014

## Introduction

*This War of Mine* is a war survival video game where players control a group of civilians trying to survive in a besieged city. The game focuses on managing resources, making moral decisions, and ensuring the survival of the group amidst war-time challenges.

![This War of Mine cover](Images/thiswarofmine_cover.jpg)

> *In modern war... you die like a dog for no good reason*
> 
> Ernest Hemingway

---

## Gameplay Overview

### Key Features
* **Survival**: Manage hunger, health, and morale of your group.
* **Crafting**: Build tools, medicine, and defenses.
* **Scavenging**: Go out at night to search for food and materials.
* **Shelter Management**: Improve and maintain your shelter to protect the group.

--- 

## Gameplay Loop

```mermaid
flowchart TB
    A[Daytime] --> B[Manage Resources]
    A --> C[Manage Characters]
    B --> D{Enough Suplies?}
    D -- No --> E[Night Scavenging]
    D -- Yes --> F[Rest]
    D -- No --> G[Find Alternatives] --> H[Trade or ask for help]
    H --> F
    E --> I{Safe Return?}
    I -- Yes --> F
    I -- No --> J[Face consequences] --> F
    F -.-> A
```(ignorar este texto)
---

## External Resources

For more detailed guides and strategies, visit the following:
* [Official Website](https://www.11bitstudios.com/this-war-of-mine)

![Official Logo](Images/thiswarofmine_logo.jpg)
```

**Jogo: Bioshock**
```
# Bioshock
**Developer** ~~**and publisher**~~ : Irrational Games   
**Publisher**: 2K Games  
**Release Year**: 2007

## Introduction
**Bioshock** is a first-person shooter video game set in the underwater city of Rapture. Players explore the dystopian world while combating enemies and uncovering the mysterious story behind the city's downfall. The game emphasizes exploration, resource management, and moral choices that affect the outcome.

![Bioshock cover](Images/bioshock_cover.jpg)

> *We all make choices, but in the end, our choices make us.*
> 
> Andrew Ryan

---

## Gameplay Overview

### Key Features

* **Exploration**: Discover the secrets of Rapture while gathering supplies.
* **Combat**: Use a combination of weapons, plasmids, and the environment to defeat enemies.
* **Resource Management**: Scavenge for ammo, health, and ADAM to survive.
* **Moral Choices**: Decide the fate of Little Sisters, influencing the game's ending.

--- 

## Gameplay Loop

```mermaid
flowchart TB
    A[Exploration] --> B[Gather Resources]
    A --> C[Manage Weapons]
    B --> D{Enough Supplies?}
    D -- No --> E[Search for More Resources]
    D -- Yes --> F[Continue Exploring]
    D -- No --> G[Trade or Hack] --> H[Get More Supplies]
    H --> F
    E --> I{Face Big Daddy?}
    I -- Yes --> J[Prepare for Combat]
    I -- No --> F
    J --> F
    F -.-> A
```()
---
## External Resources
For more detailed guides and strategies, visit the following:
* [Official Website](https://www.2kgames.com/bioshock/)

![Official Logo](Images/bioshock_logo.jpg)
```

### No Git Bash:

**Commit das alterações:**
```
git add .
git commit -m “Added readme and images”
```
---
**Integração da branch na main:**
```
git switch main
git merge [new_doc_branch]
```
ou
```
git rebase main
git switch main
git merge [new_doc_branch]
```
---

**Actualização do repositório remoto e resolução de conflitos**

* *Verificar actualizações:*

```  
# Se foi feito clone no passo 2:
git pull origin main

# Se o repositório foi criado localmente e depois conectado ao remoto no passo 2:
git pull (origin main) #origin main é opcional porque já foi feito um pull anterior
```

* *Resolução do conflito*
```
# Resolução de conflitos no editor do documento
git add README.md
git commit -m “Resolução de conflitos”
```

* Finalmente a actualização do ficheiro no repositório remoto
```
#Se foi feito clone no passo 2:
git push (-u) origin main # O argumento -u é opcional porque associação entre as branches já vem definida

#Se o repositório foi criado localmente e depois conectado ao remoto no passo 2:
git push -u origin main # O argumento -u tem que estar presente no primeiro push para associar as branches main local e remota
```

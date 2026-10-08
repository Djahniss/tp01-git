# Compte rendu — TP01 Git Lemoine Djahniss

## Question 0

La version de Git installée est 2.43.0

## Question 1

Mon URL est https://github.com/Djahniss

## Question 2

filter.lfs.clean=git-lfs clean -- %f filter.lfs.smudge=git-lfs smudge
-- %f filter.lfs.process=git-lfs filter-process filter.lfs.required=true 
user.name=Djahniss Lemoine
user.email=loldja94@gmail.com
init.defaultbranch=main
core.editor=nano 
--global signifie que c'est appliqué a la main branch, ils sont dans le fichier git 

## Question 3.1
fatal: ni ceci ni aucun de ses répertoires parents (jusqu'au point de montage /)
 n'est un dépôt git Arrêt à la limite du système de fichiers (GIT_DISCOVERY_ACROSS_FILESYSTEM n'est pas défini). 
car je ne l'ai pas défini en temps que repo git

## Question 3.2
git init a creer le dossier .git/ car c'est un dossier cacher (.)
 Sur la branche main 
 Aucun commit 
 rien à valider

## Question 3.3
il range le README dans une zone temporaire car il n'est pas encore ajouté au git, une zone de préparation

## Question 3.4
il range README.md dans le head, c'est une zone de travail en attendant de push le commit

## Question 3.5
commit 701d51a059715084ce7f863c82508a2272e66cd7 (HEAD -> main) 
Author: Djahniss Lemoine <loldja94@gmail.com> 
Date:   Thu Oct 8 09:22:25 2026 +0200
      Création du README 

le hash est "701d51..."
l'auteur est Djahniss Lemoine associé à l'email loldjah94@gmail.com
la date est le Jeudi 8 octobre 9h22 UTC+2
le message est "Création du README"

## Question 3.7
1 git status décrit le README.md comme un fichier pas a jour et avec une différence par rapport au repo

2 diff --git a/README.md b/README.md
index ba53a0b..aaab789 100755
--- a/README.md
+++ b/README.md
@@ -3,3 +3,5 @@
 Dépôt réalisé par Djahniss Lemoine, 1CIEL-IR.
 
 Ce dépôt contient mon compte rendu du TP01.
+
+Année scolaire 2026-2027.

git diff montre la différence entre le local et le repo, le plus signifiant un ajout

## Question 3.8
8b6bf01 (HEAD -> main) Ajout de la mention de l'auteur du CR
30f3f5c Création de l'aide-mémoire Git
8fbefe0 Réponse à la question 3.7
b27da50 Ajout de l'année scolaire dans le README
6c264d7 Ajout du compte rendu (question 0à3.5)
701d51a Création du README

2 il est préférable de faire plusieurs commits pour plusieurs changement si
ils n'ont pas de rapport entre eux, autant pour le changelog que pour l'apparence dans oneline

#Question 4.1
git show montre les informations concernant le commit concerné comme le contenu et le contenu ajouté/supprimé
ainsi que des information comme l'heure/la date/l'auteur et le changelog du commit

#Question 4.2
git restore a permis de recupérer le fichier depuis le git, non car il ne serrais pas sauver sur le git

#Question 4.3
test.txt ce fait désindexer et ce retrouve dans la zone de préparation, il n'est pas supprimer juste pas dans l'éventuel commit

##Question 4.4
les fichiers ont disparu, *.log signifie tout fichier incluant .log
le fichier gitignore, et oui

##Question 4.5
il contenait seulement la phrase copier de base, depuis il y a eu l'ajout de l'année scolaire

#Question 5.2
1 id_ed25519 et id_25519.pub la .Pub est la clé publique
2
-rwx------ 1 dlemoine 1cielir-26-27  464 oct.   8 10:27 id_ed25519
-rwx------ 1 dlemoine 1cielir-26-27  100 oct.   8 10:27 id_ed25519.pub

#Question 5.4
Hi Djahniss! You've successfully authenticated, but GitHub does not provide shell access.
la clé publique est seulement un medium de communication elle n'autorise en rien sans la privé

#Question 6.3
	dlemoine@d116-03:~/tp-git/tp01-git$ git remote -v
origin	git@github.com:Djahniss/tp01-git.git (fetch)
origin	git@github.com:Djahniss/tp01-git.git (push)
	dlemoine@d116-03:~/tp-git/tp01-git$ git push -u origin main
Énumération des objets: 30, fait.
Décompte des objets: 100% (30/30), fait.
Compression par delta en utilisant jusqu'à 12 fils d'exécution
Compression des objets: 100% (29/29), fait.
Écriture des objets: 100% (30/30), 4.44 Kio | 1.11 Mio/s, fait.
Total 30 (delta 10), réutilisés 0 (delta 0), réutilisés du pack 0
remote: Resolving deltas: 100% (10/10), done.
To github.com:Djahniss/tp01-git.git
 * [new branch]      main -> main
la branche 'main' est paramétrée pour suivre 'origin/main'.

2 oui l'historique est le meme, tout les fichiers indexer sont présent, les fichier du gitignore ne sont pas présent car ignorer

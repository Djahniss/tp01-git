# Compte rendu — TP01 Git

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

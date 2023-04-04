# TP N°4 - PROGRAMMATION ANDROID ListView, AutoCompleteTextView et Adapter
A brief description of what this project does.

## Table of Contents

- [Description](#Description)
- [Content](#Content of project)
## Description
  The objective of this lab is to display a student's grades in a ListView. By clicking on one of the student's grades, a Toast message will be displayed indicating whether the corresponding subject has been validated or not (grade <10 or not).

   Each student has 6 grades. The order of the grades is important since the nth grade of each student corresponds to the nth subject. We obviously need the list of subjects (6 subjects in total). When entering the name of a student, we will use an AutoCompleteTextView that will suggest student names based on the characters we have entered.

## Content of project
Pour connecter la liste des notes à votre ListView, il est impératif d’utiliser un adapter.

- [Version 1 (ArrayAdapter)] :
  On utilisera un ArrayAdapter, qui est un adapter "prédéfini" qu’on pourra utiliser directement.
  
- [Version 2 (Adapter personnalisé) :]
  On souhaite personnalisé l’affichage des Views dans la ListView. Chaque élément de la ListView
  sera composé d’une icône et de la note. On spécifiera 2 icônes. Une pour les notes des matières
  validées et une pour les autres. Pour faire cela, on pourra pas utiliser un ArrayAdapter, il nous
  faudra alors créer notre propre adapter. Il s’agira d’une classe qui hérite de la classe
  ArrayAdapter et dans laquelle on implémentera un constructeur et la méthode getView. Notre
  application devra avoir cet aspect-là, comme si les figures ci-dessous.
-[Version 3 (Firebase) :]
  A présent, nous souhaitons connecter notre application à une base de données Firebase. Les
  notes des étudiants seront alors chargées depuis Firebase au moment de la sélection d’un
  étudiant. De plus, nous créerons une nouvelle activité pour l’ajout d’un nouveau étudiant et de
  ses notes. En cliquant sur le bouton valider, nous reviendrons directement vers le MainActivity.
  Les figures ci-dessous vous donneront une idée plus claire sur le résultat attendu.

## 

![version1 search](images/version1.png)
![version1 notes](images/version1_notes.png)


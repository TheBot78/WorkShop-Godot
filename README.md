# WorkShop-Godot

# Workshop shooter en 2D sur Godot
## Introduction
> Godot est un moteur de jeu multiplateforme, c'est-à-dire un logiciel permettant de créer des jeux vidéo qui est compatible avec différents systèmes d'exploitation. Il possède la faculté de pouvoir créer des jeux en 2D ou en 3D avec son propre langage, le GDScript qui ressemble au python.

## [Installation](https://godotengine.org/)

Vous n'avez qu'a installer la version LTS ou last version de godot et de lancer le binaire qui se trouve dedans.
> ATTENTION si vous prenez la dernière version c'est a vos risques et périles.
# Création d'un nouveau projet

> Vous allez arriver ici:

<p align="center">
    <img src="./.ressources/home.png">
    </a>
</p>

Pour créer un nouveau projet, il suffit de faire:

> New Project -> Mettre son nom de projet -> Create folder -> Create & Exit

# Création du monde

Lorsque vous commencez un projet Godot, la première étape est de faire un monde dans lequel vous allez pouvoir placer des objets, players et ennemies. Nous allons donc commencer par créer notre monde en 2D.

Vous arrivez ici après la manipulation précédente:

<p align="center">
    <img src="./.ressources/World.png">
    </a>
</p>

Commencez par créer une __Scene 2D__.

Et... c'est tout. Vous pouvez maintenant sauvegarder votre monde. N'hésitez pas à renommer votre scene pour plus de clarté.
Vous pouvez maintenant lancer votre monde avec le bouton ▶.

# Création du player

Maintenant que nous avons notre monde, nous pouvons maintenant créer notre player. Ce que nous allons faire, c'est que l'on va créer une autre scène qui sera notre joueur.

## Les caractéristiques du player

Nous voulons que notre player ne soit pas soumis à la gravité car nous voulons avoir le total contrôle sur notre perso. Nous allons créer un __KinematicBody2D__ qui sera la base de notre player. Nous voulons aussi un player animé afin qu'on puisse voir notre player bouger lors de mouvement. Il faut donc hériter la node __AnimatedSprite__ à notre __KinematicBody2D__.

Au final, nous aurons quelque chose de ce genre:
<p align="center">
    <img src="./.ressources/BasicPlayer.png">
    </a>
</p>
<br>

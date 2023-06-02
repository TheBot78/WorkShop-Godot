# WorkShop-Godot

# Workshop shooter en 2D sur Godot
## Introduction
> Godot est un moteur de jeu multiplateforme et gratuit. Il possède la faculté de pouvoir créer des jeux en 2D ou en 3D avec son propre langage, le GDScript qui ressemble au python.

## [Installation](https://godotengine.org/)

Vous n'avez qu'a installer la version LTS ou last version de godot et de lancer le binaire qui se trouve dedans.
> ATTENTION si vous prenez la dernière version c'est à vos risques et périls.

# Création d'un nouveau projet

> Vous allez arriver ici:

<p align="center">
    <img src="./.ressources/home.png">
    </a>
</p>

Pour créer un nouveau projet, il suffit de faire:

> New Project -> Mettre son nom de projet -> Create folder -> Create & Exit

## Création du monde

Lorsque vous commencez un projet Godot, la première étape est de faire un monde dans lequel vous allez pouvoir placer des objets. Nous allons donc commencer par créer notre monde en 2D.

Vous arrivez ici après la manipulation précédente:

<p align="center">
    <img src="./.ressources/world.png">
    </a>
</p>

Commencez par créer une __Scene 2D__.

Et... c'est tout. Vous pouvez maintenant sauvegarder votre monde. N'hésitez pas à renommer votre scene pour plus de clarté.
Vous pouvez maintenant lancer votre monde avec le bouton ▶.

>N'oubliez pas que google et la documentation Godot sont vos amis ^^

## Création du joueur

Maintenant que nous avons notre monde, nous pouvons maintenant créer notre joueur. Ce que nous allons faire, c'est créer une autre scène qui sera notre joueur.

Nous voulons que notre joueur ne soit pas soumis à la gravité car nous voulons avoir le total contrôle sur notre personnage. Nous allons créer un __KinematicBody2D__ qui sera la base de notre joueur. Nous voulons aussi que notre personnage soit animé. Il faut donc hériter la node __AnimatedSprite__ à notre __KinematicBody2D__.

Au final, nous aurons quelque chose de ce genre:
<p align="center">
    <img src="./.ressources/BasicPlayer.png">
    </a>
</p>
<br>

## Création de l'animation du joueur

En selectionnant __AnimatedSprite__, on peut créer les frames qui servireront à animer le joueur. Il suffit d'appuyer sur _Frames_ et de faire un __New SpriteFrame__. Réappuyez sur _SpriteFrame_ et vous allez arriver sur cette interface:

<p align="center">
    <img src="./.ressources/SpriteFrame.png">
    </a>
</p>

Vous pouvez dès à présent créer vos animations avec votre sprite-sheet. Pour ce faire, vous devez appuyer sur le bouton "Add frames from a Sprite Sheet". Découpez votre sprite sheet afin que l'on puisse récupérer les sprites.
<br>
C'est maintenant à vous de créer les animations de votre personnage.
> [Si vous n'avez pas de spritesheeet](https://opengameart.org/content/a-platformer-in-the-forest)

# Collision du joueur

Vous pouvez voir qu'il y a encore une erreur sur le __KinematicBody2D__ et qu'il demande une __CollisionShape2D__. 
> Créez donc en une et placez la bien sur votre joueur.
<br/>

# Mouvement du joueur

Maintenant que votre joueur est créé, il suffit maintenant d'ajouter un script qui permettera de le faire bouger avec les touches du clavier.

## Configuration des touches

Configurez d'abord les touches du clavier dans:
 
>  Project -> Project Settings -> Input Map



Ici, vous allez bind les touches du clavier pour faire bouger le player.

Ca devrait ressembler à ceci:

<p align="center">
    <img src="./.ressources/bindKeyboard.png">
    </a>
</p>

## Placement du décors

Maintenant que le joueur est présent vous allez avoir envie de placer vos éléments pour donner un ensemble qui créé un décors.

Pour placer des éléments vous allez avoir besoin d'une __TileMap__ à l'intérieur de laquelle vous allez trouver les TileSet. Utilisez cet interface pour couper votre spritesheet

> TileMap -> TileSet -> [+]

<p align="center">
    <img src="./.ressources/TileMap.png">
    </a>
</p>
## Colisions Map

Vous pouvez maintenant rajouter des collisions avec la catégorie associée au différents TileSets et commencez à construire votre monde

## Saut du joueur

Vous allez maintenant pouvoir rajouter le saut à votre joueur, mais maintenant à vous de trouver comment faire !


## Amusez Vous
Maintenant vous maitrisez les bases pour faire un plateformer, vous êtes libre de rajouter des bonus à votre jeu !

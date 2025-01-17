# DelphiFMXGameSnippets

Des exemples de ce qui se fait lorsqu'on développe des jeux vidéos : gestion de sprites, musiques de fond, effets sonores, animations ...

Les projets sont développés sous Delphi avec son framework multi plateformes FireMonkey pour exécuter nos projets sous Windows, macOS, iOS, Android et Linux à partir de la même base de code.

Les images et musiques utilisées dans ce dépôt ne sont pas toutes libres de droit. Ne les réutilisez que si vous en avez une licence. Ils restent la propriété de leurs auteurs respectifs et ne sont présents dans les programmes qu'à des fins de démo.

Sont utilisées des images et des provenant de :
- Kenney que je remercie pour son oeuvre et son esprit de partage. Pensez à faire comme moi : soutenez le en achetant des licences de ses créations si vous les utilisez même s'il ne nous y oblige pas. https://kenney.nl/
- The Game Creators, éditeur de logiciels de création de jeux vidéos et de jeux, propose aussi des assets dont une librairie de bruitages utilisée ici. https://www.thegamecreators.com/
- GSP 500 Noises, un CD-Rom de bruitages libres de droits publié en 1995
Oui, je sais, certains d'entre vous n'étaient pas nés... Il y avait aussi une vie avant l'Internet.
- Cartoon Smart qui propose des vidéos de formation au développement de jeux vidéos pour iOS et macOS avec la possibilité de télécharger des librairies de sons et d'images libres de droit lorsqu'on est abonné. https://vasur.fr/cartoonsmart

Des informations complémentaires seront prochainement disponibles sur le blog https://developpeur-pascal.fr concernant les blocs de code réutilisables. Ce document sera également maintenu au fil des évolutions des fichiers réutilisables et exemples proposés.

Les projets de ce dépôt sont dans le groupe fr.developpeurpascal.demo.*
Merci de ne pas les diffuser sur les magasins d'application ni ailleurs en version compilée mais de systématiquement renvoyer vers ce site.

Cette librairie a été créée en direct sur Twitch lors de l'opération GamingForSidaction en faveur du [Sidaction 2021](https://sidaction.org). Vous pouvez consulter le replay de ce week-end sur https://serialstreameur.fr/sidaction-2021.php

Si vous voulez voir le résultat des animations dans un vrai jeu vidéo, jetez donc un oeil à Ok Ducky développé en direct lors de ce week-end de game coding en live :
https://gamolf.itch.io/ok-ducky

D'autres jeux ont été développés tout au long de l'année 2021 et au delà sur Twitch. Les rediffusions de ces sessions sont disponibles sur https://serialstreameur.fr/jeux-video.php ou la rubrique live coding du site https://serialstreameur.fr/live-coding.php

-----

Les projets de ce dépôt sont :

* AnimationDroiteGauche

Création d'une image composée de plusieurs qui va faire des aller/retours en bas de l'écran.

* AnimationSprite

Transformation de l'image précédente en "sprite" géré sous forme de TFrame indépendant permettant de le réutiliser.

* AnimationPlusieursCanardsALEcran

Utilisation du sprite du canard et multiplication de celui-ci à l'écran sur plusieurs niveaux.

* MusiqueDAmbiance

Création d'un librairie pour jouer des musiques en fond sonore des logiciels. Elle est réutilisable en l'état.
Le composant TMediaPlayer de FireMonkey est utilisé. Une évolution plus pratique pour améliorer les choses serait de passer directement par les différentes API de sons/musiques des systèmes d'exploitation ciblés.

* EffetsSonores

Utilisation de la librairie musicale et adaptation pour jouer des son uniques ou à plusieurs.

* AnimationVagues

Dessin et animation de vagues sur plusieurs niveaux. C'est la base des animations en parallax (plusieurs niveaux de vitesse différente).

* AnimationVaguesEtCanards

Maintenant que vous savez faire des vagues, nous ajoutons des canards sur les différents niveaux.

* AnimationGrossissement

Une animation classique dans les jeux vidéos : on touche quelque chose, il grossit jusqu'à traverser l'écran vers nous et disparaît.

* CanardPivot

On continue avec ce pauvre canard qui va maintenant pouvoir réagir si on clique sur lui ou son socle.

* CreateSpriteSheet

Les spritesheets sont des images contenant d'autres images. Hyper pratique quand on veut diminuer les temps de téléchargement sur les jeux en ligne. Ca sert aussi depuis les premiers jeux vidéos à stocker toutes les étapes d'une animation.

Dans Delphi, le framework FireMonkey propose des tas de types d'animations (au sens "modification de comportements selon une formule mathématique"). L'une de ces animations permet de modifier une image à partir d'une spritesheet et de faire ainsi des images animées.

La plupart des sources/banques d'images/graphistes proposant des animations les propose déjà sous forme de spritesheet ou de séries d'images mais elles ne sont pas toujours compatibles avec le comportement du TBitmapAnimation et il est donc nécessaire de créer nos propres spritesheets à partir des images de l'animation.

Téléchargez le programme compilé depuis https://gamolf.itch.io/spritesheet-creator

* AnimSpriteExplosion

Utilisation d'une spritesheet pour montrer comment fonctionne le TBitmapAnimation.

* AnimSpriteEauDuLac

On en profite pour faire de l'eau qui bouge sur la rive d'un lac. L'image utilisée n'étant pas top, l'effet est bizarre mais le principe reste le même avec de meilleures illustrations.

* AnimSpritePersonnage

Et on finit par faire marcher puis sauter un ninja...

* DuckJoke

Tout est dans le nom... Un programme créé un 1er avril que je dédie à toutes les personnes qui oublient de verrouiller leur session lorsqu'elles sont dans les transports en commun.

Téléchargez le programme compilé depuis https://gamolf.itch.io/duck-joke

* JeuDesCercles

Un exemple de programme avec des cercles en guise de sprite qui permet de gérer leurs mouvements, les collisions entre eux et rebonds.

* AnimGagneDesPoints

Animation lorsqu'on gagne des points dans un jeu.

* AnimScore

Animation du changement de valeur d'un score.

* AffichageTexteGeneriqueStarWars

Affichage d'un texte façon générique de Star Wars (défilement du bas vers le centre de l'écran en profondeur).

Image de fond provenant de la NASA.
Son d'ambiance provenant de https://www.soundboard.com/sb/sound/918028
(téléchargé au premier lancement du programme dans le dossier de l'exe)

Utilise une unité du projet https://github.com/DeveloppeurPascal/librairies à placer dans la même arborescence que ce groupe de projet. "librairies" doit être au niveau de "DelphiFMXGameSnippets".

* AnimMeteoNeige

Effet de neige qui tombe sur plusieurs avec éventuelement du vent.

* AnimCroixQuiTournent

Le but du jeu était de refaire l'animation correspondant à ce GIF:
https://twitter.com/OrgPhysics/status/1200324633096065024
Des croix blanches et noires qui tournent en alternance.

Cet exemple utilise les composants Radiant Shapes disponibles depuis GetIt.
https://getitnow.embarcadero.com/bonus-radiant-shapes/

TODO : comprendre pourquoi un contour persiste lors de la rotation des croix puis le corriger

* MusicLoopUnitTest

Programme multiplateforme de test des sons et musiques joués par l'unité uMusicLoop.pas
(utile pour s'assurer de l'absence de bogue sur les plateformes à chaque version de Delphi)

Utilise une unité du projet https://github.com/DeveloppeurPascal/librairies à placer dans la même arborescence que ce groupe de projet. "librairies" doit être au niveau de "DelphiFMXGameSnippets".

Le son de test (WAV) est téléchargé au lancement du programme et mis en cache depuis la page https://opengameart.org/content/win-sound-effect avec comme url https://opengameart.org/sites/default/files/Win%20sound.wav

La musique de test (MP3) est téléchargée au lancement du programme et mis en cache depuis la page https://opengameart.org/content/battle-theme-b-for-rpg avec comme URL https://opengameart.org/sites/default/files/battleThemeB.mp3

* UtilisationSpriteSheet

Exemple d'utilisation et de découpage d'une spritesheet formatée en blocs.

Sprite sheet utilisée comme démo provenant de https://kenney.nl/assets/pixel-platformer

* SpriteSheetSplitter

Découpe une spritesheet (largeur/hauteur identique, éventuelement avec un décalage en largeur ou en hauteur) en sprites.

Téléchargez le programme compilé depuis https://gamolf.itch.io/spritesheet-creator

* BitmapHorizReverse

Fait une symétrie horizontale pour retourner une image et en crée une autre (utile pour récupérer des bas de zone de décor à partir des images du haut).

cf sprites utilisés dans Egg Hunter (vidéos de création sur https://serialstreameur.fr/jv-egg-hunter.php, jeu à télécharger sur https://gamolf.itch.io/egg-hunter)

-----

## TODO LIST

* ajouter des projets de tests unitaires pour les unités réutilisables 

-----

Si vous ne connaissez pas Delphi et le langage Pascal, profitez de la version Academic (pour les étudiants, enseignants et établissements d'enseignement) ou Community Edition (gratuite pour une utilisation personnelle) disponibles chez Embarcadero (rubrique "outils gratuits").
En entreprise vous pouvez aussi tester Delphi avec la version d'évaluation.
https://www.embarcadero.com/products/delphi

Cette formation en ligne gratuite vous apprendra les bases de la programmation avec le Pascal et Delphi même si vous n'avez jamais appris à programmer :
https://apprendre-delphi.fr/apprendre-la-programmation-avec-delphi/

Des conférences en ligne et des webinaires (points techniques sur des sujets précis) sont organisés régulièrement. Consultez [le planning de ces webinaires](https://developpeur-pascal.fr/p/_6007-webinaires.html) et regardez les [rediffusions des webinaires Delphi](https://serialstreameur.fr/webinaires-delphi.php).

Des sessions de [live coding sur Twitch](https://www.twitch.tv/patrickpremartin) ou [la chaîne YouTube Developpeur Pascal](https://www.youtube.com/channel/UCk_LmkBB90jdEdmfF77W6qQ) sont également organisées régulièrement. Pour Twitch vous pouvez consulter [le planning hebdomadaire](https://www.twitch.tv/patrickpremartin/schedule). Vous pouvez aussi vous reporter à [cet article](https://developpeur-pascal.fr/p/_600e-livestreams-de-codage-en-direct-avec-delphi.html). Pour les rediffusions de tout ça, rendez-vous simplement dans la [rubrique live coding](https://serialstreameur.fr/live-coding.php) de [Serial Streameur](https://serialstreameur.fr/) où vous trouverez de nombreuses vidéos en français à destination des développeurs de logiciels, applications mobiles, sites web et jeux vidéo.

Enfin, si vous préférez la lecture à la vidéo, vous trouverez tous les livres récents publiés sur Delphi et le langage Pascal sur [Delphi Books](https://delphi-books.com)

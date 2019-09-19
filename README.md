# Projet 2 – Jekyll

Ce projet vous introduira à la génération de sites statiques grâce à **Jekyll**. Durant les prochaines semaines vous découvrirez les bases du **templating** et de l'abstraction de contenu, tout en étoffant les notions de workflow Git et GitHub Pages acquises lors du projet précédent. Vous devrez faire preuve de grande rigueur dans l'organisation de votre projet, sinon Jekyll ne fonctionnera pas. Chaque chose à sa place.  

Vous travaillerez à nouveau avec votre portfolio, dans l'optique de l'adapter de telle sorte que chaque nouvelle entrée ne nécessite qu'un fichier markdown supplémentaire et aucun markup HTML ou CSS. Profitez-en pour réfléchir au code que vous avez écrit jusqu'à présent et le néttoyer, si nécessaire.

Pour ne pas passer des heures à configurer le projet, j'ai mis en place ce *boilerplate*.

Le rendu aura lieu le **8 novembre**.

Installation du Boilerplate
======

[Jekyll](https://jekyllrb.com) est un programme Ruby. Pour l'installer il est nécessaire que vous passiez par le terminal (c'est du sérieux). 

Installation des outils de ligne de commande
------
Première chose, ouvrez votre terminal. Puis installez les outils de ligne de commande Apple, grâce à la commande suivante:
```
xcode-select --install
```
Vous devriez voir une alerte, cliquez sur **installer**. Attendez la fin de l'installation avant de continuer. 

Installation de Ruby > 2.4
------
Entrez la commande suivante dans le terminal
```
ruby -v
```
Si la version indiquée est plus grande ou égale à 2.4, vous pouvez passer directement à la section suivante. Sinon, veuillez suivre les instructions qui suivent. 

Installez le logiciel de gestion de paquets [Homebrew](https://brew.sh) (extrêmement utile), avec la commande suivante:

```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
Une fois l'installation terminée, il faut que vous installiez Ruby avec la commande suivante:

```
brew install ruby
```

Quand c'est fait, ajoutez Ruby à votre configuration avec la commande suivante:

```
export PATH=/usr/local/opt/ruby/bin:$PATH
```

Finalement, vérifiez le tout avec: 
```
ruby -v
```
Bravo, vous avez installé tout l'environnement de programmation Ruby depuis votre ligne de commande. 

Installation de Jekyll
------

Entrez la commande suivante dans votre terminal
```
gem install jekyll bundler
```
Clonez votre repo grâce à GitHub Desktop, puis dirigez votre le ligne de commande dans le dossier que le clone à créé. Vous pouvez aussi glisser le dossier en question dans votre fenêtre de terminal. 

```
cd là/où/se/trouve/le/dossier
```
Une fois dans le dossier, lancez la commande suivante
```
bundle install
```
Puis vous pouvez lancer le serveur de développement Jekyll grâce à la commande suivante:
```
bundle exec jekyll serve
```

votre site est maintenant accessible à http://localhost:4000

Et voilà. Bravo.

Configuration du boilerplate
======

Le repo que vous avez cloné est normalement déjà configuré pour l'utilisation de GitHub Pages. Il faut néanmoins que vous changiez une petite ligne dans la configuration Jekyll:

Ouvrez le fichier **_config.yml** dans votre éditeur de texte, puis modifiez la ligne suivante que le nom exact de votre répo y figure (précédé du "/").

```
baseurl: "/projet-2-boilerplate"
```


Ressources
======

* [Jekyll](https://jekyllrb.com) – Le générateur de site statique.
* [Liquid](https://shopify.github.io/liquid/) – Le language de templating que nous allons utiliser. 
* [SCSS](https://sass-lang.com) – Un précompilateur pour faire des choses formidables avec le CSS, comme introduire des variables. Vous pouvez l'utiliser, ou non. C'est votre choix. On peut écrire du CSS standard dans un fichier .SCSS
* [GitHub Pages](https://pages.github.com) – La documentation pour le système d'hébergement GitHub que nous avons déjà utilisé sur le projet précédent. 
* [Forestry](https://forestry.io) – Si nous avons le temps ou si vous êtes très en avance, vous intégrerez le CMS Forestry à votre projet. 


# POSITIONS

la position se calcule par rapport au point 0,0 , en haut a gauche.

## position : relative
Le navigateur positionne, par defaut, les elements relativement, soit par rapport au parent, soit par rapport a l'element précédent dans le DOM.toutes le directives gérant le positionnement s'appuyent sur ce principe.

## position : absolute
se definie via les directives top,right,bottom et left.la balise sort du flux (la balise suivante ne se positionne plus en s'appuyant sur sa position) du rendu.cette position est relative a la première balise parente dont la position est explicitement definie (absolute, relative,...), sinon c'est le viewport qui sert de référence.

## position : fixed
c'est une spécialisation de la position absolue mais le calcul est fait a partir du viewport.

### disclaimer
le calcul des dimensions en pourcentage s'effectue relativement aux dimensions de la balise parente.le navigateur est capable de calculer la largeur d'une balise car elle est definie par le viewport. La hauteur dépend du contenu, il n'est donc pas possible de gerer les hauteurs en pourcentage sans avoir au préalable défini une hauteur fixe sur la balise parente (le contenu total n'est pas disponible au moment du dimensionnement vertical).

# DISPLAY
défini la manière dont une balise est gérée pour l'affichage, son rendu.

## display : block
le navigateur cherche a positionner la balise sur la gauche du parent. et prépare un passage a la ligne pour l'élement suivant.

## display : inline
les balises se positionne sur une ligne (comme une chaine de caractère) et passe a la ligne suivante  si cela dépasse la largeur du parent. on peut le voir comme le cadrillage d'un cahier d'écriture 

## display : inline-block
ils gardent le comportement de type block (les marges top et bottom effectives) , néanmoins ces elements sont alignés sur la baseline (c'est a dire comme des caractères). la baseline (le centrage des caractère) va dépendre de elements inline ou inline-block définis.

## display : flex
la directive s'applique sur la balise parente des blocks a aligner (wrapper). elle est utilisée pour construire une interface web "en colonne".


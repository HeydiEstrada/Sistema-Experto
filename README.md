# Sistema-Experto

cine_juvenil(waar).

cine_juvenil(bumblebee).


cine_infantil(big_heroe).

cine_infantil(the_croods).

cine_infantil(inside_out).


cine_familiar(modern_times).

cine_familiar(interestellar).

cine_familiar(whiplash).

cine_adulto(amelie).

cine_adulto(focus).
          
genero(ficción).

genero(aventura).

genero(comedia).

genero(musical).

genero(drama).

genero(romance).

formato(tresd).

formato(animación).

formato(mudo).

formato(sonoro).

formato(imagen_real).


es_de_genero(bumblebee,acción).
es_de_genero(bumblebee,ficción).
es_de_genero(waar,accion).
es_de_genero(waar,suspenso).
es_de_genero(big_heroe,acción).
es_de_genero(big_heroe,aventura).
es_de_genero(the_croods,aventura).
es_de_genero(the_croods,comedia).
es_de_genero(inside_out,aventura).
es_de_genero(inside_out,comedia).
es_de_genero(interestellar,ficción).
es_de_genero(interestellar,aventura).
es_de_genero(modern_times,comedia).
es_de_genero(modern_times,drama).
es_de_genero(whiplash,musical).
es_de_genero(whiplash,drama).
es_de_genero(amelie,romance).
es_de_genero(amelie,comedia).
es_de_genero(focus,drama).
es_de_genero(focus,romance).

tiene_formato(bumblebee,tresd).
tiene_formato(interestellar,tresd).
tiene_formato(big_heroe,animación).
tiene_formato(the_croods,animacion).
tiene_formato(inside_out,animacion).
tiene_formato(modern_times,mudo).
tiene_formato(whiplash,sonoro).
tiene_formato(amelie,imagen_real).
tiene_formato(focus,imagen_real).
tiene_formato(waar,imagen_real).

igual_genero(X,Y):- es_de_genero(X,G),es_de_genero(Y,G).

mismo_formato(X,Y):- tiene_formato(X,F),tiene_formato(Y,F).

igual_genero_y_mismo_formato(X,Y):- es_de_genero(X,G),es_de_genero(Y,G),tiene_formato(X,F),tiene_formato(Y,F).

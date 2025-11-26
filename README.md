# P4---Rebase-con-conflicto-en-Git

## ¿Desde qué rama ejecutaste el comando git rebase main? ¿Por qué desde esa y no desde main?
En la rama estilo_texto para no modificar main porque es la rama base.

## ¿Por qué se ha producido el conflicto en notas.txt al hacer el rebase?
El conflicto ocurrió porque tanto en main como en mi rama se modificó el mismo archivo y las mismas líneas. Git no sabía qué versión debía conservar, así que me pidió que lo resolviera manualmente.

## ¿Qué habría pasado si hubieras borrado una de las versiones sin fijarte bien en el texto?
Pues habría perdido parte del contenido sin darme cuenta, ya fueran mis propios cambios o los de main. Git habría seguido el proceso de rebase, pero el archivo quedaría incorrecto o incompleto.

## ¿En qué se diferencia este caso de un conflicto de merge? (a nivel práctico, en lo que tú has tenido que hacer).
En un merge, después de resolver el conflicto hago git add y git commit.
En un rebase, después de resolverlo hago git add y git rebase --continue, porque no se crea un commit de merge y Git sigue reaplicando mis commits.

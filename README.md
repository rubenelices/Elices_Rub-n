# Elices_Ruben
# ¿Que es un Pull request?
Un Pull request es una petición que le haces al creador de un repositorio para que aplique los cambios que has realizado tú en su propio repositorio. Una vez el creado te acepte el pull request se actualizará su repositorio.
# ¿Que es un conflicto de fusión? ¿Como lo resolverias?
Un conflicto de fusión es un problema que te sale a la hora de fusionar dos ramas usando el comando merge, básicamente lo que porduce es una alteracion en el archivo de texto con el que estes trabjando en ese momento y que no te dejará avanzar hasta que lo arregles. Para resolverlo haría nano "nombre del archivo de texto que este editando"."formato del archivo" y una vez dentro del editor eliminaria aquellas frases o palabras que estuvieran generando el conflicto (normalmente salen en zonas que antes no había nada y con muchos signos repetidos). Una vez corregido todo, saldria del editor guardandolo primero (ctrl s) y luego añadiría los cambios realizados con el comando $git add .  y confirmaría que ya esta arreglado utilizando un comando git merge --continue.
# ¿Procedimiento para fusionar ambas ramas?
Primero me aseguraría de que estoy en la rama main y en caso de que no lo estuvier haría $git checkout main .Luego haría git merge "examen_parcial" y al darle al enter me saldría que hay conflictos, los resolvería como he indicado anteriormente y una vez resueltos haría $git add . para actualizar los cambios y luego $git merge --continue para confirmar que se puede seguir con la fusión y acabarla.
# ¿Comando para revertir un commit?
Para revertir un commit utilizaría el comando git reset "nombre del commit" 
# ¿Como se realiza un fork?
Para realizar un fork en github tienes que ir al repositorio que quieres copiar y una vez estes en este te saldrá un botón arriba a la derecha, lo pulsas y automaticamente se te creara un repositorio propio con el nombre del que has copiado pero en tu cuenta de github y podrás empezar a trabajar en el como si fuese tuyo. Se suele utilizar para copiar poryectos que ya se han realizaddo y hacerlos tuyos y así poder editarlos a tu gusto.
# Como llegar al archivo.txt
a) En este caso al estar en un principio en el directorio raíz tendrías que hacer cd ruben_elices y luego cd archivo.txt y sería una ruta absoluta ya que empiezas desde la raíz
b) En este caso solo tendrias que hacer cd UAX para entra en el archivo UAX y leugo ya cd archivo.txt . Sería una ruta relativa
# Comandos para realizar cada tarea
1) Git clone
2) Git checkout
3) Git checkout
4) Git add
5) Git commit
6) Git push
7) Git pull
8) Git merge
9) git reset --hard
10) Git log
# Describe detalladamente los pasos y consideraciones que tomarías para lograr esta tarea, incluyendo cómo manejarías los posibles conflictos de fusión y cómo asegurarías que la integración final en develop sea estable y funcional.
Lo primero que haría sería meterme a la rama develop para fusionar en ella las otras ramas utilizando el comando $git checkout develop. Para empezar haría $git merge "matemáticas" y resolvería los conflictos que me saliesen en el editor para mantener el codigo limpio tal y como estaba antes de hacer la fusión, una vez resueltos los conflictos haría git merge --continue para indicar que se puede seguir con la fusión porque ya he resuelto los conflictos luego haría $git add . para actualizar los cambios en la rama develop y después $git merge -m "Resolución conflictos rama matematáticas". Después comprobaría que funcione y que todo este en orden y seguiría con la rama diseño_UX haciendo lo mismo que he hecho en la rama matemáticas pero en este caso con la rama diseño_UX. Una vez hechas las dos fusiones compruebo que ambas ramas se han integrado correctamente y que todo va bien solo faltaría pasarlo a la rama main.
# Realización de la tarea 3
c) Añadi el botón x^4 al archivo index.html en mi repositorio local, creé un commit con los cambios y luego subí el repositorio local al remoto en la rama primcipal "master"

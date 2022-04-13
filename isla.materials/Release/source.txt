"La isla misteriosa" by Xavier Carrascosa (in spanish)

[ Datos bibliográficos ]

Part 1 - Introducción

The story title is "La isla misteriosa".
The story author is "Xavier Carrascosa".
The story headline is "'Una aventura llena de dudas, misterios y pocas respuestas.'".
The story genre is "Mystery".
The release number is 3.
The story creation year is 2011. [Adaptación a 2022]
The story description is "El gran conquistador Hernán Cortés se encuentra a merced del peligro en una tierra exótica buscando un tesoro perdido... ¿logrará encontrarlo? La isla misteriosa esconde una aventura que no es lo que parece...".

Section 1 - Extensiones

[Efectos de pantalla básicos]
Include Basic Screen Effects Sp by Emily Short. 

[Extensión de Ayuda básica]
Include Basic Help Menu SP by Emily Short. 

Release along with the source text, a cover art and  an interpreter.


Section 2 - Mensaje inicial y ayuda extendida
  
When play begins:
clear the screen;
say
"[line break][italic type]'Hay que estar borracho siempre. 
[line break]He ahí la única cuestión.
[line break]Para no ser los mártires esclavos del tiempo, 
[line break]que destruye tus espaldas y te doblega hacia la tierra, 
[line break]hay que embriagarse sin cesar.
[line break]¿Pero de que? 
[line break]De vino, de poesía, o de virtud, como quieras.'
[paragraph break]Charles Baudelaire[roman type]";
wait for any key;
clear the screen;
say "[paragraph break]Teclea [bold type]'AYUDA'[roman type] durante el juego para recibir instrucciones.[paragraph break]";
choose row 1 in Table of Basic Help Options;
     now description entry is "[italic type]El gran conquistador Hernán Cortés se encuentra a merced del peligro en una tierra exótica buscando un tesoro perdido... ¿logrará encontrarlo? La isla misteriosa esconde una aventura que no es lo que parece...[paragraph break][roman type]".

Table of Basic Help Options (continued)
title    	 subtable    	 description
"Contactar con el autor"    	 --    	 "Si tienes dificultades con [story title], contacta conmigo a través de mi e-mail: xavier.carrascosa@gmail.com o entra en los foros del portal CAAD: www.caad.es. También puedes visitar mi página: www.xaviercarrascosa.com o consultarme en Twitter: @XCarrascosa"
"Pistas"    	 --	"A continuación van unas cuantas pistas para [story title].[paragraph break][bold type]1. La serpiente odia las piedras.[line break]2. ¿Has probado a nadar en el mar?[line break]3. El mendigo tiene sed.[line break]4. ¡Duerme un poco y lo conseguirás![roman type]".


Part 2 - Escenario

Section 1 - El bosque

Bosque is a room. The description is "[if unvisited]Lejano entre las brumas apareces como reflejo de un arquetipo mítico, en la inmensidad verde de un bosque desconocido. Ahora eres tú el que decide el rumbo que tomarán tus pasos, las consecuencias de tus actos y las palabras que de tu boca han de surgir, tanto para recitar hermosos versos, como para juzgar con tu voz a tus semejantes. El sendero que atravesarás te espera, más allá hay un mundo nuevo, pero ten cuidado de sus peligros… [else]Te encuentras en un bosque de enormes árboles. Un sendero lleno de maleza se pierde por el sur; al norte divisas una gran montaña."
Some arboles are in the Bosque. They are scenery. The printed name of arboles is "árboles". The description is "Los árboles son tan altos que apenas dejan pasar la luz del sol.". Understand "bosque", "arboles", "sol" and "mundo" as the arboles.
The sendero is here. It is scenery. The description is "Un sendero por el que te puedes adentrar en éste desconocido mundo, cuyos peligros solo son comparables con sus maravillas. Al norte se divisa una montaña, al sur te espera la costa". Understand "camino", "maleza" as the sendero.
The montana2 is here. It is scenery. The printed name of montana2 is "montaña". The description is "Una pequeña montaña marca los límites del bosque. Podrías ir hacia el norte para alcanzar su cima." Understand "cima" and "limites" as the montana2.
The playa22 is here. It is scenery. The printed name of playa22 is "playa". The description is "A lo lejos se divisa la costa, unas playas de aguas cristalinas te esperan..." Understand "aguas", "playa" and "costa" as the playa22.
Instead of taking the arboles, say "¡No puedes cargar con todos los árboles del bosque! Si quieres madera, tendrás que conseguirla de otra forma.".

Section 2 - La playa

Playa is south of Bosque. The description is "Estás en una larga playa desde la que se divisa una isla a lo lejos. Puedes ver muchas palmeras por aquí.".

The costa is female and scenery in Playa. The description is "Estas aguas son tan bellas como peligrosas, piensas mientras observas la diminuta isla, allá a lo lejos.". Understand "isla", "mar", "playa", "aguas", "agua", "linea" and "oceano" as the costa.

Some arboles2 are in the Playa. They are scenery. The printed name of arboles2 is "árboles". The description is "Atrás has dejado el bosque y sus enormes árboles.". Understand "bosque", "arboles", "arbol", "sol" and "mundo" as the arboles2.
The sendero2 is here. It is scenery. The description is "El sendero quedó atrás, ahora debes mirar hacia delante.". Understand "camino", "maleza" as the sendero2.
The montana4 is here. It is scenery. The printed name of montana4 is "montaña". The description is "Observas la montaña a lo lejos, testigo mudo de tus actos." Understand "cima" and "limites" as the montana4.

Instead of nadaring en the costa for the first time:
	say "Decidido y sin temor te adentras en el mar, nadando hacia la lejana isla...[paragraph break]";
	wait for any key;
	say "De repente, en mitad de la travesía, te das cuenta... ¡el mar está infestado de tiburones! Nadas todo lo rápido que puedes hasta llegar exhausto a la costa... ¡esta vez has tenido suerte![paragraph break]";
	wait for any key;
	now the player is in Isla.

Instead of nadaring en the costa:
	say "Decidido y sin temor te adentras en el mar, nadando hacia la lejana isla...[paragraph break]";
	wait for any key;
	if a random chance of 1 in 5 succeeds:
		say "Pero de repente observas una amenazadora aleta de tiburón que se aproxima hacia ti... ¡intentas huir con todas tus fuerzas! Pero...[paragraph break]";
		end the story saying "Mueres en las fauces del tiburón.";
	otherwise:
		say "Finalmente, y tras un gran esfuerzo, llegas a la costa. Contemplas maravillado la paradisíaca isla...[paragraph break]";
		wait for any key;
		now the player is in Isla.

		
Instead of nadaring in Playa, try nadaring en the costa.

Some palmeras are in the Playa. They are female and scenery. The description is "La playa está repleta de palmeras, que se inclinan hacia el mar a causa del viento.".
Instead of taking the palmeras, say "¡No puedes cargar con todas las palmeras de la playa! Si quieres madera, vete al bosque.".

The cofre is in the Playa. The description is "[if open]El pequeño cofre está abierto. Su interior es impermeable y por lo tanto el agua del mar no ha estropeado su contenido...[otherwise]Un pequeño cofre misterioso, bellamente adornado, aunque algo deteriorado por las inclemencias del mar."
It is container, openable, lockable and locked. The matching key of the cofre is the llave oro.

[El cofre contiene un mapa del tesoro que está programado en la sección 2 de la Part 4 - Nudo]

Rule for printing room description details of cofre:
if the cofre is open, say " abierto";
if the Playa is unvisited, say " que llega mecido por las olas, ";
if the cofre is closed and Playa is visited, say " misterioso";
omit contents in listing.

Section 3 - La montaña

Montana is north of Bosque. The printed name of Montana is "Montaña". The description is "Te encuentras en una alta montaña desde la que se divisa un bosque y una playa, allá a lo lejos. Observas multitud de piedras por aquí."

Some piedras are in the Montana. They are female and scenery. The description is "Puedes ver numerosas piedras por aquí y por allá.". Understand "piedra", "roca" and "canto rodado" as the piedras.
The piedra is female. The description is "Una piedra con la que podrías hacer mucho daño.".

The playa21 is here. It is scenery. The printed name of playa21 is "playa". The description is "A lo lejos se divisa la costa, unas playas de aguas cristalinas te esperan..." Understand "aguas", "playa" and "costa" as the playa21.
Some arboles3 are in the Montana. They are scenery. The printed name of arboles3 is "árboles". The description is "Atrás has dejado el bosque y sus enormes árboles.". Understand "bosque", "arboles", "arbol", "sol" and "mundo" as the arboles3.
The sendero3 is here. It is scenery. The description is "El sendero se pierde hacia el sur, adentrándose en el bosque.". Understand "camino", "maleza" as the sendero3.
The montana5 is here. It is scenery. The printed name of montana5 is "montaña". The description is "Desde lo alto de la montaña, contemplas la inmensidad de éstas tierras. No se ve ningún animal por aquí, solo piedras, pero a lo lejos se divisa una playa, y aún más allá parecen adivinarse unos islotes. Tal vez en ellos encuentres lo que buscas. ". Understand "cima", "islotes", "islas", "animales", "animal", "tierras" and "limites" as the montana5.

Instead of taking the piedras:
	move the piedra to player;
	say "Coges una piedra.".

Section 4 - La isla

The islas is a region. The Isla, the Isla2, the Isla3 and the Isla4 are in the islas.

The vegetacion is a backdrop in the islas. The description is "Multitud de árboles frutales y flores de vivos colores te sorprenden a tu paso, ¡es un auténtico paraiso!.". Understand "arboles", "plantas", "flores", "flor", "bosque" and "oceano" as the vegetacion.

The arena is a backdrop in the islas. The description is "La playa está cubierta de fina arena, que se te escurre entre los dedos.". 

The sol is a backdrop. The sol is everywhere. The description is "El sol se muestra imponente en mitad del cielo azul.".

Isla is a room. The printed name of Isla is "Costa de la isla". The description is "[if unvisited]Has llegado a una exótica isla en mitad de la inmensidad del mar. Te sorprende la singular belleza de estas costas, que se extienden de este a oeste hasta donde alcanza la vista.[else]La línea de la costa se extiende de este a oeste en esta paradisíaca isla, hasta donde alcanza la vista.".

Isla2 is west of Isla and east of Isla4. The printed name of Isla2 is "Costa de la isla". The description is "[if unvisited]Continúas explorando la isla. Te sorprende la singular belleza de estas costas, que se extienden de este a oesta hasta donde alcanza la vista.[else]La vegetación es más densa en esta parte de la isla y te obliga a meterte en el agua hasta casi la cintura. La línea de la costa continúa de este a oeste.".

Isla3 is west of Isla4 and east of Isla. The printed name of Isla3 is "Costa de la isla". The description is "[if unvisited]Sigues explorando la isla. Te sorprende la singular belleza de estas costas, pero más adentro, al norte, te llama la atención un camino que conduce a un espeso bosque.[else]La isla se extiende en una larga playa de fina arena hasta donde alcanza la vista. Más adentro, al norte, puedes ver un camino que conduce a un espeso bosque.".

Isla4 is east of Isla3 and west of Isla2 and south of Bosque2. The printed name of Isla4 is "Costa de la isla". The description is "[if unvisited]Continúas explorando la isla. Te sorprende la singular belleza de estas costas, que se extienden de este a oesta hasta donde alcanza la vista.[else]La isla se extiende en una larga playa de fina arena hasta donde alcanza la vista.".

Some tablones are in Isla4. They are fixed in place. "Unos tablones de madera procedentes de un naufragio se encuentran tirados por la arena.". The description is "Restos de un naufragio, y por su aspecto no hace mucho que llegaron a estas costas.". Understand "tablas", "tablon", "restos" and "naufragio" as the tablones.

The cantimplora is female. The cantimplora can be llena or vacia. The cantimplora is vacia. The description is "Una sorprendente cantimplora de aluminio, [if vacia]totalmente vacía.[else] llena de agua.". Understand "agua" as the cantimplora.

[Desambigüación del agua de la cantimplora para que no entre en conflicto con el agua del mar ni el riachuelo.]
Does the player mean drinking the mar: it is very unlikely. 
Does the player mean drinking the cantimplora when the player is in Bosque2: it is very unlikely. 
Does the player mean examining the cantimplora when the player is in Bosque2: it is very unlikely. 

Check drinking the cantimplora:
	if the cantimplora is llena:
		say "Te bebes el agua de la cantimplora.";
		now the cantimplora is vacia;
		rule succeeds;
	otherwise:
		say "¡Pero si está vacía!";
		rule succeeds.

Instead of turning or touching or pushing or pulling the tablones, try taking the tablones.
Instead of taking the tablones for the first time:
	move the cantimplora to Isla4;
	say "Los tablones pesan demasiado, pero al moverlos has dejado al descubierto una cantimplora.".
Instead of taking the tablones, say "Los tablones pesan demasiado para llevarlos tu solo.".


Bosque2 is north of Isla3. The printed name of Bosque2 is "Bosque de la isla". The description is "[if unvisited]Has llegado a un exótico bosque. Las plantas, los árboles y las flores de vivos colores te hacen sentir como si estuvieras en un paraíso.[else]Contemplas la gran variedad de vegetación que hay en la isla, algunas plantas jamás las habías visto antes. Más allá, al sur, se vislumbra la costa.".

The riachuelo is fixed in place in Bosque2. "Un pequeño riachuelo cruza serpenteando el bosque.". The description is "El agua del pequeño riachuelo fluye limpia y clara.". Understand "rio", "agua", "caudal" and "fondo" as the riachuelo.

Instead of turning or touching or pushing or pulling the riachuelo, try taking the riachuelo.
Instead of putting the riachuelo on the cantimplora, try taking the riachuelo.
Instead of llenaring the cantimplora when the player is in Bosque2, try taking the riachuelo. [definimos verbo llenaring en Vocabulario]

Check taking the riachuelo:
	if the player carries the cantimplora:
		say "Llenas la cantimplora con el agua del riachuelo.";
		now the cantimplora is llena;
		rule succeeds;
	otherwise:
		say "Coges el agua del riachuelo con tus manos... y se escurre entre tus dedos.";
		rule succeeds.


Instead of drinking or eating the riachuelo for the first time, say "El agua del riachuelo calma tu sed, ¡qué buena está!".
Instead of drinking or eating the riachuelo, say "Ya he bebido suficiente.".
[Instead of doing something other than examining to the riachuelo, say "Tal vez lo mejor sería tratar de coger el agua... si encontraras una cantimplora podrías tratar de llenarla...".]

Section 4.1 - El mar

The mar is a backdrop in the islas. The description is "Estas aguas son tan bellas como peligrosas, piensas mientras observas la línea de la costa, allá a lo lejos.". Understand "costa", "costas", "playa", "aguas", "agua", "linea" and "oceano" as the mar.

Instead of nadaring in the barco, try nadaring en the mar.

Instead of nadaring en the mar in the presence of the barco:
	say "Decidido y sin temor te adentras en el mar, nadando hacia el enigmático galeón...";
	wait for any key;
	move the player to galeon;
	rule succeeds.
	
Instead of nadaring en the mar:
	say "Decidido y sin temor te adentras en el mar, nadando hacia la costa...[paragraph break]";
	wait for any key;
	if a random chance of 1 in 5 succeeds:
		say "Pero de repente observas una amenazadora aleta de tiburón que se aproxima hacia ti... ¡intentas huir con todas tus fuerzas! Pero...[paragraph break]";
		end the story saying "Mueres en las fauces del tiburón.";
	otherwise:
		say "Finalmente, y tras un gran esfuerzo, llegas a la playa...[paragraph break]";
		wait for any key;
		now the player is in Playa.

Instead of nadaring in the islas, try nadaring en the mar.

Section 4.2 - La llave de oro

Some rocas are in Isla2. They are scenery. The description is "Las rocas muestran la erosión que las olas del mar han provocado en ellas. Muestran, en definitiva, el paso del tiempo.". Understand "roca", "erosion" and "tiempo" as the rocas.
A llave oro is female in Isla2. The printed name of llave oro is "llave de oro". The description is "¡Brillante!". Understand "llave de oro" as llave oro.
Rule for printing room description details of llave oro:
if the Isla2 is unvisited, say ", medio escondida entre las rocas, por";
omit contents in listing.

Section 5 - El aula

The aula is a room. It is female. The printed name of the aula is "Aula de historia". The description is "Estás en clase de historia. Todos tus compañeros te miran divertidos al ver que te has vuelto a dormir en plena clase.". 

Some alumnos are here. They are scenery. The description is "Tus compañeros de clase se están riendo de ti. Te entran ganas de salir de clase...". Understand "companeros" as the alumnos.

The clase is scenery. The clase is here. The description is "El aula, demasiado grande para tan pocos alumnos, te parece aún más grande tras haberte quedado dormido y ser ahora el hazmerreír de tus compañeros. El profesor, con su actitud severa y socarrona tampoco te ayuda a sentirte mejor. ¡Se estaba tan bien durmiendo! Tal vez puedas continuar tu sueño saliendo de aquí". Understand "aula" as the clase.

Instead of going outside from the aula for the first time:
say "Sales corriendo de clase, escuchando las hirientes risas de tus compañeros y la amenaza de suspenso del profesor. Te da igual, nunca te ha gustado la historia... y no soportas que se rían a tu costa.[paragraph break]";
wait for any key;
say "Tal vez nunca tuviste a ningún buen profesor que te explicara que la Historia, con mayúscula, era algo más que una sucesión de calamidades. Nunca tuviste aun [bold type]Duby[roman type], a un [bold type]Dumézil[roman type] o a un [bold type]Mircea Elíade[roman type] que te explicara epistemología, discurso mítico e integrado o la trifuncionalidad indoeuropea.[paragraph break]";
wait for any key;
say "Por eso sueñas. En tu imaginación la historia es una aventura, un desafío, una emoción. En tus sueños los nombres de reyes, dioses y conquistadores se mezclan y producen fantasiosos relatos donde la búsqueda de tesoros, el rescate a princesas y la caza de dragones son los ingredientes principales.[paragraph break]";
wait for any key;
say "Esa es tu visión de la historia... o lo que es lo mismo, por aquél entonces no sabías aún que querías ser escritor, pero las historias brotaban de tu mente... solo que no tenías consciencia de ello, no te ponías a escribirlo. Tampoco nadie te dijo que podías escribirlo, nadie te ayudó a pensar.[paragraph break]";
wait for any key;
say "Te daban los datos, las definiciones, las consecuencias... pero no los argumentos, las causas, las dudas. Nadie te dio clases para hacerte preguntas, convivir con la duda y la incertidumbre... y así estás ahora.[paragraph break]";
wait for any key;
say "En este momento de tu historia, tienes tantas dudas como temor a saber las respuestas. Por eso, solo te apetece dormir... porque tal vez en el sueño se disuelvan las dudas y desaparezca el miedo.";
wait for any key;
now the player is in parque.

The parque are outside from the aula. The printed name of the parque is "En el parque". The description is "Te encuentras en un pequeño parque cercano al colegio, en la soledad del momento percibes la fresca brisa matinal, el canto de algunos pajarillos y el ir y venir de hombres y mujeres muy atareados, yendo a sus trabajos, a la compra o simplemente simulando estar muy ocupados."

The colegio is here. The colegio is scenery. The description is "A unos pocos metros tienes la entrada al colegio, pero no quieres entrar mientras dure la clase de historia.".
Some pajarillos are here. They are scenery. The description is "Algunos pajarillos cantan, felices ellos, no parecen tener dudas de ningún tipo.".
The brisa is here. The brisa is scenery. The description is "Una brisa algo más que fresca hace que te friegues las manos y te abrigues bien con tu ropa. ¡Tienes las orejas y la punta de la nariz casi heladas!" Understand "calle" and "frio" and "arboles" as the brisa.
Some personas (f) are here. They are scenery. The description is "De aquí para allá, hombres y mujeres van de un lado a otro, como pollos sin cabeza, haciendo rodar al mundo. Ellos no lo saben, pero forman también parte de la historia, solo que no saldrá explicada en los libros, ni habrá quien la estudie, si a caso algún antropólogo despistado... ¿quién sabe?". Understand "hombres" and "mujeres" as the personas.

Instead of going inside from the parque when the profesor is in aula, say "No te apetece volver a clase. Aquí se está bien. Solo te apetece dormir...".
Instead of going inside from the parque when the profesor is in galeon:
	say "Entras en el colegio, todavía te quedan muchas cosas que aprender. Aunque no te guste la asignatura de historia, ni las matemáticas, ni la clase de lengua...[paragraph break]";
	wait for any key;
	say "Empiezas a cuestionar la forma que tienen los profesores de enseñar. En realidad, no enseñan, más bien vomitan datos. Son como máquinas, en ningún caso se paran a pensar, ni te hacen pensar. Todo lo que dicen lo han leído en los libros, pero no han vivido nada de lo que cuentan.[paragraph break]";
	wait for any key;
	say "Tú, en cambio, vives tus sueños. Sabes que hay mucho más que simples definiciones, nombres y determinadas cantidades, fechas y demás datos. Las cosas no son como nos las cuentan, sino como nosotros las vivimos.[paragraph break]";
	wait for any key;
	say "¿Cuál era el tesoro? Tal vez para ti sea algo material, Sebastián... o tal vez no, pues de ti depende el darle valor a lo que te rodea según tu propio baremo.[paragraph break]";
	wait for any key;
	say "Tal vez quieras contar que lo importante no es el tesoro, y que como Ulises en su viaje a Ítaca, lo importante es la experiencia que se tiene en su búsqueda.";
	wait for any key;
	end the story finally.
	


Section 6 - El barco

The barco is fixed in place. The description is "Un majestuoso galeón español se encuentra cerca de la costa. Tal vez pudieras llegar a él a nado, antes de que se aleje demasiado...".

Rule for printing room description details of barco:
say " español navegando por la costa, cerca de";
omit contents in listing.


galeon is a room. The printed name of galeon is "El barco Guadalupe". The description is "Te encuentras en la cubierta de un galeón español, que viento en popa a toda vela, surca el mar que no vuela, a manos de un marinero bribón. [if unvisited]No eres el mejor de los grumetes, pues nunca antes habías montado en un barco, y no sabes ni dónde está la proa o la popa, ni lo que es babor o estribor. Pero tal vez el marinero te ayude...".

The timon is here. The timon is scenery. The printed name of the timon is "timón". The description is "El marinero sujeta firmemente el timón.".
Some velas are here. They are female and scenery. The description is "Las velas están parcialmente desplegadas, así que el barco navega muy lento.". Understand "vela" as the velas.

Instead of listening in the presence of the marinero, say "Escuchas la alegre canción del marinero.".

The proa is female and scenery in galeon. The description is "La proa y la popa del barco... nunca has sabido cuál es la parte de delante y la de detrás.". Understand "isla", "mar", "playa", "aguas", "agua", "popa", "estribor", "babor" and "costa" as the proa.

Instead of nadaring in the galeon, try nadaring en the proa.

Instead of nadaring en the proa for the first time:
	say "Decidido y sin temor te adentras en el mar, nadando hacia la lejana isla...[paragraph break]";
	wait for any key;
	say "De repente, en mitad de la travesía, te das cuenta... ¡el mar está infestado de tiburones! Nadas todo lo rápido que puedes hasta llegar exhausto a la costa... ¡esta vez has tenido suerte![paragraph break]";
	wait for any key;
	now the player is in Isla4.

Instead of nadaring en the proa:
	say "Decidido y sin temor te adentras en el mar, nadando hacia la lejana isla...[paragraph break]";
	wait for any key;
	if a random chance of 1 in 5 succeeds:
		say "Pero de repente observas una amenazadora aleta de tiburón que se aproxima hacia tu posición... ¡intentas huir con todas tus fuerzas! Pero...[paragraph break]";
		end the story saying "Has muerto";
	otherwise:
		say "Finalmente, y tras un gran esfuerzo, llegas a la costa. Contemplas maravillado la paradisíaca isla...[paragraph break]";
		wait for any key;
		now the player is in Isla4.
		
Part 3 - Reparto

Section 1 - El jugador

conquistador is a man in the Bosque. The printed name of conquistador is "Hernán Cortés". The description is "Eres un conquistador español del siglo XIV, tu nombre es Hernán Cortés y te encuentras perdido en una tierra desconocida.". The player is conquistador. Understand "hernan" and "cortes" and "hernan cortes" as the conquistador.

Sebastian is a man in the Aula. The printed name of Sebastian is "Sebastián". The description is "Eres un alumno de instituto, aburrido en plena clase de historia. Piensas que lo mejor que puedes hacer es seguir durmiendo..."

Section 1.1 - Despertar y dormir al jugador

Before waking up:
	if the player is in aula or the player is in galeon:
		say "Estoy despierto... ¿o estoy soñando?";
		rule succeeds;
	if the player is conquistador and the parque is unvisited: 
		say "Oyes una voz a lo lejos que te dice: 'Sebastián! ¡Despierta, Sebastián! Otra vez te has quedado dormido en clase... [bold type]¡Sebastián!'[roman type][paragraph break]";
		wait for any key;
		say "Aturdido, te despiertas de un sobresalto. Te habías quedado completamente dormido en clase de historia, justo cuando el profesor estaba explicando todo el rollo de la colonización... ¿a quién le importará, si ya hace tanto de eso?[paragraph break]'Sebastián, ¿me puedes decir de qué estaba hablando?' te pregunta airado el profesor Antonio...";
		wait for any key;
		move Sebastian to aula;
		now the player is Sebastian;
		rule succeeds;
	if the player is conquistador and the parque is visited: 
		say "Lentamente te desperezas...[paragraph break]";
		wait for any key;
		move Sebastian to parque;
		now the player is Sebastian;
		rule succeeds;
	if the player is Sebastian and the naufrago is recuperado: 
		say "Lentamente te desperezas...[paragraph break]";
		wait for any key;
		now the player is in parque;
		rule succeeds;
	otherwise:
		 say "Creo que ya estoy despierto...";
		rule succeeds.
		

Before sleeping:
	if the player is in aula:
		say "No puedo quedarme dormido aquí...";
		rule succeeds;
	if the profesor is in galeon:
		say "Ya no tengo sueño, no quiero dormir más.";
		rule succeeds;
	if the player is Sebastian and the naufrago is recuperado: 
		say "Vuelves a soñar, otra vez... pero en el sueño, ahora eres tú el protagonista...[paragraph break]";
		wait for any key;
		remove tablones from play;
		remove naufrago from play;
		now the description of conquistador is "Tu antiguo yo en el sueño, el conquistador Hernán Cortés, parece una estatua de sal, como un maniquí con pose mayestática, sus ojos sin pupilas se dirigen al mar, pero no tienen vida.";
		move the cofre to Isla;
		move the mapa to cofre;
		move the llave oro to Isla2;
		move barco to Isla4;
		move the player to Isla4;
		rule succeeds;
	if the player is Sebastian and the naufrago is moribundo: 
		say "Lentamente tus ojos se cierran de nuevo y te sumerges en tu sueño...[paragraph break]";
		wait for any key;
		now the player is conquistador;
		rule succeeds;
	otherwise:
		 say "Creo que ya estoy durmiendo...";
		rule succeeds.
		
Understand "duermete", "dormir" as sleeping.

Understand "agarra [something]" as taking.


Section 2 - El náufrago

naufrago is a man in the Isla. The naufrago can be moribundo or recuperado. The naufrago is moribundo. The printed name of naufrago is "un náufrago". The description is "Un hombre vestido con harapos está tumbado sobre la arena, moribundo.". Understand "hombre", "arapos", "moribundo" and "antonio" as the naufrago. 

Rule for printing room description details of naufrago:
if the Isla is unvisited, say " moribundo tumbado sobre la arena, por ";
if the cofre is carried and Isla is visited, say " mirando con sorpresa tu misterioso cofre, por ";
omit contents in listing.

Instead of touching naufrago, say "El hombre sigue vivo, tal vez puedas ayudarle dándole un poco de agua.". 
Instead of attacking naufrago, say "El hombre no representa ningún peligro.".

Instead of telling someone about something, try asking the noun about it. Instead of answering the noun that something, try asking the noun about it. 

After asking naufrago about "hola", say "El hombre te observa detenidamente y te pregunta '¿Eres amigo o enemigo?.'".
After asking naufrago about "amigo": say "El hombre sonríe con debilidad y te dice 'Mi nombre es Antonio Velasco y hace dos días arribé a estas costas, tras un naufragio...'";
now the printed name of naufrago is "Antonio".
After asking naufrago about "naufragio", say "'Los piratas nos abordaron y hundieron el barco, creo que soy el único superviviente...'".
After asking naufrago about something, say "El hombre no atiende a lo que dices, prueba con otras palabras".

Instead of singing when the naufrago is in location, say "El hombre se tapa los oídos y dice: 'Por dios, ¡haz el favor de callarte!'".
	
Instead of throwing the piedra at the naufrago, say "El hombre no representa ningún peligro.".

After asking the naufrago about something when the naufrago is recuperado: try waking up.


Section 3 - La serpiente

The serpiente is in Bosque. The serpiente is female and an animal. The description is "Una serpiente se aproxima hacia ti desde el sur, con aspecto amenazador...".

Rule for printing room description details of serpiente:
if the Bosque is unvisited, say " aproximándose hacia ti desde el sur,";
otherwise say " siseando amenazadoramente, impidiéndote el paso hacia el sur,";
omit contents in listing.

Instead of going south in the presence of the serpiente:
	say "Intentas rodear a la serpiente para ir al sur, pero esta se abalanza hacia ti con los colmillos y...";
	end the story saying "¡Estás muerto!".
	
Instead of throwing the piedra at the serpiente:
	say "Lanzas la piedra a la serpiente, que retrocede asustada, perdiéndose por entre el follaje del bosque...";
	remove the serpiente from play;
	remove the piedra from play.	
	

Section 4 - El profesor

A profesor is a man in the aula. "El profesor Antonio te mira con severidad.". The description is "Tiene un gran parecido con el náufrago de tu sueño.". Understand "Antonio" as the profesor.

After asking the profesor about a topic listed in the Table of profesor_conversacion, say "El profesor dice: [muse entry]."

Table of Profesor_conversacion 
Topic   	Muse   
"hola" or "explicacion" or "pregunta"   	"'¡Te he hecho una pregunta! ¿Qué es lo que estaba explicando?'"   
"historia"	"'¡Muy bien! Por lo menos sabes en qué aula estás, ¿puedes decirnos de qué historia hablamos?'"
"colonizacion"   	"'Exacto, Sebastián... veo que por lo menos sabía a qué venías a clase. ¿Quién fue Colón?'"   
"colon" or "cristobal colon"   	"'Te he hecho una pregunta, ¿quién fue Colón?'"   
"descubrimiento" or "descubridor"   	"'Colón fue un descubridor, Sebastián... ¿y quién fue Hernán Cortés?'"   
"conquistador" or "hernan" or "hernan cortes"   	"'Hernán Cortés fue el que conquistó el imperio azteca, lo que hoy es México.'"  
"no se" or "no lo se" or "ayuda"	"'¿Cómo que no sabes? ¡Hablamos del descubrimiento de América!'"
"america" or "continente"	"'Sí, América, lo que descubrió Colón ¿te suena el nombre, Sebastián?'" 

Section 5 - El marinero del barco

A marinero is a man in the galeon. "Un alegre marinero maneja el timón del barco.". The description is "El marinero resulta ser el náufrago moribundo de antes, que parece estar totalmente recuperado. Silba contento una vieja canción.". Understand "Antonio" as the marinero.

After asking the marinero about a topic listed in the Table of marinero_conversacion, say "El marinero dice: [muse entry]."

Table of marinero_conversacion 
Topic   	Muse   
"hola/explicacion/pregunta"   	"'¡Hola de nuevo, Sebastián! Nos volvemos a encontrar... dime... ¿traes aquél viejo cofre que encontraste en la playa?'"   
"cofre/llave/playa/guadalupe/barco"	"'¡En el cofre debe haber un mapa del tesoro, si Romualdo Guimaraes no andaba errado! Vuelve a por él a nado, tal vez se encuentre en la isla que dejamos atrás...'"
"tesoro/mar/romualdo"   	"'¡Un sinfín de riquezas nos aguardan, mi joven grumete... ¿¡a qué esperas!? ¡Dame el mapa del tesoro y pongamos rumbo a una nueva aventura!'"   
"antonio/naufrago/marinero"   	"'Sí, Sebastián, soy yo, Antonio... tu profesor, náufrago y ahora marinero... no me preguntes porqué me has elegido a mí, pero así lo has querido en tu sueño.'"   
"timon/rumbo/velas/isla"   	"'Vamos donde te indique tu propio sueño, pues todo esto no es más que artificio, Sebastián.'"   
"proa/delante/parte delantera"   	"'La proa, Sebastián, es la parte delantera, la que hace avanzar al barco cortando las olas del mar.'"  
"popa/atras/parte trasera"   	"'La popa es la parte posterior del barco, ¿y sabrías decirme cuál es la parte de estribor y cuál la de babor?'"  
"estribor/derecha"   	"'Grumete, la parte de estribor es la parte derecha del barco, mirando en el sentido de la marcha, o sea, a la proa.'"  
"babor/izquierda"   	"'Grumete, la parte de babor es la parte izquierda del barco, mirando en el sentido de la marcha, o sea, a la proa.'"  
"no se" or "no lo se" or "ayuda"	"'¡Pareces perdido! Encuentra el viejo cofre que viste cuando eras Hernán Cortés, así podré poner rumbo al lugar que indique el mapa que contiene ese cofre.'"
"mapa"	"'No te preocupes por eso, a algún lugar nos conducirá ese mapa...'" 
"mojado/seco/inservible/empapado"	"Amigo mío, no importa. Lo que cuenta es el viaje."

Instead of attacking naufrago, say "¡El marinero es tu amigo!".

Instead of giving the cofre to the marinero, say "'No es el cofre lo que quiero, Sebastián, sino el mapa que contiene.'".
Instead of giving the llave oro to the marinero, say "'Con esa llave podrás quitar el cerrojo del cofre para poder abrirlo, Sebastián.'".

Instead of giving the mapa del tesoro to the marinero when the mapa del tesoro is mojado:
	say "El hombre coge el mapa y lo observa... 'Sebastián, este mapa ya no sirve para nada...'[paragraph break]";
	wait for any key;
	say "'Pero no pasa nada, amigo mío. Vamos a poner rumbo a lo desconocido. Tal vez encontremos un tesoro o la muerte, pero una cosa está clara: nuestro destino no está escrito.'[paragraph break]";
	wait for any key;
	say "Un barco errante cruza el mar ignoto, su destino es una incertidumbre.  ¿Qué escondía la isla misteriosa? Muchas son las preguntas y tal vez no haya una respuesta. Pero ¿cuál es el tesoro? Un tesoro es algo muy valioso, del cual solo alcancamos a saber el valor cuando lo perdemos. Mientras tanto, un barco errante cruza el mar ignoto...";
	wait for any key;
	end the story finally.
	
Instead of giving the mapa del tesoro to the marinero when the mapa del tesoro is seco:
	say "El hombre coge el mapa y lo observa... ¡Sebastián, gracias a este mapa vamos a encontrar un tesoro! El marinero da un golpe al timón y cambia el rumbo de la marcha. Las velas se desplegan y el viento sopla fuerte. El barco va ganando velocidad dirigiéndose a alta mar.'[paragraph break]";
	wait for any key;
	say "Te alejas de la isla misteriosa, dejando atrás a Hernán Cortés, a las dudas y a la incertidumbre. El cielo azul, nítido y limpio, te aclara las ideas. Nuevas preguntas surgirán, nuevos temores saldrán a flote, pero ahora ha llegado el momento de despertar, de vivir...[paragraph break]";
	wait for any key;
	say "Te despiertas lentamente, sin saber aún muy bien qué es real y qué es aún vigilia. Te frotas los ojos y estiras tu cuerpo, ya no hace tanto frío y ahora tienes calor. Has tenido un sueño extraño, casi has dormido una hora y... ¡¡endrías que espabilarte para entrar en la siguiente clase.[paragraph break]";
	wait for any key;
	move the profesor to galeon;
	move the player to the parque;
	rule succeeds.
	
	
Part 4 - Nudo

Section 1 - Escena del náufrago

Tener sed is a scene. Tener sed begins when the Isla is visited for the first time.
Tener sed ends happily when the naufrago is recuperado.
Tener sed ends sadly when the time since Tener sed began is 40 minutes.

[When Tener sed begins:
	change contador to 0.]

When Tener sed begins:
	now contador is 0.

When Tener sed ends happily:
	say "El náufrago empieza a tener mejor aspecto, te mira agradecido[line break]-¡Gracias, amigo! -te dice el hombre, levantándose con dificultad."

[When Tener sed ends sadly:
	end the game saying "El náufrago cae inconsciente en la arena, muerto de sed. Entonces despiertas sobresaltado... ¡ya no volverás a tener el mismo sueño!"]

When Tener sed ends sadly:
	end the story saying "El náufrago cae inconsciente en la arena, muerto de sed.'"

The contador is a number that varies.
Every turn during Tener sed:
	increase contador by 1;
	if contador is 1, say "-¡Tengo sed! Ahh...- le oyes decir.";
	if contador is 9, say "El náufrago parece estar sediento, apenas puede apoyarse en la arena.";
	if contador is 13, say "Aún puedes escuchar los lamentos del náufrago...";
	if contador is 17, say "Aún puedes escuchar los lamentos del náufrago...";
	if contador is 22, say "Los lamentos del náfrago cada vez son más débiles...";
	if contador is 29, say "Deberías pensar en darle algo de agua al náufrago...";
	if contador is 33, say "Deberías darle algo de agua al náufrago rápidamente, o caerá inconsciente.";
	if contador is 38, say "El náufrago apenas está ya consciente...".

Instead of giving the cantimplora to the naufrago when the cantimplora is llena:
	say "El hombre coge nerviosamente la cantimplora con las dos manos y bebe de ella hasta la última gota...";
	now the naufrago is recuperado;
	now the description of naufrago is "Un hombre vestido con arapos, ahora tiene mejor aspecto. Es un tipo alto y delgado que parece haber sobrevivido a terrible naufragio.";
	now the cantimplora is vacia.

Instead of giving the cantimplora to the naufrago when the cantimplora is vacia:
	say "El hombre coge nerviosamente la cantimplora con las dos manos... ¡y ve que está vacía![paragraph break]Encolerizado te la arroja, aunque sin fuerzas, y te implora '¡Dame agua, por favor!'";
	move the cantimplora to Isla.	

Section 2 - El mapa del tesoro

In the cofre is the mapa del tesoro. The mapa del tesoro can be seco or mojado. The mapa del tesoro is seco. The description is "¡Parece un mapa auténtico! En el mapa hay varias anotaciones: un dibujo, una cruz, un símbolo y un escrito. Tal vez si logro descifrarlo todo encontraré un tesoro... ¡y seré rico! ¡Ja!". 

A anotacion is a kind of thing. The plural of anotacion is anotaciones. They are scenery. Some anotaciones in the mapa del tesoro are defined by the Table of tabla_anotaciones. The description of a anotacion is "[if the mapa del tesoro is seco]Bajo [palabra], está manuscrito lo siguiente: [descripcion].[otherwise]El mapa está mojado e inservible. ¡Deberías haber tenido más cuidado al cruzar a nado la costa!". 

    Table of tabla_anotaciones
    anotacion   	palabra   	descripcion   
    a dibujo   	"el dibujo de la isla"   	"Hay varias islas en este archipiélago del infierno, pero la isla del tesoro es la que está más al norte, y la más peligrosa..."   
    a cruz   	"una cruz en el mapa"   	"El tesoro se encontró en el barco 'Guadalupe', que fue atacado por los salvajes... si encuentro los restos del barco, encontraré la isla"   
    a simbolo   	"un símbolo tribal"   	"Este símbolo es la representación del dios de los salvajes que custodian el tesoro, tal vez si me lo tatuara creerían que soy su dios..."   
    a escrito   	"un escrito"   	"Romualdo Guimaraes, que murió persiguiendo un sueño. Si encuentras este mapa, encontrarás el tesoro o tu muerte."   

The cruz is female.

Before listing contents while taking inventory: group anotaciones together. Rule for grouping together anotaciones: say "en el mapa puedes ver el dibujo de una isla, una cruz, un símbolo y un escrito.".

Before nadaring en the costa:
	if the mapa is carried:
		now the description of the mapa del tesoro is "El agua lo ha destrozado... apenas se pueden ver las anotaciones... ";
		now the mapa is mojado.

Before nadaring en the mar:
	if the mapa is carried:
		now the description of the mapa del tesoro is "El agua lo ha destrozado... apenas se pueden ver las anotaciones... ";
		now the mapa is mojado.

Part 5 - Vocabulario

[Nadar]
nadaring is an action applying to nothing. 
understand "nada" and "bucea" as nadaring.
Report nadaring:
say "No hay suficiente agua aquí, ¿dónde he de nadar?".

nadaring en is an action applying to one thing.
understand "nada [something]", "nada a [something]", "nada en [something]", "nada hacia [something]",   "nadia hacia la [something]", "bucea [something]",  "bucea a [something]", "nada en [something]", "bucea hacia [something]" and "bucea hacia la [something]" as nadaring en.
Check nadaring en something:
say "No puedo nadar en [the noun], mejor será nadar en el mar..." instead.

[Llenar la cantimplora]
llenaring is an action applying to one thing. Understand "llena [something]" as llenaring.
report llenaring: say "No parece que [the noun] pueda llenarse, ¿qué pretendes hacer exactamente?.".

[Rezar]
rezaring is an action applying to nothing. 
understand "reza" as rezaring.
report rezaring:
say "¡Quiera Dios que mis plegarias sean escuchadas!" instead.

Instead of rezaring for the first time, say "Alzas tus brazos al cielo y suplicas al altísimo: 'Padre nuestro, que estás en el cielo, santificado sea tu Nombre; venga a nosotros tu reino...'".

[Cantar]
Singing is an action applying to nothing. Understand "canta", "recita", "canto", "llora", "grita" as singing. 
Report singing: say "Ahora mismo no tienes muchas ganas de cantar.".

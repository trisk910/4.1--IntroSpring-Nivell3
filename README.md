# 4.1--IntroSpring-Nivell3

#Nivell 1

- Exercici Spring i Maven
  
Aquest exercici és un primer contacte amb Spring i Maven.

Accedeix a la pàgina ->https://start.spring.io/, i genera un projecte Spring boot amb les següents característiques:


PROJECT (gestor de dependències)

Maven.

LANGUAGE

Java.

SPRING BOOT

La darrera versió estable.

PROJECT METADATA

Group

cat.itacademy.s04.t01.n01

Artifact

S04T01N01

Name

S04T01N01

Description

S04T01N01

Package name

cat.itacademy.s04.t01.n01

PACKAGIN

Jar

JAVA

Mínim versió 11 

Dependències:

Spring Boot DevTools

Spring Web


Importa’l a Eclipse amb l’opció File > Import > Existing Maven Project.

A l’arxiu application.properties, configura la variable server.port amb el valor 9000.

Convertirem aquesta aplicació en una API REST:
Depenent del package principal, crea un altre subpackage anomenat controller, i dins seu, afegeix la classe HelloWorldController.
Haurà de tenir dos mètodes:

String saluda
String saluda2

Aquests dos mètodes rebran un paràmetre String anomenat nom, i retornaran la frase:

“Hola, “ + nom + “. Estàs executant un projecte Maven”.


El primer mètode respondrà a una petició GET, i haurà de ser configurat per a rebre el paràmetre com un RequestParam. El paràmetre "nom" tindrà el valor per defecte “UNKNOWN”.

Haurà de respondre a:

http://localhost:9000/HelloWorld
http://localhost:9000/HelloWorld?nom=El meu nom

 

El segon mètode respondrà a una petició GET, i haurà de ser configurat per a rebre el paràmetre com una PathVariable. El paràmetre "nom" serà opcional.

Haurà de respondre a:

http://localhost:9000/HelloWorld2
http://localhost:9000/HelloWorld2/elmeunom

Practicar Comandes Bàsiques de Maven
Assegura't que Maven està instal·lat i configurat al teu sistema. Obre una terminal (des del teu IDE o des de la línia de comandes de Windows, Mac, etc.) i navega al directori del teu projecte. L'objectiu és que et familiaritzis amb algunes comandes importants de Maven:

Compilar el Projecte: mvn compile
Empaquetar el Projecte: mvn package
Netejar el Projecte: mvn clean


Nivell 2






- Exercici Spring i Gradle

Veuràs que aquest nivell és quasi idèntic al nivell 1, però fent servir Gradle com a Gestor de dependències.

Accedeix a la pàgina ->https://start.spring.io/, i genera un projecte Spring boot amb les següents característiques:

PROJECT (gestor de dependències)

Gradle.

LANGUAGE

Java.

SPRING BOOT

La darrera versió estable.

PROJECT METADATA

Group

cat.itacademy.s04.t01.n02

Artifact

S04T01N02

Name

S04T01N02

Description

S04T01N02

Package name

cat.itacademy.s04.t01.n02

PACKAGIN

Jar

JAVA

Mínim versió 11 

Dependències:

Spring Boot DevTools

Spring Web


Importa’l a Eclipse amb l’opció File > Import > Existing Gradle Project.


A l’arxiu application.properties, configura la variable server.port amb el valor 9001.


Convertirem aquesta aplicació en una API REST:
Depenent del package principal, crea un altre subpackage anomenat controller, i dins seu, afegeix la classe HelloWorldController.

Haurà de tenir dos mètodes:

String saluda
String saluda2


Aquests dos mètodes rebran un paràmetre String anomenat "nom" i retornaran la frase:

“Hola, “ + nom + “. Estàs executant un projecte Gradle”.

El primer mètode respondrà a una petició GET, i haurà de ser configurat per a rebre el paràmetre com un RequestParam. El paràmetre "nom" tindrà el valor per defecte “UNKNOWN”.

Haurà de respondre a:

http://localhost:9001/HelloWorld
http://localhost:9001/HelloWorld?nom=El meu nom
 

El segon mètode respondrà a una petició GET, i haurà de ser configurat per a rebre el paràmetre com una PathVariable. El paràmetre "nom" serà opcional.

Haurà de respondre a:

http://localhost:9001/HelloWorld2
http://localhost:9001/HelloWorld2/el meu nom

Practicar Comandes Bàsiques de Gradle
Assegura't que Gradle està instal·lat i configurat al teu sistema. Obre una terminal (des del teu IDE o des de la línia de comandes de Windows, Mac, etc.) i navega al directori del teu projecte.

L'objectiu és que et familiaritzis amb algunes comandes importants de Gradle:

Compilar el Projecte: gradle build
Empaquetar el Projecte: gradle assemble
Netejar el Projecte: gradle clean
Executar l'Aplicació: gradle bootRun

 Molt Important

A més de l’enllaç a Git de la tasca resolta, hauràs d’incloure almenys dos enllaços diferents dels recursos que t’hem proporcionat al campus, que t’hagin servit o ho haguessin pogut fer, per resoldre la totalitat de la tasca o algunes parts.




#Nivell 3

- Exercici Postman

Es tracta de provar els anteriors projectes des de Postman.

Crea dos entorns:

-          Projecte Maven

-          Projecte Gradle

 

Ambdós entorns tindran dues variables:

-          Servidor, que en els dos casos tindrà el valor http://localhost

-          Port, que en el cas del projecte Maven tindrà el valor 9000, i en el cas del projecte Gradle, 9001.

 

Que has d’entregar? (4 arxius):

-          Els dos entorns exportats.

-          Una captura de pantalla per cada entorn, on es vegi l’execució des de Postman usant l’entorn i les variables definides en ells.

-          Pots provar l'URL: http://localhost:xxxx/HelloWorld/elmeunom, o qualsevol altra de les que admeten els dos projectes. (recorda que perquè l’execució funcioni correctament, hauràs de tenir en execució els dos projectes a Eclipse).

Executa des d’Eclipse els projectes creats als dos nivells anteriors, i mostra el retorn obtingut en cada projecte, quan crides a algunes de les peticions disponibles, fent servir els entorns creats i les seves variables.

Hauràs d’entregar dues captures de pantalla, una per l’execució de cada entorn, i dos arxius amb format JSON, amb els entorns exportats.
Executar l'Aplicació: mvn spring-boot:run

 Molt Important

A més de l’enllaç a Git de la tasca resolta, hauràs d’incloure al menys dos enllaços diferents dels recursos que t’hem proporcionat al campus, que t’hagin servit o ho haguessin pogut fer, per resoldre la totalitat de la tasca o algunes parts.

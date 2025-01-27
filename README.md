# Projecte Spring Boot: Maven i Gradle

## Descripció
Aquest repositori conté les solucions per als exercicis dels nivells 1, 2 i 3 relacionats amb Spring Boot utilitzant Maven i Gradle com a gestors de dependències. Els exercicis inclouen la configuració d’una API REST bàsica, la pràctica de comandes bàsiques de Maven i Gradle, i la validació mitjançant Postman.

---

## Nivell 1: Spring Boot amb Maven

### Característiques del projecte
- **Gestor de dependències**: Maven
- **Llenguatge**: Java
- **Spring Boot**: Darrera versió estable
- **Package**: JAR
- **Versió de Java**: Mínim 11

### Dependències:
- Spring Boot DevTools
- Spring Web

### Configuració:
1. **Variable `server.port`:** Configurat a `9000` dins de l'arxiu `application.properties`.
2. **Estructura:**
   - Crea un package `controller` dins del package principal `cat.itacademy.s04.t01.n01`.
   - Afegir la classe `HelloWorldController` amb els següents mètodes:
     - `String saluda`: Respon a una petició GET a `http://localhost:9000/HelloWorld` amb un paràmetre `nom` (RequestParam, valor per defecte: `UNKNOWN`).
     - `String saluda2`: Respon a una petició GET a `http://localhost:9000/HelloWorld2/{nom}` amb un paràmetre `nom` opcional (PathVariable).

### Comandes Maven:
- **Compilar el projecte**: `mvn compile`
- **Empaquetar el projecte**: `mvn package`
- **Netejar el projecte**: `mvn clean`
- **Executar l’aplicació**: `mvn spring-boot:run`

### Enllaços d’ajuda:
- [Documentació Spring Boot](https://spring.io/projects/spring-boot)
- [Introducció a Maven](https://maven.apache.org/guides/index.html)

---

## Nivell 2: Spring Boot amb Gradle

### Característiques del projecte
- **Gestor de dependències**: Gradle
- **Llenguatge**: Java
- **Spring Boot**: Darrera versió estable
- **Package**: JAR
- **Versió de Java**: Mínim 11

### Dependències:
- Spring Boot DevTools
- Spring Web

### Configuració:
1. **Variable `server.port`:** Configurat a `9001` dins de l'arxiu `application.properties`.
2. **Estructura:**
   - Crea un package `controller` dins del package principal `cat.itacademy.s04.t01.n02`.
   - Afegir la classe `HelloWorldController` amb els següents mètodes:
     - `String saluda`: Respon a una petició GET a `http://localhost:9001/HelloWorld` amb un paràmetre `nom` (RequestParam, valor per defecte: `UNKNOWN`).
     - `String saluda2`: Respon a una petició GET a `http://localhost:9001/HelloWorld2/{nom}` amb un paràmetre `nom` opcional (PathVariable).

### Comandes Gradle:
- **Compilar el projecte**: `gradle build`
- **Empaquetar el projecte**: `gradle assemble`
- **Netejar el projecte**: `gradle clean`
- **Executar l’aplicació**: `gradle bootRun`

### Enllaços d’ajuda:
- [Documentació Spring Boot](https://spring.io/projects/spring-boot)
- [Introducció a Gradle](https://gradle.org/guides/)

---

## Nivell 3: Validació amb Postman

### Objectius:
1. Provar els projectes Maven i Gradle des de Postman.
2. Crear dos entorns Postman:
   - **Projecte Maven**:
     - Variable `Servidor`: `http://localhost`
     - Variable `Port`: `9000`
   - **Projecte Gradle**:
     - Variable `Servidor`: `http://localhost`
     - Variable `Port`: `9001`

### Passos:
1. Configura les variables a Postman.
2. Prova les peticions:
   - Exemple Maven: `http://localhost:9000/HelloWorld?nom=El meu nom`
   - Exemple Gradle: `http://localhost:9001/HelloWorld2/elmeunom`
3. Exporta els entorns i inclou:
   - **2 arxius JSON** amb els entorns exportats.
   - **Captures de pantalla** per cada entorn mostrant una petició correcta.

### Enllaços d’ajuda:
- [Introducció a Postman](https://www.postman.com/)
- [Documentació Postman per a entorns](https://learning.postman.com/docs/sending-requests/managing-environments/)

---

## Entrega
1. Codi dels projectes Maven i Gradle.
2. Enllaç a GitHub amb el repositori complet.
3. Arxius JSON dels entorns Postman exportats.
4. Captures de pantalla de les peticions correctes realitzades amb Postman.


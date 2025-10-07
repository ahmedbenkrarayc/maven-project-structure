# maven-project-structure

```
mon-projet/
│
├── src/
│   ├── main/
│   │   ├── java/         → code source principal
│   │   └── resources/    → fichiers de configuration
│   └── test/
│       ├── java/         → tests unitaires
│       └── resources/    → ressources de test
│
├── target/               → fichiers générés (classes compilées, .jar)
└── pom.xml               → fichier de configuration principal
```
---

```
pom.xml
│
├── <project>                → racine du fichier POM, contient toutes les informations du projet
│
├── <modelVersion>4.0.0</modelVersion>
│                            → version du modèle POM utilisé par Maven
│
├── <groupId>com.example</groupId>
│                            → identifiant unique du groupe ou organisation
│
├── <artifactId>demo</artifactId>
│                            → nom du projet ou de l’artefact
│
├── <version>1.0.0</version>
│                            → version du projet
│
├── <packaging>jar</packaging>
│                            → type de livrable : jar, war, pom…
│
├── <dependencies>           → liste des bibliothèques externes nécessaires au projet
│   └── <dependency>
│       ├── <groupId>junit</groupId>
│       │                       → groupe de la dépendance
│       ├── <artifactId>junit</artifactId>
│       │                       → nom de la dépendance
│       ├── <version>4.13.2</version>
│       │                       → version de la dépendance
│       └── <scope>test</scope> → portée (ici : uniquement pour les tests)
│
├── <build>                  → configuration des plugins et étapes de compilation
│   └── <plugins>
│       └── <plugin>         → exemple : plugin de compilation, packaging…
│
└── <repositories>           → dépôts où Maven va chercher les dépendances
    └── <repository>
        ├── <id>central</id>
        │                   → identifiant du dépôt
        └── <url>https://repo.maven.apache.org/maven2</url>
                            → URL du dépôt distant
```

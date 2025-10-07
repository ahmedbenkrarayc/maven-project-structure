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
├── <project>                → racine du fichier POM
│
├── <groupId>com.example</groupId>
│                            → identifiant unique du groupe ou organisation
│
├── <artifactId>demo</artifactId>
│                            → nom du projet
│
├── <version>1.0.0</version>
│                            → version du projet
│
├── <packaging>jar</packaging>
│                            → type de livrable (jar, war…)
│
├── <dependencies>           → bibliothèques externes nécessaires
│   └── <dependency>
│       ├── <groupId>junit</groupId>
│       ├── <artifactId>junit</artifactId>
│       ├── <version>4.13.2</version>
│       └── <scope>test</scope>
│
└── <build>                  → configuration des plugins (optionnel)
    └── <plugins>
        └── <plugin>        → plugin Maven utilisé pour compiler ou packager

```

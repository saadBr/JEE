
# Injection des Dépendances en Java
Ce projet illustre l'injection de dépendances en Java à travers trois approches :

- Injection statique
- Injection dynamique
- Injection via Spring (XML + Annotations)

## 📁 Structure du Projet
```
📂 src
├── 📂 main
│   ├── 📂 java
│   │   ├── 📂 net.elmabrouk
│   │   │   ├── 📂 dao
│   │   │   ├── 📂 ext
│   │   │   ├── 📂 metier
│   │   │   ├── 📂 pres
│   ├── 📂 resources
├── 📂 test
├── 📂 target
├── .gitignore
├── config.txt
├── pom.xml
```
## 🚀 Fonctionnalités Implémentées
✅ Interface ```IDao``` avec méthode ```getData()```
✅ Implémentation ```DaoImpl```
✅ Interface ```IMetier``` avec méthode ```calcul()```
✅ Implémentation ```MetierImpl``` (couplage faible)
✅ Injection par :

Instanciation statique → ```PresentationV1.java```
Instanciation dynamique → ```PresentationV2.java```
Spring (XML) → ```PresSpringXML.java``` + ```config.xml```
Spring (Annotations) → ```PresSpringAnnotation.java```
## 🛠️ Exécution
### Instanciation statique :

```net.elmabrouk.pres.PresentationV1```

Implementation DAO:


![staticBD](images/StaticBD.png)

Implementation EXT:

![staticWS](images/StaticWS.png)

### Instanciation dynamique :

```net.elmabrouk.pres.PresentationV2```

Implementation DAO:


![DynamicBD](images/DynamicBD.png)

Implementation EXT:

![DynamicWS](images/DynamicWS.png)

### Injection via Spring (XML) :

```net.elmabrouk.pres.PresSpringXML```

Implementation DAO:


![XMLBD](images/xmlBD.png)

Implementation EXT:

![XMLWS](images/xmlWS.png)

### Injection via Spring (Annotations) :

```net.elmabrouk.pres.PresSpringAnnotation```

Implementation DAO:


![AnnotationBD](images/AnnotationBD.png)

Implementation EXT:

![AnnotationWS](images/AnnotationWS.png)

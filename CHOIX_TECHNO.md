# Analyse des choix technologiques

## ADR - Framework Frontend JS

### Contexte
Le projet ECOM nous impose l'utilisation de JHipster, qui lui-même s'appuie sur des framework Javascript. Lequel choisir ?

### Options possibles
* [Angular](https://angular.io)
* [VueJS](https://vuejs.org)
* [React](https://reactjs.org)

### Décision

Nous avons choisi d'utiliser **React**, car une partie de l'équipe a déjà un peu d'expérience avec ce framework. Dans une optique d'efficacité, il est intéressant de se reposer sur les compétences déjà présentes. De plus, **React** repose sur la gestion de composants distincts, cela permet de développer plusieurs d'entre eux de manière indépendante et de paralléliser le développement.


## ADR - Builder

### Contexte
Le projet ECOM nous impose l'utilisation de JHipster, qui lui-même s'appuie sur des builders différents. Lequel choisir ?

### Options possibles
* [Maven](https://maven.apache.org/)
* [Gradle](https://gradle.org/)

### Décision

Nous avons choisi d'utiliser **Gradle**, c'est un builder plus récent et donc probablement plus durable à long terme.
Nous estimons que les conventions sont plus récentes et plus claires, le code sera plus susceptibles d'être maintenu dans le temps.
Ces deux raisons favorisent une potentielle reprise du projet.


## ADR - IDE

### Contexte
Le projet ECOM nécessite du développement, pour cela, il faut utiliser un IDE. Il en existe de nombreux, chacun possède ses spécificités. Lequel choisir ?

### Options possibles
* [Eclipse](https://www.eclipse.org/)
* [Visual Studio Code](https://code.visualstudio.com/)
* [Intellij](https://www.jetbrains.com/fr-fr/idea/)
* [Atom](https://github.com/atom)

### Décision

Nous avons choisi d'utiliser **Eclipse** pour développer en Java, car grâce à notre formation, nous sommes déjà familiarisés avec cet IDE.  
Cet IDE est complet, permet de débuguer facilement, et possède de nombreuses fonctionnalités qui favorisent l'efficacité et la simplicité du développement.  
Nous avons choisi d'utiliser **Visual Studio Code** pour développer dans les autres langages, car nous sommes déjà familiarisés avec cet IDE.
L'avantage majeur de cet IDE est le nombre d'extensions qui facilite et accélère le développement.


## ADR - BDD

### Contexte
Le projet ECOM nous impose l'utilisation de JHipster, qui lui-même s'appuie sur des types de base de données différents. Lequel choisir ?

### Options possibles
* [H2](https://www.h2database.com/html/main.html)
* [PostgreSQL](https://www.postgresql.org/)
* [MySQL](https://www.mysql.com/)
* [MariaDB](https://mariadb.org/)
* [Oracle](https://www.oracle.com/)
* [MSSQL](https://www.npmjs.com/package/mssql)

### Décision

Nous avons choisi d'utiliser **PostgreSQL**, car nous avons déjà de l'expérience avec cette technologie. PostgreSQL a une conformité plus stricte aux normes SQL.
De plus, c'est une technologie standard très répendue. Il sera donc facile de trouver quelqu'un ayant les compétences nécessaires en cas de reprise du projet.


## ADR - Outil d'organisation 

### Contexte
Le projet ECOM nécessite une organisation d'équipe structurée pour que l'avancée dans le projet soit efficace. Il existe de nombreux outils d'organisation. Lequel choisir ?

### Options possibles
* [Trello](https://trello.com/)
* [Gantt](https://www.gantt.com/)

### Décision

Nous avons choisi d'utiliser **Trello**, car nous avons déjà de l'expérience avec cet outil. **Trello** permet de planifier et d'acquitter les tâches ainsi que leur avancement.

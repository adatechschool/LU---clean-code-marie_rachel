# Comprendre

**Clean code, pourquoi ?** 

- Essentiel pour que le code reste simple, lisible, concis pour les autres développeurs et pour nous-même dans le futur. et nos équipes
- A noter : la notion de propreté étant subjective, le clean code d’une personne est rarement le clean code de l’autre !
- Refactorisation/refactoring : ensemble de méthodes permettant de transformer un code considéré comme difficile en code propre, sans changer son comportement.


Les grands principes du clean code : 

- il est expressif : on doit donner des noms clairs aux variables, aux classes etc. A la lecture, on doit pouvoir comprendre facilement ce que va faire le code. On doit également éviter de polluer avec trop de documentations/commentaires. La bonne lisibilité du code est plus importante que d'être concis.

Ex de deux bonnes pratiques : 

⇒ Mettre des nombres connus dans des constantes bien nommées (ex : `const CACHE_TIME = 200;`) 

⇒ Créer des noms plus longs au lieu de noms plus courts (ex : `userHasFormAccess` plutôt que `canAccess`, qui n'est pas aussi clair).

- il est simple : on évite de créer des fonctions et des classes dans tous les sens. On suit la méthode KISS (Keep it Simple Stupid).

⇒ chaque classe et fonction ne doit remplir qu'un rôle pour simplifier la compréhension 

⇒ on ne se répète pas, pas de copier-coller de code identique, on va plutôt créer une fonction qui pourra être appelée à plusieurs reprises.

- il est maintenable : le but est de pouvoir travailler durablement sur le code. Le clean code permet de pouvoir updater, tester, ajouter de nouvelles fonctionnalités facilement. Un code mal écrit va être au contraire difficile à modifier sans créer de bugs.

Comment pousser au clean code ? 

- Pull requests : les autres devs lisent et commentent notre code avant qu'il ne puisse être intégré. Cela permet de créer de la discussion dans l'équipe et partager les bonnes pratiques communes.
- TDD : écrire les tests avant le code nous aide à bien comprendre ce que doit faire notre code, et donc à écrire du code simple. Les TDD permettent également de retester facilement notre code si on le modifie, le refactorise.
- Faire régulièrement de la refacto

D'autres principes du clean code : 

- YAGNI : You aren't gonna need it

Ne pas ajouter de fonctionnalités inutiles. YAGNI fait partie de la méthodologie de l'extreme programming (XP), qui veut améliorer la qualité logicielle et se rapprocher toujours plus des demandes du client. 

- Être consistent : principe essentiel, si on décide de coder d'une certaine manière, il faut en faire ainsi tout du long. Si l'on se retrouve obligé de faire une exception, alors il faut clarifier le pourquoi en commentaire.

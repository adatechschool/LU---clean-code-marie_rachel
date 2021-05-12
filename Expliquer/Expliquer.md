# Expliquer


- **Factorisation** : ensemble de méthodes permettant de transformer un code considéré comme difficile en code propre, sans changer son comportement.

4 étapes : 

⇒ Elimination du code mort (ex : méthodes qui ne sont plus utilisées depuis longtemps, code en commentaire depuis toujours etc.)

⇒ Normalisation et documentation du code : vérifier que les normes de codage sont bien appliquées si on en a, penser à écrire la docu et des commentaires (pour les endroits complexes)

⇒ Renommage et harmonisation : les noms de méthodes doivent se comprendre idéalement d'elles mêmes, il faut harmoniser le code en déplaçant les fonctions à des emplacements qui font sens pour nous aider à les retrouver plus tard.

⇒ Optimisation (optionnel) : après toutes ces étapes,on peut améliorer le code pour des raisons de performance.

- **Dette technique** : concept du développement logiciel inventé par Ward Cunningham en 1992. Elle peut être intentionnelle (si la priorité est de livrer rapidement un logiciel ou une nouvelle fonctionnalité) ou non. Dans le deuxième cas, cela pose problème car cela vient d'un code qui n'est pas optimal.Une conception logicielle négligée induit des coûts futurs : les intérêts, à rembourser sous forme de temps de développement supplémentaire et de bugs de plus en plus fréquents. La dette technique doit être remboursée rapidement pour éviter l'accumulation de ces intérêts, d'où l'analogie avec le concept de dette financière.

- **Isofonctionnel** :réussir à garder les mêmes fonctionnalités d'un logiciel lors d'une migration (compliqué car il y en aura qui ne seront pas native au nouveau langage choisi par exemple)

- **Code smell** (mauvaises odeurs): mauvaises pratiques de conception logicielle qui conduisent à l’apparition de défauts. Ces défauts sont souvent issus de mauvais choix d’implantation ou de conception et conduisent à une complexification du code source et de la maintenance et évolutivité de celui‐ci. A la différence d'un AntiPattern, les code smells ne sont pas forcément des erreurs, c'est-à-dire qu'ils peuvent persister sans perspective d'évolution dans un logiciel. Afin de corriger un code smell, il est nécessaire de procéder à une refacto.

- **Design pattern** (patrons de conception) **:**

    Façon standard de résoudre un problème de conception logiciel récurrent. 

- **Anti-pattern :** les anti-patrons sont des erreurs courantes de conception des logiciels. Leur nom vient du fait que ces erreurs sont apparues dès les phases de conception du logiciel, notamment par l'absence ou la mauvaise utilisation de design patterns. Les anti-patrons se caractérisent souvent par une lenteur excessive du logiciel, des coûts de réalisation ou de maintenance élevés, des comportements anormaux et la présence de bugs.

- **Code legacy** : l’ensemble du code qui n’est pas testé unitairement. Ce code est difficilement réutilisable car non couvert par des tests automatisés.

- **DRY** : Don't Repeat Yourself. Proche du  kiss et de la philosophie de design minimaliste. Ce principe dit que chaque élément de savoir (ici, le code) doit avoir une représentation unique, autoritaire et sans ambiguïtés dans un système (codebase). Une violation du DRY s'appelle un WET : We Enjoy Typing, Write Everything Twice, Waste Everyone's Time.

- **KISS** : Keep It Simple Stupid

Une manière de concevoir l'écriture du code qui vient de l'US Navy dans les années 60.L'idée est de penser les systèmes de la manière la plus simple possible (sans pour autant les simplifier comme aurait dit Einstein). Il faut éviter les complexités inutiles. 

⇒ Toujours se poser la question : est-ce que ce code peut être écrit de manière plus simple ?  

**SOLID** : acronyme pour les 5 premiers designs orientés objet développé par Robert C. Martin

- **[S** - Single-responsiblity Principle]

⇒ une fonction, une classe ne doit remplir qu'un seul rôle

- **[O** - Open-closed Principle]

⇒ un objet ou une entité doit être ouverte à l'extension mais fermée à la modification

- **[L** - Liskov Substitution Principle]

⇒ chaque sous-classe ou classe dérivée doit être substituable par sa base ou sa classe parent

> Let q(x) be a property provable about objects of x of type T. Then q(y) should be provable for objects y of type S where S is a 
subtype of T.

- **[I** - Interface Segregation Principle]

Un client ne doit jamais être forcé à implémenter une interface qu'il n'utilise pas, ou ne doivent pas être forcés à dépendre de méthodes qu'il n'utilise pas

- **[D** - Dependency Inversion Principle]

Les entités doivent dépendre d'abstractions et non du concret. Les modules haut-niveau ne doivent pas dépendre des modules bas niveau. Ils doivent dépendre d'asbtractions. 

- **Linter** (aussi appelé lint) ****: outil d'analyse de code qui détecte les erreurs de programmation, les erreurs stylistiques et les constructions suspicieuses. Le terme vient d'une commande Unix qui examine le code source du langage C.

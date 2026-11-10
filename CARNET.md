# 📒 Mon carnet de bord

**Nom :** guenard

**Prénom :** Manon

**Adresse de mon site :** https://manon2031.pythonanywhere.com

> Modifiez ce fichier directement sur GitHub (icône crayon ✏️) pour répondre aux questions de chaque exercice.
> Écrivez avec vos propres mots : une réponse courte et juste vaut mieux qu'un long copier-coller ! 🙂

---

## 🟢 Exercice 1 — Mon premier déploiement

1. Où se trouve physiquement le code qui fabrique votre page : sur votre ordinateur, sur GitHub ou sur PythonAnywhere ?

   > _Ma réponse :_ sur GitHub

2. Pourquoi votre voisin(e) peut-il voir votre site, alors que vous n'avez rien installé sur son ordinateur ?

   > _Ma réponse :_ car le site est en public et peut etre vu par tous

---

## 🟢 Exercice 2 — Les URL et les routes

1. Dans l'URL `https://www.google.com/maps`, quel est le nom de domaine ? Quel est le chemin ?

   > google.com

2. Que veut dire le message *Not Found* ? Qui l'a envoyé : votre navigateur ou le serveur ?

   >l'objet informatique n'a pas pu etre trouvé ou utilisé

3. Que se passe-t-il si deux fonctions portent le même nom dans `flask_app.py` ? (Indice : essayez, puis lisez l'Error log.)

   > la commande error log se met en route

---

## 🔵 Exercice 3 — Le langage HTML

1. Quelle est la différence entre ce que le serveur **envoie** et ce que le navigateur **affiche** ?

   > il envoie des phrases entre des balises et il affiche des paragraphes avec des points de presentations des titres etct.

2. À quoi servent les balises `<h1>`, `<p>`, `<ul>` et `<li>` ?

   > pour le titre principal , paragraphe du texte, liste, un élément 

3. Pourquoi l'image s'affiche-t-elle alors qu'elle n'est pas sur votre serveur ?

   > car il y a la balise pour inserer l'iamge.

---

## 🔵 Exercice 4 — Les templates

1. Pourquoi est-ce une bonne idée de séparer le code Python et le HTML ? (Pensez à une équipe avec un développeur et un graphiste.)

   >car chacun a un rôle différent, l'un travail sur le programme en lui même tandis que lautre travaille sur la mise en forme de celui ci

2. Les `{{ prenom }}` sont-ils remplacés par le serveur ou par le navigateur ? Comment l'avez-vous vérifié ?

   >  grâce au moteur de templates utilisé par Flask. On peut le vérifier en affichant le code source de la page dans le navigateur  (mon code ne marche pas )

---

## 🔵 Exercice 5 — Le CSS et les liens

1. Quelle est la différence de rôle entre le HTML et le CSS ?

   > Le HTML sert à structurer le contenu d'une page web, comme les titres, les paragraphes et les images, tandis que le CSS sert à définir son apparence, comme les couleurs, les tailles, les polices et la mise en page. Le HTML donne donc la structure de la page et le CSS permet de la rendre plus esthétique.

2. Pour afficher votre page `/presentation`, combien de fichiers le navigateur doit-il télécharger ? (Vous pourrez le vérifier à l'exercice suivant !)

   >Le navigateur doit télécharger un seul fichier, le fichier HTML presentation.html, car il ne contient pas encore de fichier CSS ou d'autres ressources externes.




3. Pourquoi faut-il parfois faire **Ctrl + F5** pour voir les changements de CSS ?

   > Il faut parfois faire Ctrl + F5 pour voir les changements de CSS car le navigateur garde parfois une ancienne version du fichier en mémoire cache et cette manipulation force le navigateur à recharger la page et à récupérer les dernières modifications du CSS

---

## 🟣 Exercice 6 — Espionner le navigateur

1. Que signifie HTTP ? Qui envoie la **requête** et qui envoie la **réponse** ?

   >HTTP signifie HyperText Transfer Protocol, c'est le protocole qui permet la communication entre le navigateur et le serveur, le navigateur envoie une requête au serveur et le serveur lui renvoie une réponse
   
2. Combien de requêtes votre page `/presentation` a-t-elle déclenchées ? Lesquelles ?

   >La page /presentation a déclenché deux requêtes, une pour récupérer la page HTML et une autre pour récupérer la favicon, qui est la petite icône affichée dans l'onglet du navigateur

3. Que signifie le code `200` ? Et le code `404` de la favicon ?

   > Le code 200 signifie que la requête a réussi et que le serveur a correctement envoyé la page, tandis que le code 404 signifie que la ressource demandée n'a pas été trouvée, dans ce cas la favicon

4. Pourquoi les modifications faites dans l'onglet Éléments ne sont-elles pas visibles par les autres visiteurs ?

   > Les modifications faites dans l'onglet Éléments ne sont pas visibles par les autres visiteurs car elles sont réalisées directement dans le navigateur et ne modifient pas les fichiers du serveur, elles sont donc temporaires et disparaissent lorsqu'on recharge la page

---

## 🟣 Exercice 7 — Envoyer des informations dans l'URL

1. Dans l'URL `https://www.youtube.com/results?search_query=chat`, quel est le nom du paramètre ? Quelle est sa valeur ?

   > Dans l'URL https://www.youtube.com/results?search_query=chat, le nom du paramètre est search_query et sa valeur est chat 

2. Pourquoi le serveur plante-t-il avec `a=bonjour` ? Que faudrait-il faire pour l'éviter ?

   > Le serveur plante avec a=bonjour car il reçoit une valeur qui n'est pas du type attendu par le programme, par exemple un nombre, et provoque une erreur lors du traitement. Pour éviter cela, il faut vérifier les données reçues et contrôler leur type avant de les utiliser

3. Pourquoi est-il dangereux d'afficher **tel quel** ce que l'utilisateur envoie ?

   >Il est dangereux d'afficher directement ce que l'utilisateur envoie car il pourrait insérer du code HTML ou JavaScript malveillant qui pourrait être exécuté dans le navigateur des visiteurs. Il faut donc toujours sécuriser et échapper les données avant de les afficher

---

## 🟣 Exercice 8 — Les formulaires

1. Quelle est la différence visible entre GET et POST ?

   > La différence visible entre GET et POST est que la méthode GET affiche les données envoyées dans l'URL sous forme de paramètres, tandis que la méthode POST envoie les données dans le corps de la requête sans les afficher dans l'adresse du navigateur

2. Pour un formulaire de **recherche**, quelle méthode choisiriez-vous ? Et pour un formulaire de **connexion avec mot de passe** ? Pourquoi ?

   >Pour un formulaire de recherche, je choisirais la méthode GET car elle permet de retrouver facilement une recherche grâce à son URL et de la partager avec d'autres personnes

3. Les données envoyées en POST sont-elles vraiment « secrètes » ? (Pensez à ce que vous avez vu dans l'onglet Réseau.)

   > Pour un formulaire de connexion avec un mot de passe, je choisirais la méthode POST car le mot de passe n'apparaît pas directement dans l'URL 

---

## 🔴 Exercice 9 — Les codes de statut

1. Quelle est la différence entre une erreur `4xx` et une erreur `5xx` ? Qui est « fautif » dans chaque cas ?

   > Une erreur 4xx signifie qu'il y a un problème dans la requête envoyée par le navigateur, par exemple une page qui n'existe pas avec une erreur 404. C'est généralement le client qui est responsable, tandis qu'une erreur 5xx signifie qu'il y a un problème du côté du serveur qui n'arrive pas à traiter correctement la requête

2. Comment fonctionne une redirection ? Qui fait la deuxième requête : le serveur ou le navigateur ?

   >Une redirection fonctionne lorsque le serveur indique au navigateur qu'il doit se rendre vers une autre adresse. C'est le navigateur qui effectue alors une deuxième requête vers la nouvelle adresse 

3. Donnez un exemple de situation où un vrai site utilise une redirection.

   >Un exemple de redirection est lorsqu'on se connecte à un site et qu'on est automatiquement redirigé vers la page d'accueil ou vers son espace personnel après avoir réussi la connexion

---

## 🔴 Exercice 10 — Ce que le serveur sait de vous

1. Citez trois informations que le serveur connaît sur vous, sans que vous ayez rien rempli.

   >Le serveur connaît plusieurs informations sur moi sans que j'aie besoin de les remplir, comme mon adresse IP, le type de navigateur que j'utilise et la langue de mon navigateur

2. À quoi peut servir l'en-tête `Accept-Language` pour un site comme Wikipédia ?

   > L'en-tête Accept-Language permet à un site comme Wikipédia de détecter la langue préférée du visiteur et de lui proposer automatiquement les pages dans cette langue

3. Dans l'Access log, retrouvez une requête qui a reçu un code `404`. Quelle page était demandée ?

   >Dans l'Access log, la requête qui a reçu un code 404 correspond à une page qui n'a pas été trouvée, par exemple la favicon si c'est celle qui apparaît dans mon journal

4. Après cet exercice, que pensez-vous de la notion de « navigation anonyme » ?

   > Après cet exercice, je pense que la navigation anonyme est difficile à garantir car les sites peuvent récupérer plusieurs informations sur les visiteurs, même sans qu'ils remplissent de formulaire.

---

## 🔴 Exercice 11 — Le Web des machines : API et JSON

1. Quelle est la différence entre une page HTML et une réponse JSON ? À qui chacune est-elle destinée ?

   > _Ma réponse :_ 

2. Dans la page `/horloge`, quel code s'exécute sur le **serveur** et quel code s'exécute dans le **navigateur** ?

   > _Ma réponse :_ 

3. Citez une application de votre téléphone qui, selon vous, utilise une API. Quelles données échange-t-elle ?

   > _Ma réponse :_ 

---

## 🏁 Pour conclure

En quelques phrases, expliquez à un ami ce qui se passe entre le moment où il tape une adresse dans son navigateur et celui où la page s'affiche :

> _Ma réponse :_ 

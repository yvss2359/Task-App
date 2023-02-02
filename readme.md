# Projet React Groupe A: Saadi Nadine - Rachedi Ilyas - Hubert Anaïs - Vanègue Adrien

Ce dépôt contient le code du projet React du Groupe A de JS.

## Comment ouvrir le projet?
Toutes les commandes sont à exécuter à partir de ce dossier `projet-react/`
 * récupérer le dépôt
 * installer les paquets *Node.js* :
  ```bash
  $  npm install
  ```
  * créer le dossier `dist/`
  ```bash
  $  npm run build
  ```

  * Ouvrez l'application en ouvrant le fichier `dist/index.html`

## Liste des composants et leur role:

La structure et le rôle de nos composants suivent la même hiérarchie et rôle montrés dans la vidéo de démonstration de Mr Routier. Tous les composants se trouvent dans le dossier `components/`

* `taskApp.jsx`: c'est la racine de l'application qui est un gestionnaire de tâches auquel on peut ajouter, terminer des tâches, tout en les classant par priorité décroissante.
* `toDo.jsx`: c'est un composant servant à lister les tâches (Task) à faire. Il permet aussi de filtrer les tâches à faire à afficher à l'aide d'un champ de saisie dans lequel on peut entrer la description des tâches que l'on veut afficher. Ce filtre est non sensible à la casse.
* `task.jsx`: c'est un composant représentant une tâche à faire. Une tâche a un id, une description, une durée, une priorité et contient une échelle de priorité afin de changer sa priorité et un bouton pour terminer la tâche.
* `doneButton.jsx` : composant représentant un bouton permettant de terminer la tâche qui lui est associée.
* `priorityScale.jsx`: c'est un composant représentant une échelle de priorité (de 1 à 6 par défaut) qui contient des niveaux de priorités pour changer la priorité d'une tâche.
* `priorityLevel.jsx` : c'est un composant représentant un niveau d'une échelle de priorité. Cliquer dessus modifie la priorité de la tâche qui lui est associée.
* `addTask.jsx`: composant servant à ajouter une tâche dans le composant ToDo.
* `done.jsx` : composant servant à lister les tâches déjà faites (DoneTask).
* `doneTask.jsx` : composant représentant une tâche déjà faite, affichant ainsi sa description, sa durée et sa priorité.

## Fonctionnalités supplémentaires.

* On a mis en place la sauvegarde de l'état de l'application dans le stockage local de l'utilisateur. Ainsi, entre chaque fermeture/ouverture de l'application, toutes les tâches ajoutées, à faire et faites sont conservées.

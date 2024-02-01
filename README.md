# TaeKwonDo API

Voici l'API française la plus complète sur le TaeKwonDo.
Simple d'utilisation et facile à intégrer dans vos projets, cette API vous servira à récupérer toutes les informations sur le TaeKwonDo dont vous avez besoin.

## Installation

Ouvrez un terminal et exécutez la commande suivante dans le dossier de votre projet :

```bash
git clone https://github.com/AlexShadow3/TaeKwonDo_API.git
```

## Usage

```js
async function fetchData() {
    try {
        const response = await fetch('taekwondo.json');
        if (!response.ok) {
            throw new Error('Failed to fetch data');
        }

        const taekwondo = await response.json();
        // Utilisez l'objet 'taekwondo' ici
        console.log(taekwondo); // { grades: [...], poomsae: [...] }
        console.log(taekwondo.grades); // [ { name: '10ème Kup', ... }, ... ]
    } catch (error) {
        console.error('Error loading JSON file:', error);
    }
}

// Appelez la fonction asynchrone
fetchData();
```

## Liste des fonctionnalités

Liste des fonctionnalités disponibles (ou à venir) :

- [x] Les grades
  - [x] Grades enfant
  - [x] Grades adulte
  - [x] Grades master (à partir de la ceinture noire)
- [x] Les positions
- [x] Les techniques
  - [x] Les techniques de blocage à mains ouvertes
  - [x] Les techniques de blocage à mains fermées
  - [x] Les techniques de coup de poing
  - [x] Autres techniques de blocage à la main
  - [x] Les techniques de coup de pied
- [x] Les poomsae
  - [x] 1er poomsae
  - [x] 2ème poomsae
  - [x] 3ème poomsae
  - [x] 4ème poomsae
  - [x] 5ème poomsae
  - [x] 6ème poomsae
  - [x] 7ème poomsae
  - [x] 8ème poomsae
- [x] Les mots à connaître et leur traduction

**Il existe tellement de mots qu'il m'est impossible de compléter entièrement la dernière partie !!**

## Contribuer

Envie de contribuer ? Hésite pas à faire un pull request !

N'oubliez pas de laisser un ⭐ ça me ferait plaisir !

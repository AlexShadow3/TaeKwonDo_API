# TaeKwonDo API

Voici l'API française la plus complète sur le TaeKwonDo.
Simple d'utilisation et facile à intégrer dans vos projets, cette API vous servira à récupérer toutes les informations sur le TaeKwonDo dont vous avez besoin.

## Installation

```bash

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
        // Use the 'taekwondo' object here
        console.log(taekwondo); // { grades: [...], poomsae: [...] }
        console.log(taekwondo.grades); // [ { name: '10ème Kup', ... }, ... ]
    } catch (error) {
        console.error('Error loading JSON file:', error);
    }
}

// Call the async function
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
- [ ] Les mots à connaître et leur traduction

## Contribuer

Envie de contribuer ? Hésite pas à faire un pull request !

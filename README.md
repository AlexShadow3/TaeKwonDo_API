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
- [] Les positions
- [] Les techniques de défense
- [] Les techniques de coup de pied
- [] Les techniques de coup de poing
- [] Autres techniques
- [x] Les poomsae

## Contribuer

Envie de contribuer ? Hésite pas à faire un pull request !

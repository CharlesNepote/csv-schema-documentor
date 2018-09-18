# csv-schema-documentor

[english/français]

(fr) Crée une documentation HTML à partir d'un schéma de données au format [Table Schema](https://frictionlessdata.io/specs/table-schema/). csv-schema-documentor est un outil en ligne de commande fonctionnant sous Linux et probablement sous Mac OS X. Voici [un exemple de documentation générée](http://rn7.net/csv-schema-documentor/doc.html), à partir de la [spécification](https://github.com/CharlesNepote/liste-prenoms-nouveaux-nes/blob/v1.1.1/prenom-schema.json) de la liste des prénoms des nouveaux nés.

(en) Create HTML documentation from a CSV Schema ([Table Schema](https://frictionlessdata.io/specs/table-schema/)). csv-schema-documentor is command line tool working under Linux and probably Mac OS X.  Check [this example of generated doc](http://rn7.net/csv-schema-documentor/doc.html), from this [specification](https://github.com/CharlesNepote/liste-prenoms-nouveaux-nes/blob/v1.1.1/prenom-schema.json) (in french).

## Installation

(fr)
- Installer [handlebars-cmd](https://www.npmjs.com/package/handlebars-cmd) ou bien [render-cli](https://www.npmjs.com/package/render-cli).

- Télécharger le repos ou bien seulement le fichier `template.hbs`.

## Usage

(fr)

Crée une documentation doc.html à partir de votre fichier schema.json.

`handlebars schema.json < template.hbs > doc.html`

Example à partir d'un fichier en ligne :

`curl -O https://raw.githubusercontent.com/CharlesNepote/liste-prenoms-nouveaux-nes/v1.1.1/prenom-schema.json && handlebars prenom-schema.json < template.hbs > doc.html`


(en)

Create a doc.html documentation from your schema.json.

`handlebars schema.json < template.hbs > doc.html`

## TODO

- Explain properties outside of strict Table Schema spec.

- French/english doc based on browser config.

- Provide an example for multiple files.

- Generation form.

# Gestion des Données Passagers pour un Aéroport

## Introduction
Ce projet vise à vous familiariser avec le format YAML en transformant des données tabulaires représentant les informations des passagers d'un aéroport en un format exploitable pour des applications web ou mobiles.

## Exercices

### Exercice 1 : Conversion de Données Tabulaires en YAML
Objectif: Convertir une table de données passagers en format YAML.
Données initiales:
  | nom       | prénom    | n° vol | Nbr bagages | N° client |
  |-----------|-----------|--------|-------------|-----------|
  | Einstein  | Albert    | 45622  | 2           | 154565    |
  | Lavoisier | Antoine   | 45644  | 4           | 235002    |
  | Raimbault | Arthur    | 12896  | 2           | 544552    |
  | Poincaré  | Henri     | 45644  | 3           | 781201    |
  | Lavoisier | Antoine   | 45644  | 1           | 785154    |
  | Einstein  | Albert    | 75906  | 0           | 858547    |

### Instructions:
  - Utilisez les données fournies pour créer une représentation YAML.

### Exercice 2 : Ajout d'Informations d'Adresse
Objectif: Enrichir chaque enregistrement passager avec des informations d'adresse en YAML.
Nouvelles données à inclure:
  - Num_CIV: Numéro civique
  - Rue: Nom de la rue
  - CP: Code postal
Instructions:
  - Ajoutez une nouvelle section dans chaque enregistrement passager pour inclure l'adresse complète en format YAML.


**Exemple pour un passager :**
```yaml
- nom: Einstein
  prénom: Albert
  n° vol: 45622
  Nbr bagages: 2
  N° client: 154565
  adresse:
    Num_CIV: "10"
    Rue: "Rue de l'Univers"
    CP: "75005"
```


### Exercice 3 : Gestion des Adresses Multiples
Objectif: Modifier la structure YAML pour permettre plusieurs adresses pour un passager donné.

**Instructions :**
- Étendez la structure YAML de l'exercice précédent pour prendre en charge plusieurs adresses pour au moins un passager.
- Pour le passager 'Einstein Albert', ajoutez une seconde adresse dans le fichier YAML.
- La section 'adresse' doit être modifiée pour devenir une liste d'adresses.

**Exemple avec plusieurs adresses pour un passager :**
```yaml
- nom: Einstein
  prénom: Albert
  n° vol: 45622
  Nbr bagages: 2
  N° client: 154565
  adresses:
    - Num_CIV: "10"
      Rue: "Rue de l'Univers"
      CP: "75005"
    - Num_CIV: "21"
      Rue: "Rue de la Paix"
      CP: "75002"
```

### Résultat attendu:
  - Pour l'exercice 1: Un document YAML représentant la table initiale.
  - Pour l'exercice 2: Le même document YAML avec des adresses ajoutées pour chaque passager.
  - Pour l'exercice 3: Le document YAML modifié pour montrer plusieurs adresses pour certains passagers.

### Visualisation:
  - Utilisez un éditeur YAML en ligne ou un outil de validation pour vérifier la structure de votre document YAML après chaque exercice.














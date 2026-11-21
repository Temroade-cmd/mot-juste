# mot-juste

Un skill pour écrire en français sans sonner comme une IA.

Un texte écrit par une IA ne se repère pas à une faute. Il se repère à ce qu'il est trop lisse. Les mêmes mots reviennent (crucial, véritable, essentiel), les phrases font toutes la même longueur, la typographie est anglaise, et on pourrait changer le nom du destinataire sans rien changer au reste. mot-juste donne à un assistant IA une méthode pour écrire l'inverse, un texte précis qui n'appartient qu'à son auteur.

Le but n'est pas de tromper un détecteur. Le but est d'écrire mieux.

## Ce qu'il contient

| Fichier | Rôle |
|---|---|
| [`skills/mot-juste/SKILL.md`](skills/mot-juste/SKILL.md) | La méthode en sept passes (le fond, le lexique, les tournures, le rythme, la typographie française, la structure, la voix) et une liste de contrôle |
| [`references/tics.md`](skills/mot-juste/references/tics.md) | Le catalogue des tics, avec pour chacun un exemple et une meilleure version |
| [`references/candidatures.md`](skills/mot-juste/references/candidatures.md) | Le bonus candidatures, pour les lettres de motivation, le projet d'études Campus France, les mails à un directeur de thèse et les relances |

## Exemple

Avant

> Passionné par l'intelligence artificielle depuis mon plus jeune âge, c'est avec un grand intérêt que j'ai découvert votre offre, qui s'inscrit pleinement dans mon projet professionnel.

Après

> J'ai lu votre offre de thèse sur la segmentation d'IRM cardiaques. Mon mémoire de master portait sur la prédiction du risque cardiovasculaire, avec un modèle XGBoost entraîné sur 1190 patients.

## Installation

Avec Claude Code, copier le dossier dans les skills de l'utilisateur.

```bash
git clone https://github.com/Temroade-cmd/mot-juste.git
cp -r mot-juste/skills/mot-juste ~/.claude/skills/
```

Sur claude.ai, compresser le dossier `skills/mot-juste` en `.zip` puis l'ajouter dans les réglages, rubrique Skills.

Avec un autre assistant, coller le contenu de `SKILL.md` au début de la conversation suffit.

Ensuite il suffit de demander, par exemple « relis ma lettre de motivation avec mot-juste ».

## Feuille de route

- [x] v0.1, la méthode et une liste de tics tirée de l'observation
- [x] Le bonus candidatures
- [ ] Une étude mesurée, qui compare des textes écrits par des modèles de langue à des textes humains en français, pour savoir quels mots et quelles tournures sont vraiment surutilisés
- [ ] v0.2, le catalogue remplacé par la liste mesurée

## Licence

MIT, voir [LICENSE](LICENSE). Créé par Tamer Benturquia.

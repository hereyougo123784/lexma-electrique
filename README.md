# Lexma Électrique

Site vitrine pour **Lexma Électrique**, électricien résidentiel et commercial à
Saint-Ambroise, membre de la CMEQ. Page unique en défilement, construite avec
le skill [scroll-craft](../../../.agents/skills/scroll-craft/SKILL.md) :
HTML, CSS et JavaScript purs, sans framework ni étape de build.

## Mise en ligne

Le site vit dans le dépôt `claude-webb`, sous
`scrollcraft/builds/lexma-electrique/`, et il est publié dans son **propre
dépôt** où il occupe la racine, ce dont GitHub Pages a besoin. Il n'y a pas
de copie : le dossier de travail reste la seule source, et `git subtree`
republie ce qu'il contient.

**La première fois**, créer un dépôt GitHub vide nommé `lexma-electrique`,
sans README, sans .gitignore, sans licence. Puis :

```bash
git -C /Users/jg/claude subtree push --prefix=scrollcraft/builds/lexma-electrique lexma main
```

Ensuite, dans le dépôt sur GitHub : Settings → Pages → Source « Deploy from a
branch » → Branch `main`, dossier `/ (root)` → Save. Le site paraît à
`https://hereyougo123784.github.io/lexma-electrique/` en une minute ou deux.

**Ensuite**, à chaque modification, c'est la même commande. Le dépôt distant
`lexma` est déjà configuré.

## Lancer en local

Aucune dépendance à installer. Servez le dossier :

```bash
npx serve scrollcraft/builds/lexma-electrique
```

Puis ouvrez l'adresse affichée. La section contact est à `#contact`.

## À faire avant la mise en ligne

1. **Vérifier ce que la page ne dit pas.** Aucune heure d'ouverture, aucun
   prix, aucune statistique : rien de tout cela n'a été fourni et rien n'a été
   inventé. Si vous voulez les afficher, donnez-les et ils seront ajoutés.

2. **Choisir un hébergement et un nom de domaine.** Le site est un dossier de
   fichiers statiques : n'importe quel hébergeur le sert tel quel, sans base
   de données ni serveur d'application.

## Les visuels

Les quatre fichiers fournis sont en place, redimensionnés et compressés :
21 Mo au départ, 1,2 Mo au total. Deux largeurs par photo, servies par
`srcset`, donc un téléphone télécharge 80 Ko au lieu de 460 Ko pour la photo
d'ouverture.

**Les logos d'autres entreprises ont été retirés des trois photos.** Celle de
la prise a été recadrée sur les mains gantées, ce qui sort de l'image le logo
« APEX Electrical Services » qui était parfaitement lisible. Celle du panneau a
été retouchée : l'écusson brodé a été effacé pixel par pixel et le tissu
reconstruit à partir de celui qui l'entourait, en gardant les plis et la
lumière. L'électricien du camion ne porte aucun logo. Détail dans
`assets/A-LIRE.md`.

## La demande de soumission

La section « Envoyez-nous votre projet » recueille nom, téléphone, courriel,
adresse des travaux, type de travaux et description, et l'envoie à
`gestion@lexma-electrique.com` **par FormSubmit** — le même service que le
site JG AGENCY.

### Un seul geste, et il est à faire une fois

FormSubmit n'a ni compte ni clé. En revanche, **la première demande envoyée
déclenche un courriel de confirmation** à `gestion@lexma-electrique.com`, avec
un lien à cliquer. Tant que ce lien n'est pas cliqué, les demandes suivantes
n'arrivent pas.

Une fois le site en ligne : remplissez le formulaire une fois vous-même,
ouvrez la boîte, cliquez le lien. C'est fini pour toujours.

### Changer le destinataire

Un seul endroit, l'attribut `action` de la balise `<form>` dans `index.html` :

```html
<form class="lx-form" method="POST"
      action="https://formsubmit.co/gestion@lexma-electrique.com">
```

Le script relit cette adresse ; il n'y a pas de deuxième copie à synchroniser.
Pour envoyer à plusieurs personnes, ne touchez pas au formulaire : gardez une
seule adresse et faites une redirection ou un alias chez le fournisseur de
courriel. Le jour où quelqu'un s'ajoute ou s'en va, ça se règle dans la boîte
courriel et pas dans le code du site.

### Deux chemins, et le second est un vrai filet

Le formulaire a une `action` et une `method` : **c'est un vrai formulaire**, il
part tout seul si le JavaScript ne charge pas. Le script ne fait qu'améliorer.

- **Avec JavaScript** : envoi en arrière-plan, la confirmation s'affiche sans
  quitter la page.
- **Sans JavaScript, ou si l'envoi en arrière-plan échoue** : le navigateur
  poste le formulaire comme il l'a toujours fait, FormSubmit renvoie le
  visiteur sur la page avec `?envoye=1`, et la confirmation s'affiche pareil.

### Contre les robots

Le champ piège `_honey`, hors de l'écran et retiré du parcours au clavier, est
celui que FormSubmit attend. Un programme qui remplit tout se dénonce en le
remplissant.

### Ce que la politique de confidentialité en dit

Elle nomme FormSubmit et décrit ce que sa politique dit — et ce qu'elle ne dit
pas. **Elle ne fixe aucune durée de conservation** et le service n'offre aucun
réglage pour en imposer une. La politique l'écrit franchement plutôt que de
promettre ce qu'on ne contrôle pas, et propose au visiteur d'écrire ou
d'appeler directement s'il préfère rester hors de ce circuit.

Si cette absence de durée vous dérange, Web3Forms annonce une conservation
réglable (jusqu'à trois ans par défaut) en échange d'une clé à demander. Dites-
le-moi et je rebranche.

## La barre d'appel sur téléphone

En portrait seulement, une barre fixe en bas de l'écran avec deux boutons :
**Appeler** et **Courriel**. Elle n'apparaît qu'après le premier écran, qui
porte déjà son propre bouton d'appel. En paysage, la page n'a aucune barre.

## Coordonnées publiées

| | |
|---|---|
| Téléphone | 450 756-7111 |
| Courriel | gestion@lexma-electrique.com |
| Adresse | 128, rue des Œillets, Saint-Ambroise-de-Kildare (Québec) J0K 1C0 |
| Licence RBQ | 5767-5993-01 |
| | Membre de la CMEQ |

Un seul numéro de téléphone. La suite `5767599301` transmise au départ était
la licence RBQ sans ses traits d'union, pas un second numéro : elle a été
publiée un temps comme un lien d'appel, puis remise à sa place.

## La politique de confidentialité

`confidentialite.html` est une page autonome, liée depuis le pied de page et
sous le formulaire. Elle décrit exactement ce que le site fait, et ce qu'il
fait est peu de chose : **aucun témoin, aucun outil de suivi, aucun stockage
sur l'appareil du visiteur, aucune ressource chargée ailleurs**. C'est pour ça
qu'il n'y a pas de bandeau de consentement : il n'y a rien à consentir.

Pour que ce soit vrai, **les polices de caractères ont été rapatriées sur le
serveur**. Elles venaient du CDN de Google, qui recevait l'adresse IP et le
navigateur de chaque visiteur : c'était le seul transfert de données vers un
tiers de tout le site. Archivo et Geist sont sous licence libre, donc les
héberger soi-même est permis. Elles sont dans `assets/fonts/`, en latin
seulement, 228 Ko.

### Trois blancs à remplir avant la mise en ligne

1. **Le délai de conservation.** La politique dit qu'une demande sans suite est
   supprimée « au plus tard douze mois après le dernier échange ». Ce chiffre
   est un choix raisonnable, pas une obligation légale. Mettez le vôtre, et
   tenez-le.
2. **Le responsable de la protection des renseignements personnels.** La loi
   québécoise en exige un ; à défaut de désignation, c'est la personne qui a la
   plus haute autorité dans l'entreprise. La page renvoie à l'adresse courriel
   générale. Nommer la personne serait mieux.
3. **L'hébergeur.** La section sur les journaux de connexion est écrite de
   façon générale parce que l'hébergeur n'est pas encore choisi. Une fois qu'il
   l'est, on peut le nommer.

**Cette politique n'est pas un avis juridique.** Elle décrit fidèlement le
fonctionnement du site et reprend les droits prévus par la loi québécoise sur
la protection des renseignements personnels dans le secteur privé. Faites-la
relire si vous voulez une garantie sur la conformité de l'entreprise dans son
ensemble, qui déborde largement du site web.

## Structure

```
index.html            la page
confidentialite.html  la politique de confidentialité et de témoins
scrollcraft.css       le moteur : jetons et styles. Ne pas modifier
scrollcraft.js        le moteur : mécanique de scroll. Ne pas modifier
assets/               le logo et les photographies
assets/fonts/         Archivo et Geist, hébergées localement
BRIEF.md          le brief créatif : grammaire, courbe, sommet, partition
```

Le thème complet de la page tient dans six couleurs et deux familles
typographiques, en haut de `index.html`. L'encre bleu nuit et l'or viennent du
logo fourni.

## Ce que la page fait

- **Sept sections**, en alternance : une photographie plein cadre épinglée
  (« plan »), puis du texte seul sur un fond plat (« plaque »), à coupe
  franche, jamais en fondu.
- **Le mur qui se retourne**, au sommet : six lignes de très gros texte où ce
  que le propriétaire voit bascule, ligne par ligne et à des seuils
  dispersés, vers ce que l'électricien trouve derrière. Entraîné par le
  scroll, en CSS pur, donc identique au doigt sur un téléphone et identique
  pour un visiteur en mouvement réduit.
- **Aucune barre de navigation.** Le numéro est un lien d'appel réel dans le
  premier écran et dans le dernier.
- **Des données structurées** (`schema.org/Electrician`) pour la fiche locale
  dans les moteurs de recherche.

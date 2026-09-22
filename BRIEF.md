# BRIEF — Lexma Électrique

**Partiellement interviewé, le reste auto-rédigé sous délégation créative.**
Le client a fourni le nom, la clientèle (résidentiel et commercial), la
direction visuelle
(« électrique et audacieux »), l'emplacement de la construction, l'adresse,
deux numéros, le courriel, l'appartenance à la CMEQ, puis **quatre visuels**
(un logo et trois photographies) avec la consigne « créer des animations
incroyables et propres pour un site web professionnel et vendeur ». Tout ce
que ces faits ne décident pas est une décision d'auteur, étiquetée comme
telle. Aucune citation du client n'est inventée : ses réponses réelles sont
marquées **(client)**.

Cible d'implémentation : build statique autonome, moteur scroll-craft,
HTML/CSS/JS pur, aucun framework, aucune étape de build. Choix du client.

---

## Changement de prémisse en cours de build

La première version de cette page était en **affiche typographique**, et elle
l'était pour une seule raison : il n'y avait aucun visuel. Pas de photo
client, pas de `ffmpeg`, pas de clé kie.ai. `uniqueness.md` §2.5 nomme
exactement ce cas.

Le client a ensuite fourni un logo et trois photographies. La raison d'être de
cette grammaire a disparu avec l'arrivée des actifs, donc la grammaire a
changé plutôt que d'ajouter des photos à une grammaire qui les interdit
explicitement (« sol photographique » est dans sa liste d'interdits). Ce
paragraphe existe pour que la décision reste lisible : ce n'est pas une
hésitation, c'est un fait nouveau.

Ce qui a survécu de la première version, parce que ça ne dépendait pas de
l'absence de photos : l'écart d'échelle typographique, la courbe de ressenti,
le silence d'auteur, et le signature move.

---

## Les huit sujets

1. **Le vibe.** **(client)** « Électrique et audacieux ». Références
   d'auteur, hors du web : une plaque signalétique de panneau, un ruban de
   chantier, la sérigraphie d'un boîtier de disjoncteurs.
2. **Le parcours de scroll.** Auteur : le camion qui arrive chez vous, puis
   les quatre phrases que les clients disent vraiment au téléphone, puis un
   silence, puis le mur qui se retourne, puis ce qu'on fait, puis pourquoi
   c'est encadré par la loi, puis les coordonnées au calme.
3. **La courbe d'énergie.** Auteur : fort à l'ouverture, moyen sur les
   phrases, presque muet juste avant le sommet, le plus fort au sommet, puis
   descente continue jusqu'à une fermeture silencieuse.
4. **Le ressenti, étape par étape, et LE moment.** Voir la courbe plus bas.
5. **Une chose qu'aucun autre site ne fait.** Auteur : les mots du mur se
   retournent. Voir « Signature move ».
6. **Distance du premium-minimal.** **(client)** Audacieux. L'audace vient de
   l'échelle et du contraste, pas de l'encombrement : un seul accent, deux
   sols, et de très gros écarts de taille.
7. **Un monde continu ou des scènes distinctes.** Auteur : des scènes
   distinctes, à coupe franche. Grammaire **plaque et plan**, définie plus bas.
8. **Les actifs existants.** **(client)** Un logo et trois photographies,
   fournis en cours de build. Rien n'a été généré : aucune dépense, aucune
   image inventée. Les fichiers pesaient 21 Mo ; ils sont servis à 1,2 Mo, en
   deux largeurs par photo via `srcset`.

## Faits fixes (client)

- Nom : Lexma Électrique. Métier : électricien. Clientèle : **résidentiel et
  commercial**. Le commercial a été ajouté par le client après la première
  livraison ; la page avait été écrite « résidentiel seulement » et affirmait
  six fois que c'était un choix délibéré. Tout a été repris.
- Membre de la CMEQ.
- Téléphone : 450 756-7111. **Un seul numéro.**
- Courriel : gestion@lexma-electrique.com
- Adresse : 128, rue des Œillets, Saint-Ambroise-de-Kildare (Québec) J0K 1C0.
- **Licence RBQ : 5767-5993-01**, valide.
- Logo : lettres bleu nuit, éclair doré à la place du X. La palette de la page
  en sort : encre marine, or. La page n'invente pas de couleurs.

## Hypothèses d'auteur, signalées au client

- **Les trois services commerciaux sont d'auteur.** Le client a dit « ils font
  aussi commercial » et rien de plus. Les trois lignes écrites (locaux
  commerciaux, panneaux et distribution, entretien et dépannage) sont ce que
  fait n'importe quel entrepreneur en électricité titulaire d'une licence,
  donc rien n'y est inventé au sens fort, mais elles ne sont pas non plus
  dictées. Elles sont à confirmer ou à remplacer par ce que Lexma fait
  réellement.
- **L'industriel n'est pas mentionné.** Le client a nommé le commercial, pas
  l'industriel, et les deux ne se valent pas comme promesse.

- **Aucune heure d'ouverture** n'a été fournie, donc la page n'en affiche
  aucune. Inventer un horaire sur le site d'un entrepreneur est un engagement
  qu'il devra tenir.
- ~~Aucun numéro de licence RBQ.~~ **Corrigé après coup :** le client l'a
  fourni, 5767-5993-01. Il est maintenant sur la page à deux endroits, dont
  une plaque dans le plan de preuve, parce que c'est le fait le plus
  vérifiable du site : n'importe qui peut le valider au registre de la Régie
  du bâtiment du Québec.
- **Aucun prix, aucune garantie chiffrée, aucune statistique** nulle part,
  parce qu'aucune n'a été fournie et qu'en inventer est une responsabilité
  légale autant qu'une perte de crédibilité.
- ~~Le second numéro (576 759-9301).~~ **Erreur corrigée.** La suite
  `5767599301` fournie au départ n'était pas un téléphone : c'était le numéro
  de licence RBQ 5767-5993-01, saisi sans ses traits d'union. Elle a été
  publiée un temps comme second numéro d'appel avec un lien `tel:`. Le lien a
  été retiré et la valeur remise à sa vraie place. C'est aussi pour cela que
  576 ne ressemblait à aucun indicatif régional : le signal était bon, la
  lecture était fausse. Il n'y a qu'un seul téléphone, le 450 756-7111.
- ~~La région desservie.~~ **Précisée par le client :** la municipalité
  complète est Saint-Ambroise-de-Kildare, dans Lanaudière. La page l'écrit au
  long partout, y compris dans le titre et les données structurées, parce que
  c'est ce que les gens tapent dans une recherche locale. La zone servie
  reste « et les environs », qui est la seule formulation que les faits
  fournis autorisent.
- **Les photographies portaient des marques tierces.** Réglé de deux façons
  différentes, et le choix mérite d'être expliqué.
  La photo de la prise montrait « APEX Electrical Services » en toutes lettres
  sur le polo : inacceptable, et **recadrée**. Le cadre retenu garde les mains
  gantées, la prise ouverte, le mur, la plinthe, la toile et les outils au
  sol, et il sort le logo. C'est aussi une meilleure image de service qu'un
  portrait posé.
  La photo du panneau porte un écusson brodé illisible, dont le texte est
  inversé et qui ne nomme rien. Trois retouches ont été essayées (diffusion
  depuis la bordure, greffe de tissu propre, désaturation plus flou) et **les
  trois ont produit une tache plus visible que l'écusson d'origine**. Elles
  ont été abandonnées : la photo est publiée telle quelle, le cadrage portrait
  la sort du cadre sur téléphone, et la vraie correction, refaire la photo
  avec un vêtement Lexma, est écrite dans le README plutôt que maquillée.

---

## Grammaire : plaque et plan

Grammaire nommée, pas une des huit de `uniqueness.md` §2. Le skill autorise
une grammaire neuve « quand sa navigation, sa séquence, sa fin et ses
interdits décrivent une structure différente ». Les voici.

**L'unité.** La page alterne deux choses et rien d'autre.
Une **plaque** est du texte sur un sol plat, à l'échelle de l'affiche, sans
aucune image. Un **plan** est une photographie plein cadre, épinglée, avec une
seule idée par-dessus. Jamais les deux dans la même section.

**La transition.** Coupe franche, toujours. Aucun `drift`, aucun fondu entre
sections. Le passage plan → plaque est un cut, et c'est ce cut qui donne son
rythme à la page.

**La navigation.** Aucune en paysage : pas de barre, pas de logo fixe, pas de
jauge, pas d'ancre. En portrait, **une exception demandée par le client** : une
barre d'action fixe en bas de l'écran, deux boutons, Appeler et Courriel. Elle
contredit la règle que cette grammaire s'était donnée, et c'est assumé. Un
électricien résidentiel se fait joindre depuis un téléphone, et obliger
quelqu'un à remonter onze écrans pour retrouver le numéro coûte des appels.
Elle n'apparaît qu'après le premier écran, qui porte déjà son propre bouton,
et elle entre en animation de défilement native sous `@supports`, donc un
navigateur qui ne connaît pas la règle l'affiche simplement tout le temps.
S'ajoute un lien d'évitement vers les coordonnées, invisible tant qu'il n'a pas
le focus.

**Le héros.** Un plan, avec le mot-symbole posé dans le tiers bas du cadre,
protégé par une bande de densité et non par un voile plein écran. Le plan
garde ses deux tiers hauts intacts : la photographie est un actif, pas une
texture.

**La fermeture.** L'inversion. Après toute la page en bleu nuit, l'écran final
bascule en clair, tout y est petit, le vrai logo y vit nativement sur son sol
pâle, et l'appel à l'action est un lien souligné plutôt qu'un bouton.

**Interdits.** `scrub` (aucune vidéo), les rails `pan` de cartes, les cartes,
les compteurs, les numéros de chapitre, `spotlight`, `magnet`, les voiles
plein cadre, et tout fondu entre deux sections.

**Le sommet reste une histoire de maison.** Le mur qui se retourne parle de
cuisines, de sous-sols et de maisons de 1970, et il n'a pas été élargi au
commercial quand celui-ci est arrivé. Mêler les deux dans les six lignes du
sommet les aurait rendues génériques, et le sommet vit précisément de sa
précision. Le commercial est porté par la liste des services, par le plan de
preuve et par le formulaire ; l'arc émotionnel reste celui d'un propriétaire.
C'est un déséquilibre assumé, pas un oubli.

**Une plaque de travail.** La demande de soumission est une plaque comme les
autres : du texte sur un sol plat, des filets, aucune carte, aucune boîte. Les
champs sont soulignés plutôt qu'encadrés, exactement comme les lignes de la
liste des services. Son titre descend d'un cran sous l'échelle d'affiche des
autres plaques, pour deux raisons : le sommet doit rester le plus gros
événement visuel de la page, et un formulaire poussé sous la ligne de
flottaison par un titre de 166 px est un formulaire qu'on ne remplit pas.

**Pourquoi pas les huit autres.** *Filmique en un plan* demande du métrage et
interdit les coupes franches, qui sont ici le rythme. *Éditorial chapitré*
demande de la matière longue et de la retenue papier, à l'opposé de
« audacieux ». *Surface vivante* : il n'y a pas de produit qui tourne. *Monde
continu* demande une géographie réelle et de la vidéo, et `justing` l'occupe.
*Galerie* demande une gamme d'objets ; il y a un métier et une clientèle.
*Scène scindée* est occupée par `fred-gagner-antirouille` et le métier n'est
pas une comparaison à deux côtés. *Cutlist rythmique* est la grammaire des
marques d'énergie ; à côté d'une décision à quatre chiffres sur une maison,
elle serait non sérieuse. *Affiche typographique* était la bonne réponse tant
qu'il n'y avait aucun visuel, et elle interdit le sol photographique : elle est
tombée avec l'arrivée des photos.

## Signature move : le mur qui se retourne

Une plaque épinglée tient six lignes de très gros texte, empilées comme des
mots peints sur un mur. Chaque ligne porte **deux** textes dans exactement la
même case de grille : ce que le propriétaire voit, et ce que l'électricien
trouve derrière. Chaque ligne a son propre seuil, écrit en attribut (`--at`),
et l'opacité des deux couches se calcule en CSS pur à partir de `--sc-p`, la
progression que le moteur publie sur l'acte :

```css
.lx-wall__face { opacity: clamp(0, calc((var(--at) - var(--sc-p, 0)) * 36), 1); }
.lx-wall__true { opacity: clamp(0, calc((var(--sc-p, 0) - var(--at)) * 36), 1); }
```

Le facteur 36 rend la bascule quasi instantanée : ce n'est pas un fondu, c'est
un claquement, comme un disjoncteur. Les seuils ne suivent pas l'ordre
vertical (4, 1, 6, 2, 5, 3), donc le mur ne s'essuie pas de haut en bas, il se
retourne par endroits ; à mi-acte il est moitié façade, moitié vérité.

Trois propriétés qui en font autre chose qu'un effet :

- **Le moteur n'est pas touché.** Tout vit dans la page.
- **Aucun `clip-path`, aucun masque, aucun curseur.** Ça fonctionne
  identiquement au doigt, ce qui compte parce que le client d'un électricien
  résidentiel lit sur un téléphone. C'est aussi ce qui le distingue du
  Rebuild Scrubber de `justing`, qui est un essuyage `clip-path`.
- **Aucun `transform`, aucune `transition`.** Le mouvement réduit ne lui
  enlève rien : un visiteur en `prefers-reduced-motion` voit exactement le
  même sommet.

## Gate des empreintes

Registre : `scrollcraft/FINGERPRINTS.md`, deux lignes.

| Dimension | vs `fred-gagner-antirouille` | vs `justing` |
|---|---|---|
| 1 Grammaire | plaque et plan ≠ scène scindée ✔ | ≠ worldflight ✔ |
| 2 Nav | aucune chrome ≠ la ligne médiane EST la chrome ✔ | ≠ barre fixe + CTA fantôme ✔ |
| 3 Héros | plan plein cadre, mot-symbole dans le tiers bas sous bande ≠ split 50/50 établi ✔ | ≠ objet cadre-navigateur, titre centré ✔ |
| 4 Séquence | 3 plans épinglés et 4 plaques, ~10,7vh ≠ 4 actes épinglés, 6,6vh ✔ | ≠ 4 legs, 6,6vh ✔ |
| 5 Fermeture | inversion en clair, typo minuscule, lien souligné ≠ effondrement vers un agenda ✔ | ≠ bouton centré tenu ✔ |
| 6 Signature | le mur qui se retourne ≠ curseur de saison ✔ | ≠ Rebuild Scrubber ✔ |

**6 sur 6 contre chaque ligne.** Le gate en demande 4. Passé.

---

## La courbe de ressenti

```
1  Plan héros    Assurance        un camion équipé, déjà dans une entrée comme la vôtre
2  Plaque        Reconnaissance   quatre phrases que le visiteur a déjà dites
3  Plaque        Inquiétude calme une seule ligne sur un écran vide
4  SOMMET        Révélation       les mots du mur se retournent un par un
5  Plaque        Compétence       la liste, en texte nu, et une photo de vrai travail
6  Plan preuve   Sécurité         la CMEQ, la licence, ce que ça veut dire en droit
7  Plaque devis  Passage à l'acte on lui demande son projet, il l'écrit
8  Fermeture     Décision simple  tout devient clair et minuscule, le numéro
```

Aucun ressenti ne se répète d'un acte à l'autre. L'acte 3 est le silence
d'auteur : une ligne, aucune animation sauf l'opacité et l'essuyage, juste
devant le plus bruyant. Il tient une phrase, ce n'est pas du scroll mort.

## Le sommet

> « J'ai scrollé et les mots du mur se sont retournés un par un pour me dire
> ce qu'il y a vraiment dedans. »

Acte 4. Plus grande travée de la page (2,8 hauteurs de fenêtre contre 1,45
pour le héros et 1,6 pour la preuve), la plus grosse typo du site, et l'acte
le plus silencieux juste devant.

## Phrase à raconter

C'est le site où les mots écrits sur le mur se retournent et te disent ce
qu'il y a vraiment derrière.

## La partition

| Temps | Appareil | Pourquoi celui-là |
|---|---|---|
| Héros | `pin` + caméra depuis `--sc-p`, cue « greet and hold » | La composition est entière au premier pixel, puis la caméra avance dans le cadre |
| Tension | `flow` + `in` échelonné, `kinetic` mots | Quatre phrases en ordre de lecture, une fois, sans se recacher |
| Silence | `reveal` sur un emballage | Un essuyage est un changement d'état, et il est ici seul sur l'écran |
| **Sommet** | `pin` + le mur (CSS de page sur `--sc-p`) | La bascule par seuil, la plus grande travée |
| Substance | `flow` + `in`, `reveal` sur la photo | Une liste se lit ; la photo entre par un essuyage, pas par un fondu |
| Preuve | `pin` + caméra, `kinetic` lignes | Le fait légal sur le geste qui l'illustre, en plein cadre |
| Soumission | `flow` + `in` sur le titre seul | La page arrête d'argumenter et tend un outil. Le titre arrive, le formulaire ne bouge pas : animer des champs pendant qu'on essaie de les remplir est une punition, pas une attention |
| Fermeture | section claire à coupe franche | L'inversion est un cut, pas une interpolation |

Familles distinctes : `pin`, `flow`/`in`, `reveal`, `kinetic`, plus la coupe
de fond et la caméra de page. Cinq au moins, le plancher en demande quatre.
Aucune famille deux fois de suite (pin, flow, reveal, pin, flow, pin, flow).
Aucun `scrub` : la grammaire l'interdit et il n'y a pas de vidéo. Aucun
`drift` : `devices.md` §10 interdit d'interpoler du presque-noir vers du
clair, donc chaque changement de sol est une arête franche.

Longueur mesurée : environ 12 hauteurs de fenêtre en paysage (11,9 à
1280x840, 12,2 à 1280x860), sur 8 sections. Hors de la bande 6 à 7 actes / 13,6 à 13,8vh
qu'ont tous touchée les builds de l'auteur du skill, et hors des 6,6vh des
deux lignes du registre.

## Les animations, et pourquoi elles sont celles-là

Tout ce qui bouge est entraîné par le scroll ou par le chargement, en
`transform`, `translate`, `opacity` ou `clip-path`, et rien d'autre. Aucune
boucle infinie, aucun `autoplay`, aucune vidéo : rien ne s'agite pendant que
le visiteur lit.

**L'arrivée.** Le mot-symbole, la phrase et le bouton montent de 26px en
740 ms, échelonnés de 60, 210 et 300 ms, une seule fois au chargement. Ce
n'est pas un fondu au scroll : le plancher exige que le héros soit plein dès
le premier pixel, donc la seule entrée autorisée est celle qui se termine
avant que le visiteur ait eu le temps de défiler. Elle écrit `translate` et
non `transform`, pour ne pas entrer en collision avec la dérive de parallaxe
qui vit sur les mêmes éléments.

**La profondeur du héros.** Trois plans à trois vitesses : la photo recule de
2,4vh en grandissant de 1,07 à 1,16, le mot-symbole suit à 2,2vh, le pied de
composition à 0,9vh. Mesuré : 21,4px, 16,9px, 6,9px de bout en bout. C'est
cette différence de vitesse, et rien d'autre, qui sépare une scène d'une image
de fond avec du texte posé dessus.

**Le mur.** Le sommet. L'opacité claque au seuil de chaque ligne, et un
déplacement de 10px claque avec elle : la vérité entre par la droite, la
façade sort par la gauche. Les deux valeurs sont bornées par `clamp`, donc
hors du seuil elles valent exactement 0 et rien ne flotte. C'est le déclic
d'un disjoncteur, pas un fondu.

**Les filets de la liste.** Chaque ligne de service voit son filet se tracer
de gauche à droite en 700 ms plutôt qu'apparaître. Le retard est déclaré
`transition-delay: inherit` sur le pseudo-élément, donc il va chercher
l'échelonnement que le moteur pose sur l'article : le trait suit exactement la
cascade du texte, sans une seule valeur dupliquée.

**La caméra de la photo de service.** Même mouvement que les plans, en plus
discret : de 1,02 à 1,10 pendant qu'on lit la liste à côté.

**Les listes.** Opacité plus 14px de montée sur 620 ms, échelonnées de 60 à
70 ms, déclenchées une seule fois à l'entrée. Plus grand, plus lent ou plus
rebondi n'est jamais plus premium ; la retenue est le signal.

**La fermeture.** Elle porte le numéro de téléphone, donc son entrée est une
**animation de défilement native** (`animation-timeline: view()`), sous
`@supports`, et non un `data-sc-in`. La différence compte : avec `data-sc-in`,
le bloc part à opacité 0 et attend qu'un `IntersectionObserver` le révèle ; si
le script ne tourne pas, le contenu le plus important de la page n'existe
pas. Avec `@supports`, un navigateur qui ne connaît pas la règle affiche
simplement le bloc, complet et immobile. C'est l'inverse du réflexe habituel,
et c'est le bon sens dans lequel prendre le risque.

**La demande de soumission.** Le titre et la phrase montent une fois à
l'entrée. Le formulaire, lui, ne bouge pas : échelonner l'apparition de champs
pendant que quelqu'un essaie de les remplir est une punition déguisée en
attention.

**La barre d'action du téléphone.** Elle monte depuis le bas entre 55 % et 92 %
de la première hauteur d'écran, en `animation-timeline: scroll(root block)`.
Native, donc sans script, et sous `@supports`, donc toujours visible sur un
navigateur qui ne connaît pas la règle.

**Mouvement réduit.** Les caméras se figent, les montées et les déplacements
tombent, les opacités et les essuyages restent. Vérifié en simulant le
contrat : à `--sc-p` = 0,62, avec tous les `transform` neutralisés, le mur
affiche toujours quatre lignes retournées sur six. Le sommet de la page ne
dépend d'aucun déplacement.

## Direction artistique du téléphone

Le mur et le plan de preuve changent de traitement en portrait, et c'est
délibéré.

- **Le mur.** En `nowrap`, la plus longue ligne plafonne le corps à environ
  25px sur un écran de 375 : ce n'est plus un mur, c'est une légende. En
  portrait les lignes passent à 9,6vw, et les deux formules les plus longues
  ont été raccourcies (« fils sans terre », « circuit de trop ») pour que rien
  ne se replie et que les six lignes gardent la même hauteur, sinon la bascule
  laisserait un trou dans le mur.
- **Le cadrage des plans.** Une photo paysage dans un cadre 375x812 ne montre
  que 31 % de sa largeur. Au centre, le camion perdait l'électricien et la
  maison, c'est-à-dire toute l'histoire. Chaque plan a donc son propre point
  d'ancrage en portrait (`object-position`), remonté pour que le sujet ne
  passe pas sous la bande de copie. Effet secondaire utile : le cadrage
  portrait du panneau sort l'écusson du vêtement hors du cadre.
- **Le plan de preuve.** En paysage la copie tient une colonne à gauche et le
  dégradé est une colonne. En portrait la copie prend toute la largeur : le
  dégradé redevient une bande basse et la copie descend l'y rejoindre. Laisser
  la copie centrée au-dessus d'une bande basse est la façon la plus courante
  de rater un contraste sur téléphone, et elle est invisible sur un écran
  large.
- **Les cibles tactiles.** Le bouton d'appel prend toute la largeur, et les
  numéros de la fermeture sont rembourrés. Un numéro qu'on rate est un appel
  perdu.

## La page de confidentialité, et ce qu'elle a coûté

Écrire une politique de confidentialité honnête a obligé à auditer ce que le
site fait vraiment. Résultat de l'audit : aucun témoin, aucun stockage local,
aucun script tiers, aucun outil de mesure, et **une seule ressource externe**,
le CDN de polices de Google, qui reçoit l'adresse IP et le navigateur de chaque
visiteur.

C'était la seule chose que la politique aurait eu à déclarer, et la déclarer
aurait été moins bon que la supprimer. Les deux familles sont sous licence
libre, donc les fichiers ont été rapatriés dans `assets/fonts/`, en latin
seulement, 228 Ko, avec les plages unicode et les axes variables conservés
tels que Google les déclare. Le site ne contacte plus personne.

La page elle-même est volontairement dépouillée : aucun script, aucune image,
aucun tiers. Un document qui décrit la sobriété d'un site aurait mauvaise
grâce à la contredire. Elle reprend le sol clair de la fermeture, ce qui la
rattache visuellement à la page sans copier sa grammaire, puisqu'elle n'en a
pas besoin : c'est du texte long, et le texte long se lit en colonne.

## Ce qui a été vérifié, et comment

- **Contraste, mesuré sur le composite réel.** La photo est redessinée dans un
  canvas avec le même `object-fit: cover` et le même `object-position` que la
  page, le dégradé est reconstruit par-dessus, puis on échantillonne le pixel
  **le plus clair** sous chaque ligne de texte. Héros : 7,2 / 11,0 / 15,3 /
  13,4 pour des minimums de 3 et 4,5. Plan de preuve : 14,9 / 14,0 / 11,7 pour
  un minimum de 4,5. Sur fond plat, les 40 et quelques éléments de texte de la
  page passent tous, aucun en dessous du seuil.
- **Structure.** Sept sections, sept titres. Les trois plaques narratives n'en
  avaient aucun : à la lecture d'écran la page était une suite de blocs
  anonymes. Deux titres sont désormais réservés au lecteur d'écran. La
  fermeture est un `<footer>`. Le logo passe en `alt=""` : il répétait à voix
  haute le nom écrit juste dessous.
- **Clavier.** Un lien d'évitement vers les coordonnées, invisible tant qu'il
  n'a pas le focus, parce que la page fait onze hauteurs d'écran et n'a aucune
  barre de navigation. Quatre liens au total, tous réels, dans l'ordre du
  document.
- **Aucun débordement horizontal** à 1440, 1024 et 375.
- **Longueur** : environ 12 hauteurs de fenêtre en paysage.
- **Le formulaire.** Validation à vide, partielle et complète : le message
  nomme les champs manquants dans un français qui se lit (« Il manque votre
  nom, votre téléphone et une description du projet. »), le focus saute au
  premier champ vide, et le message disparaît dès la première frappe. L'URL
  `mailto:` composée à partir d'un cas réaliste et long fait 1018 caractères,
  bien en deçà de la limite où les logiciels de messagerie coupent, avec les
  accents et les sauts de ligne correctement encodés.
- **La barre d'action.** Absente sur le premier écran, présente ensuite,
  70 px de haut pour un minimum recommandé de 44, et elle ne recouvre ni la
  dernière ligne du pied de page ni le bouton d'envoi du formulaire.

## Ce qui n'a pas pu être vérifié

- `doctor.mjs` signale l'absence de Chrome et de `playwright-core` sur cette
  machine, donc le harnais `shoot.mjs` n'a pas tourné et il n'y a pas de
  planche-contact. La vérification a été faite à la main dans le navigateur
  intégré : héros, tension, silence, sommet à 0,10 / 0,50 / 0,90, services,
  preuve et fermeture, en 1440x900, 1024x768 et 375x812, plus l'ordre de
  tabulation et l'absence de débordement horizontal.
- Les dégradés ont d'abord été réglés contre des images de substitution
  volontairement **presque blanches**, le pire cas possible pour du texte
  clair, puis **revérifiés sur les vraies photographies** une fois celles-ci
  en place, en paysage et en portrait. Aucune mesure instrumentée du contraste
  composite n'a été faite, faute du harnais : le jugement est visuel, sur un
  réglage calibré au pire cas.
- **Aucun vrai téléphone.** Le navigateur intégré émule un écran, pas un
  appareil.

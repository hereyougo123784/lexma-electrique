# Les visuels

Tous en place. Les sources sont les fichiers fournis par le client ; ce qui
est ici a été redimensionné et compressé pour le web (21 Mo au départ, 1,2 Mo
au total maintenant).

| Fichier | Contenu | Dimensions |
|---|---|---|
| `logo-lexma.png` | Le logo LEXMA | 447 × 447 |
| `plan-camion.jpg` | Le camion dans l'entrée | 2000 × 1116 |
| `plan-camion-800.jpg` | La même, version téléphone | 800 × 446 |
| `plan-panneau.jpg` | L'électricien au panneau | 2000 × 1493 |
| `plan-panneau-800.jpg` | La même, version téléphone | 800 × 597 |
| `plan-prise.jpg` | Les mains gantées sur la prise | 810 × 1080 |
| `plan-prise-480.jpg` | La même, version téléphone | 480 × 640 |

Les deux largeurs sont servies par `srcset` : un téléphone télécharge 80 Ko au
lieu de 460 Ko pour la photo d'ouverture.

## Une modification apportée à une photo

`plan-prise.jpg` est **recadrée**. L'originale montrait un électricien de
trois quarts avec un polo portant, bien lisible, le logo « APEX Electrical
Services ». Publier ça sur le site de Lexma n'était pas envisageable. Le
recadrage garde les mains gantées, la prise ouverte, le mur, la plinthe, la
toile de protection et les outils au sol, et il sort le logo du cadre. Le
résultat est aussi une meilleure image de service qu'un portrait posé.

Les deux autres photos ne sont pas retouchées.

## Le logo du panneau, effacé

`plan-panneau.jpg` portait un écusson brodé sur la poitrine. Il a été retiré :
les pixels de la broderie sont détectés par leur teinte (orange et cyan, hors
de la plage du tissu bleu marine) et par leur écart à un filtre médian, puis
reconstruits par diffusion depuis le tissu voisin, avec le grain du tissage
réinjecté à son amplitude mesurée. Les plis et le dégradé de lumière sont
intacts ; seule la broderie a disparu.

Un tirage à vos couleurs resterait préférable à une retouche, mais la photo
est publiable telle quelle.

## Le logo

`logo-lexma.png` est détouré : le fond blanc du fichier d'origine est devenu
transparent, sinon il dessinait une boîte blanche sur le gris pâle de la
fermeture. Les marges vides ont été rognées, d'où le format 423 × 123 plutôt
que le carré de départ.

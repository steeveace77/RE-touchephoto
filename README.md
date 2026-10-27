# RE-touchephoto — Android v0.3 (prototype)

Éditeur photo natif Android, sans publicité ni abonnement.

## Outils disponibles
- Importer une image depuis le téléphone
- Ajouter une image comme calque superposé
- Régler luminosité, contraste, saturation
- Convertir en noir et blanc
- Recadrage progressif au centre (90 % par pression)
- Rotation photo par 90°, miroir
- Déplacer le calque au doigt ou par flèches, redimensionner, tourner, régler sa transparence, supprimer
- Annuler / rétablir (jusqu'à 40 états)
- Exporter en PNG ou JPEG dans la galerie

## Limites connues
- Pas encore de sélection au lasso, gomme, masques, détourage, suppression d'objets, remplissage intelligent, ni IA.
- Un seul calque photo superposé pour le moment.
- La prévisualisation utilise des images réduites à 3200 pixels de côté au maximum.
- L'interface et les outils sont expérimentaux; la compilation et les tests sur appareil restent à confirmer.

## Compiler
GitHub Actions > Compiler APK Android > dernière exécution > Artifacts > RE-touchephoto-APK.
Le workflow est déclenché automatiquement lors des commits sur main.

## Version 0.4 — remplacement de couleur
- Pipette tactile pour échantillonner une couleur sur la photo
- Choix parmi 10 teintes de remplacement
- Seuil de tolérance réglable (sélection par proximité de teinte HSV)
- Conservation approximative de la luminosité d'origine pour préserver les ombres
- Activation et désactivation de la recoloration
- Commandes tactiles utilisables au doigt et avec un stylet Android compatible

**Limite** : la sélection s'applique aux pixels de teinte proche dans toute l'image, et pas seulement à l'objet touché. Une sélection localisée au lasso, les masques et le traitement des objets restent à développer. L'APK et l'ergonomie n'ont pas encore été testés sur un téléphone.

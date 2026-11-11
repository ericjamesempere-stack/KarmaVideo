# KarmaVideo V18 — zéro euro

Application web statique. Aucun serveur ni abonnement requis pour les fonctions locales.

## Fonctions
- Import d'images, vidéos et musique depuis Android.
- Découpage de texte en cartes de scènes, ordre et suppression.
- Prévisualisation Canvas et export WebM via MediaRecorder (dépend du navigateur et de ses codecs).
- Sauvegarde JSON du plan de montage, sans intégrer les médias (les fichiers doivent être réimportés).
- Liens vers des recherches de démonstrations publiques Wan Animate, Wan 2.2 et LTX. Aucune API distante n'est intégrée ni présentée comme fonctionnelle.

## Utilisation
Ouvrir index.html dans un navigateur moderne, ou héberger les trois fichiers sur un hébergement statique HTTPS gratuit. Sur Android, l'export MediaRecorder et le mixage audio dépendent du navigateur. Le rendu s'effectue en temps réel : un clip de 60 s demande au moins 60 s. Pour obtenir MP4, convertir le WebM dans une application de montage Android compatible.

## Limites importantes
- Ce n'est pas un moteur génératif IA autonome. Les liens vers des démos peuvent ne pas être accessibles.
- Les clips MP4 et le rendu Wan ne sont pas fournis par ce prototype.
- La piste audio n'est pas synchronisée à des timecodes précis.
- Les vidéos sont dessinées sans audio source (la musique importée est la seule piste audio du rendu).
- Les fichiers médias ne persistent pas après rechargement de la page.
- Ne pas contourner les quotas des services publics.

## Validation
Tests statiques et syntaxiques possibles avec Node et Python. La compatibilité sur le Xiaomi 14T Pro exige un test manuel sur l'appareil ; aucun test de navigateur Android n'est revendiqué.

# Publier les mises à jour de Manga Caisse GeekWiller

Ce dépôt sert **uniquement à distribuer les installateurs officiels**. Aucune donnée de caisse ou de client ne doit y être ajoutée.

## État au 18 novembre 2026

- Le dépôt est créé et public.
- La v1.5 **de test** est reliée à ce dépôt pour consulter GitHub Releases.
- **Aucun installateur officiel n'est encore publié.** Le résultat normal du bouton « Vérifier en ligne » est donc : « Aucune mise à jour publiée pour le moment ».
- Le PC Windows 10 de la boutique n'a pas encore servi à tester l'installation.

## Avant de publier une version

1. Finaliser le code et vérifier les tests sur Windows 11 **et** sur Windows 10.
2. Fabriquer l'installateur de la version à publier.
3. Vérifier sur un PC de test que l'installation conserve le catalogue, le stock, les ventes et les jaquettes, et qu'un retour arrière est possible.
4. Vérifier l'empreinte SHA-256, la provenance et, à terme, la signature de l'installateur.
5. Créer une **Release** GitHub stable, par exemple avec le tag `v1.6.0`, puis ajouter le fichier `INSTALLER-GEEKWILLER-v1.6.0.exe`.
6. Tester depuis la v1.5 installée le bouton « Vérifier en ligne », puis le téléchargement. Aucune installation ne doit se lancer toute seule.

## Format obligatoire

- Numéro croissant : `vMAJEUR.MINEUR.PATCH` (exemple `v1.6.0`).
- Fichier de la Release : `INSTALLER-GEEKWILLER-vMAJEUR.MINEUR.PATCH.exe`.
- Dépôt : `victorfischer68/GeekWiller-Updates`.
- Ne pas utiliser les options **Draft** ou **Pre-release** pour une version destinée au logiciel installé.

## Confidentialité

Ne jamais déposer de `catalogue.json`, sauvegarde, historique de vente, dossier de jaquettes, coordonnées de clients, mot de passe ou jeton GitHub dans ce dépôt **public**.

**Important :** le dépôt GitHub seul ne rend pas une mise à jour opérationnelle. Elle exige un véritable installateur, validé pour Windows 10 et Windows 11.

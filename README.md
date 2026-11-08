# TimeTracker — versions publiées

Installeurs de [TimeTracker](https://github.com/OlderGlow/TimeTracker-Rust) (Windows, macOS, Linux) et fichier
`latest.json` lu par la mise à jour automatique de l'application.

Ce dépôt ne contient pas le code de l'application. Chaque version est construite et publiée ici par le workflow
[Release](.github/workflows/release.yml), lancé à la main : il récupère le code du dépôt privé le temps du build, puis
dépose les installeurs et `latest.json`. Windows est toujours construit ; macOS et Linux seulement si leur case
est cochée au lancement. Télécharger la dernière version : [Releases](../../releases/latest).

Les installeurs ne sont pas signés par un certificat Apple ou Windows : macOS et Windows affichent un avertissement à la
première ouverture. Les mises à jour, elles, sont signées (clé Tauri) et vérifiées par l'application avant installation.

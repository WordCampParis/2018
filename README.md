# 2018

## Mise en place de l'environnement

- Installer [VVV 2.0](https://github.com/Varying-Vagrant-Vagrants/VVV/releases/tag/2.0.0)
- Créer un fichier de config custom en copiant celui fournit par défaut: vvv-config.yml -> vvv-custom.yml
- Décommenter les lignes 28 et 29 de `vvv-custom.yml` de sorte à avoir :

```
wordpress-meta-environment:
    repo: https://github.com/WordPress/meta-environment.git
```

Il ne restera plus qu'à jouer ces commandes :

```
vagrant halt
vagrant up --provision
```

## Mise en place de l'apparence via le customizer

- TwentySeventeen
- Page statique en page d'accueil avec utilisation des panels,
- Logo personnalisé et couleurs personnalisées en choisissant `#144f8f` comme couleur du texte d'entête,
- Désactivation du header,
- Retrait de tous les widgets de la sidebar,
- Utilisation d'un menu social,
- Utilisation d'un menu principal.

## Mise en place de la Remote CSS

- Depuis le menu "Apparence" de l'administration du site, activer le sous-menu "Remote CSS".
- Coller le lien vers le style.css du repo: `https://api.github.com/repos/WordCampParis/2018/contents/style.css`
- Laisser l'option sur "Add-on".
- Cliquer sur le bouton "Update" (répéter ce click à chaque édition du fichier style.css du repository 2018).

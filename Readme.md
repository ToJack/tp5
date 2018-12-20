# TP 5 : Kubeflow labs
Ce TP utilise les ressources mises à disposition par Azure pour déployer une instance Kubeflow et distribuer un modèle Tensorflow entrainé.

## Mise à jour
Après avoir forké le repo, pour se mettre à jour avec la dernière version, exécuter les commandes suivantes:
```bash
git remote add parent https://github.com/cours-ece/tp5.git
git pull
```

## Instructions
Pas de **answers.md** pour ce tp. Le but est de manipuler toutes les notions vues en tp depuis le premier TP.

Suivre le [lab Azure](https://github.com/Azure/kubeflow-labs) en prenant en compte les remarques ci-dessous

> Lire chaque partie Context et réaliser uniquement la partie Exercise

# 2 Kubernetes
Modifier l'exemple de tensorflow pour utiliser l'image de base (non gpu) que vous avez push lors de l'étape précédente.

> Penser à supprimer les montages et les limites nvidia

# 3 Helm
Pas obligé d'installer dokuwiki

# 4 Kubeflow
Si problème lors du `ks pkg install`
https://github.com/ksonnet/ksonnet/blob/master/docs/troubleshooting.md#github-rate-limiting-errors

# 5 Jupyterhub
Dans la partie Spawner Options, ne pas rentrer de valeur dans "Extra Resource Limits" et remplir uniquement le champ image. Utiliser une image *-cpu


# PowerShell-PostInstall

## Fonctionnalités du script Init
- Téléchargement des scripts
- Récupération de l'IP de la VM
- Récupération du nom du client en fonction de l'IP
- Récupération du CSV du client en fonction de son nom

## Lancement
- La première commande définit la politique d'exécution en mode "non restreint"
- La seconde télécharge le script d'Init et le place à la racine de C:
- La troisième lance le script d'Init

```
Set-ExecutionPolicy -Force Unrestricted
Invoke-WebRequest -Uri https://projet-m1-powershell.zaniah.eu/19AxxjukqsLJbFkVzquL/Scripts/PostInstall/Init.ps1 -OutFile C:\Init.ps1
powershell C:\Init.ps1
```

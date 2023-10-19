# installing-firebase-cli

https://bobbyhadz.com/blog/flutterfire-is-not-recognized-as-internal-or-external-command



```
PS C:\Users\medam\Documents\elearny_app_0> firebase login
firebase : Impossible de charger le fichier C:\Users\medam\AppData\Roaming\npm\firebase.ps1, car l’exécution de scripts est désactivée sur ce système. Pour plus d’informations, consultez about_Execution_Policies à l’adresse 
https://go.microsoft.com/fwlink/?LinkID=135170.
Au caractère Ligne:1 : 1
+ firebase login
+ ~~~~~~~~
    + CategoryInfo          : Erreur de sécurité : (:) [], PSSecurityException
    + FullyQualifiedErrorId : UnauthorizedAccess
PS C:\Users\medam\Documents\elearny_app_0>
```

https://learn.microsoft.com/fr-fr/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-7.3



>> solution : https://stackoverflow.com/questions/60594178/firebase-cannot-be-loading-because-running-scripts-is-disabled-on-this-system

https://stackoverflow.com/a/77202333/10216101

run powershell as admin :

```
Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
```



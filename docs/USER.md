# Manuel pour les utilisateurs

# SOMMAIRE
+ [Gestion des adhérents](#adherent)
+ [Gestion des tiers](#tiers)
+ [Exporter des adhérents](#export)
+ [Créer une facture](#facture)
+ [Ajouter un service/produit](#serv-prod)
+ [Module de caisse](#caisse)
+ A voir : gestion resssources; encaissement ; mailing

## INFO
+ Les champs en bleu sont à remplir obligatoirement.
+ Edition de facture impossible sans associer un tiers à un adhérent


## <a name="adherent"></a>GESTION DES ADHERENTS

### Comment ajouter un nouvel adhérent
+ Se positionner dans le module Adhérents (cliquer sur l'icone adhérents située en haut à gauche)
+ cliquer sur "Nouvel adhérent" dans la liste à gauche
+ Choisir le type d'adhérent : particulier ou assoc ou pro ou entreprise
+ Choisir la nature : physique ou moral
+ Entrer nom, prénom,  adresse, mail, téléphone
+ Cocher "oui" si mineur -18ans. Si oui, cocher oui si attestation parentale fournie
+ Cocher les différents choix pour réglement intérieur, autorisation image, attestation assurance et convocation AG...
+ Si besoin compléter les champs profession et ajouter des infos
+ cliquer sur le bouton "créer adhérent" : la fiche est créée mais l'adhérent n'est pas encore validé (fiche à l'état de brouillon)

### Toujours valider un nouvel adhérent après l'avoir ajouter
+ Après création  de l'adhérent, on arrive sur sa fiche
+ cliquer sur le bouton valider (confirmer par oui dans la boite de dialogue qui s'ouvre)

### Enregistrer paiement cotisation (1ere adhésion ou renouvellement)
+ Aller sur la fiche de l'adhérent puis sur l'onglet Adhésions/Cotisations
+ cliquer sur "créer cotisation"
+ Choisir date de début d'adhésion
+ Pas besoin d'entrer la date de fin (automatiquement 1 an)
+ Entrer le montant de l'adhésion
+ Si besoin modifier le "libellé"
+ Action complémentaire : choisir aucun pour l'instant  (qd config, possibilité créer écriture comptable direct avec paiement et en plus si besoin de générer automatiquement la facture : attention pas de brouillon, incrémente directement le numéro de facture non modifiable)
+ Valider en cliquant sur "créer cotisation"


### Comment rechercher un adhérent puis accéder/mofifier fiche
+ Se placer dans le module adhérent
+ Dans la colonne de gauche choisir "liste" pour voir tous les adhérents ou bien choisir selon les attributs proposés (à jour...)
+ On peut trier les adhérents suivants les attributs proposés (nom, prenom, etc.) ou directement entrer un nom, un prenom... dans les cases situé au desssus du nom des atrributs. Puis cliquer sur la loupe pour valider le tri.
+ Cliquer sur le numéro de  "Réf." pour accéder à une fiche

### Comment résilier un Adhérent
+ Aller sur la fiche de l'adhérent
+ Cliquer sur résilier (puis valider par oui).


## <a name="tiers"></a>GESTION DES TIERS
+ Un tiers peut-être un client/prospect ou un fournisseur. Pour le FabLab les membres qui achètent des prestations (ex : découpe laser) sont donc des clients.
+ Pour pouvoir éditer une facture, il faut avoir d'abord créer un tiers client que l'on va ensuite reliéer à l'adhérent 

### Créer un tiers à partir de la fiche d'un adhérent
+ Aller sur la fiche de l'adhérent
+ Cliquer sur "créer un tiers" (bouton vert en bas de la fiche)
+ Renseigner/modifier si besoin le nom du tier
+ Valider le tiers

## <a name="facture"></a>CREER UNE FACTURE
### Pour une adhésion
+ Créer puis valider le membre si besoin, sinon aller sur sa fiche
+ Dans l'onglet Adhésion/Cotisation, cliquer sur "créer cotisation"
+ Renseigner date et montant d'adhésion
+ Au niveau du champs "Action complémentaire à l'enregistrement", sélectionner  "Créer une facture avec paiement sur compte bancaire ou caisse"
+ Cliquer sur "créer un tiers", un boite de dialogue apparait
+ Vérifier les infos puis valider
+ Renseigner le compte, le mode et la date du réglement
+ Cliquer sur "créer cotisation".

### Pour une prestation (ou un produit)
+ Nota : il faut avoir créer le tiers préalablement (voir [ici](#tiers))
+ Aller dans le module "facturation/paiement"
+ Choisir "nouvelle facture "
+ Choisir le nom du client (tiers)
+ Choisir la date de Facturation
+ Laisser condition réglement "A réception"
+ Cliquer sur "créer brouillon"
+ On accède à la fiche de la facture
+ Ajout nouvelle ligne : ajouter le type de prestation (choix menu déroullant) et le montant. Valider en cliquant sur "ajouter". (si le produit/service n'existe pasdans la liste il faut le créer ou si c'ets un service/produit non redondant on peut saisir manuellement le libellé et le prix)
+ On peut alors cliquer sur "valider". Boite de dialogue pour confirmation avec indication numéro de facture (ATTENTION : va alors créer un numéro de facture, on ne peut alors plus supprimer la facture ; pour l'annuler il faudra obligatoirement faire une facture d'avoir)
+ Imprimer la facture

## ENTRER UNE NOTE DE FRAIS
+ Aller dans le module GRH
+ Choisir Nouveau
+ Remplir les champs puis valider

## FAIRE UN DEVIS
+ Aller dans le module "Commercial
+ Choisir "nouvelle proposition"
+ remplir les champs puis Valider

## <a name="export"></a>EXPORTER DES ADHERENTS
+ Aller dans l'onglet "Outils"
+ Sélectionner nouvel export
+ Sélectionner le lot à exporter : ici "adhérents" (cliquer sur le soleil tout à droite)
+ Choisissez les champs à exporte ou un profil prédéfini (par exemple "mailing newsletter") ; cliquer sur sélectionner pour valider le profil prédéfini. Puis cliquer sur suivant
+ Ajouter si besoin des filtres sur les champs puis suivant
+ Choisir l'ordre des champs puis cliquer sur étape suivante
+ choisir le format d'export : CVS
+ Cliquer sur "Générer" (*Attention cliquer toujours sur "Générer" même si il a déjà un fichier pour être sur qu'il soit bien mis à jour*)
+ Cliquer sur le fichier générer pour le télécharger

*Remarque : le profil "mailing newsletter" est défini pour récupérer les mail des adhérents valides (à jour et non à jour) qui ont acceptés l'envoi de la newsletter*

## <a name="serv-prod"></a> AJOUTER UN NOUVEAU SERVICE/PRODUIT
+ Aller dans le module "Produits/Services"
+ Choisir nouveau produit ou nouveau service
+ Entrer une référence en débutant par un des préfixes for, loc...  (ex: "for_laser" pour formation découpe Laser)
+ Entrer le libellé du service/produit
+ Choisir la catégorie/tag du service ou produit
+ Si besoin ajouter d'autres élément dans le champs "Description"
+ Choisir si besoin l'unité de temps
+ Entrer le prix de vente du produit/service
+ Choisir le code comptable à la vente (demander si besoin)
+ Cliquer sur créer

### Créer une nouvelle catégorie de services ou produits
+ Aller dans le module "Produits/Services"
+ Cliquer sur Tags/Catégorie (les catégories sont communes entre produits et services)
+ Cliquer sur Créer un nouveau Tags/Catégorie (en haut à droite de la page)
+ Remplir le champs "REF" avec le nom de catégorie souhaité
+ Choisir une couleur
+ Valider

## <a name="caisse"></a> MODULE DE CAISSE
**A utiliser pour les encaissements sans facture** (i.e un tiers générique est alors associé à chaque vente)

*Si besoin d'éditer une facture et pour tout client pro, il faut **impérativement** créer une facture [voir ici](#facture)*

+ Lancer le module depuis l'onglet caisse de Dolibarr
+ Choisir le ou les services/produits vendus
+ Modifier la quantité si besoin
+ Appliquer la remise si nécessaire
+ Valider

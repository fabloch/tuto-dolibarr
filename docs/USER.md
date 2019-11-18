# Manuel pour les utilisateurs

# SOMMAIRE
+ [Gestion des adhérents](#adherent) Adhésion et paiement cotisation
+ [Gestion des tiers](#tiers) *=client (adhérent ou non) qui achètent une prestations*
+ [Module de caisse](#caisse)
      *Pour les paiements des particulier. Facture non-nominative.*
+ [Créer une facture et enregistrer le paiement](#facture)
      *On fait une facture nominative pour les clients pro, assoc et entreprises*
+ [Imprimer/télécharger une facture](#imprFacture)
+ [Annuler une facture](#annulation) *réservé au manager*
+ [Exporter des adhérents](#export)
+ [Ajouter un service/produit](#serv-prod)
+ [Faire un devis](#devis)
+ [Entrer une note de frais](#frais)
+ A voir : gestion resssources; encaissement ; mailing

## Info importante
+ Toutes factures validées et toutes ventes enregistrées par la caisse ne peuvent pas être annulées (il faut faire une facture d'avoir).
+ Edition de facture impossible sans associer un tiers à un adhérent
+ Les champs en bleu sont à remplir obligatoirement.


## <a name="adherent"></a>GESTION DES ADHERENTS

### Comment ajouter un nouvel adhérent

1. **Se positionner dans le module Adhérents** (cliquer sur l'icone adhérents située en haut à gauche)
  + cliquer sur "*Nouvel adhérent*" dans la liste à gauche
  + Choisir le type d'adhérent : particulier, association, professionnel ou entreprise
  + Choisir la nature : physique ou moral
  + Entrer nom, prénom,  adresse, mail, téléphone
  + Cocher "oui" si mineur -18ans. Si oui, cocher oui si attestation parentale fournie
  + Cocher les différents choix pour réglement intérieur, autorisation image, attestation assurance et convocation AG...
  + Si besoin compléter les champs profession et ajouter des infos
  + Cliquer sur le bouton "*créer adhérent*" : la fiche est créée mais l'adhérent n'est pas encore validé (fiche à l'état de  
  brouillon)

2. **Valider le nouvel adhérent après l'avoir ajouté**
  + Après création  de l'adhérent, on arrive sur sa fiche au stade brouillon.
  + Cliquer sur le bouton "*Valider*" (confirmer par oui dans la boite de dialogue qui s'ouvre)

### Pour les assoc, pro ou entreprise : créer un tiers 
**Toujours** créer un tiers pour les associations, professionnel et entreprise afin de pouvoir éditer des factures.
+ Sur la fiche adhérent cliquer sur "*créer un tiers*"
+ Confirmer et valider

### <a name="cotisation"></a>Enregistrer le paiement de la cotisation (1ere adhésion ou renouvellement)
*A faire uniquement après avoir reçu l'intégralité du paiement.*
+ Aller sur la fiche de l'adhérent puis sur l'onglet Adhésions/Cotisations
+ cliquer sur "créer cotisation"
+ Choisir date de début d'adhésion
+ Pas besoin d'entrer la date de fin (automatiquement 1 an)
+ Entrer le montant de l'adhésion
+ Si besoin modifier le "libellé"
+ Action complémentaire, cocher soit : 
    + choisir "*aucun*" pour l'instant  
    + "*Création une écriture directe sur le compte bancaire ou caisse*" : pour une adhésion particulier sans facture ; va valider le paiement. Pas besoin de passer par le module caisse. Compléter les infos suivantes : 
        + Choisir compte Crédit Agricole
        + Choisir le mode de réglement
        + Indiquer la date du paiement
        + Si chèque compléter numero et banque et si virement indiquer le numero
    + "*Création facture sans paiement*" : pour une adhésion assoc, professionelle ou entreprise. Si besoin d'éditer une facture avant de recevoir le paiement (*valider avec un manager*). A réception du paiement il faudra valider la facture.
    + "*Créer une facture avec paiement sur compte bancaire ou caisse*" : pour une adhésion assoc, professionelle ou  entreprise, avec paiement reçu.  Va éditer et valider la facture (attention pas de brouillon, incrémente directement le numéro de facture non modifiable). Compléter les infos suivantes : 
        + Choisir compte Crédit Agricole
        + Choisir le mode de réglement
        + Indiquer la date du paiement
        + Si chèque compléter emetteur, banque et numéro et, si virement indiquer le numéro
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
+ Un tiers est un client/prospect ou un fournisseur. Il peut aussi être un adhérent. 
+ Pour pouvoir éditer une facture, il faut d'abord créer un tiers à partir d'un adhérent. On créer un tiers directement, sans le relié à un adhérent, uniquement pour les tiers non adhérent (ex: une assoc qui loue le herlomaton)

### Créer un tiers à partir de la fiche d'un adhérent
+ Aller sur la fiche de l'adhérent
+ Cliquer sur "créer un tiers" (bouton vert en bas de la fiche)
+ Renseigner/modifier si besoin le nom du tier
+ Valider le tiers

## <a name="caisse"></a> MODULE DE CAISSE
**A utiliser pour les encaissements sans facture nominative** (i.e un tiers particulier générique est alors associé à chaque vente) Possibilité d'éditer un ticket de caisse ou une facture non-nominative.
*Si besoin d'éditer une facture nominative et pour tout client pro, assoc, entreprise il faut **obligatoirement** créer une facture nominative [voir ici](#facture)*
+ Lancer le module TakePOS depuis l'onglet "PdV" de Dolibarr
+ S'identifier avec son login Dolibarr
+ Choisir le compte Crédit Agricole
+ Choisir le tier "Générique Caisse"
+ Choisir le ou les services/produits vendus (taper le préfixe dans le champ "recherche" pour resteindre les choix)
+ Modifier la quantité si besoin
+ Appliquer la remise si nécessaire
+ Cliquer sur "*ajouter cet article*"
+ Cliquer sur le "mode de réglement" adéquate (si espèce, entrer la somme reçu pour pouvoir valider)
+ Vérifier le résumer et indiquer en "*note*" : 
        + Pour un chèque : émetteur, banque et numéro
        + Hello assoc : numéro
+ Cliquer sur "*valider facture*"
+ Imprimer si besoin le ticket de caisse.

## <a name="facture"></a>CREER UNE FACTURE ET ENREGISTRER LE PAIEMENT

Il faut avoir [créer un tiers](#tiers) auparavant.
Il est possible d'enregistrer un paiement partiel. La facture passe du status "impayée" à "commencée".

### Pour une prestation (ou un produit)
+ Nota : il faut avoir créer le tiers préalablement (voir [ici](#tiers))
+ Aller dans le module "facturation/paiement" et choisir "nouvelle facture "
+ **Ou** Aller dans le module "tiers", aller sur la fiche du tiers, cliquer sur l'onglet "client" puis cliquer sur le bouton "créer une facture"
+ Choisir le nom du client (tiers)
+ Choisir la date de Facturation
+ Laisser condition réglement "A réception"
+ Cliquer sur "créer brouillon"
+ On accède à la fiche de la facture
+ Ajout nouvelle ligne : ajouter le type de prestation (choisir  dans le menu déroulant) et le montant. Indiquer quantité et remise si nécessaire puis valider en cliquant sur "ajouter". (on peut saisir un service/produit n'existant pas manuellement en indiquant le libellé, la quantité et le prix)
*Pour corriger un prix, il faut d'abord ajouter l'article.*
+ On peut alors cliquer sur "valider". 
+ Confimer la création. (ATTENTION : va alors créer un numéro de facture, on ne peut alors plus supprimer la facture ; pour l'annuler il faudra obligatoirement faire une facture d'avoir)
+ Enregistrer le paiement :
        + Cliquer sur "*Saisir réglement*"
        + Renseigner date et mode de réglement
        + Renseigner le "compte à créditer" ("**caisse**" pour une réglement en espèces sinon "**compte bancaire CA**" pour tous les autres modes de réglement.
        *(Il est possible d'enregistrer un paiement partiel, et d'enregistrer le solde plus tard. La facture passe du status "impayée" à "commencée".)*


### Pour une adhésion (si oublie au moment de la création de la cotisation)
+ Créer puis valider le membre si besoin, sinon aller sur sa fiche
+ Dans l'onglet Adhésion/Cotisation, cliquer sur "créer cotisation"
+ Renseigner date et montant d'adhésion
+ Au niveau du champs "Action complémentaire à l'enregistrement", sélectionner  "Créer une facture avec paiement sur compte bancaire ou caisse"
+ Cliquer sur "créer un tiers", un boite de dialogue apparait
+ Vérifier les infos puis valider
+ Renseigner le compte, le mode et la date du réglement
+ Cliquer sur "créer cotisation". [Voir ici](#cotisation)

## <a name="imprFacture"></a> IMPRIMER/TELECHARGER UNE FACTURE
+ Aller sur la fiche de la facture concernée
+ Scroller vers le bas
+ Dans l'encars "Fichier joint" : cliquer sur "*Générer*" (toujours le faire pour être sur d'avoir la dernière version)
+ Si besoin, cliquer sur la loupe pour visualiser la facture
+ Cliquer sur le numéro de facture pour la télécharger
+ Ouvrir le PDF sur l'ordi et l'imprimer
+ Ou joindre le pdf à un mail 

## <a name="annulation"></a>ANNULER UNE FACTURE
*A voir avec un manager*
+ Aller sur la fiche de la facture concernée *(ou bien sur la fiche du tiers concerné, aller dans l'onglet "client")*
+ Cliquer sur "*Créer Facture Avoir*"
+ Sous facture d'avoir, cocher la 1ère case "*Créer l'avoir avec les même lignes que la factures dont il est issu*"
+ Renseigner date, mode de réglement (du remboursement pas du paiement initial) et compte bancaire
+ En note, renseigner date et numéro du chèque ou virement
+ Cliquer sur "*créer brouillon*"
+ Vérifier puis valider la facture d'avoir.

**NE JAMAIS** classer une facture comme "**ABANDONNEE**" sauf pour "mauvais payeur" (A toujours valider avec la/le comptable)

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

## <a name="devis"></a>FAIRE UN DEVIS
+ Aller dans le module "Commercial
+ Choisir "nouvelle proposition"
+ remplir les champs puis Valider

## <a name="frais"></a>ENTRER UNE NOTE DE FRAIS
+ Aller dans le module GRH
+ Choisir Nouveau
+ Remplir les champs puis valider

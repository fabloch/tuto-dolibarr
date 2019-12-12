# Manuel pour les utilisateurs

# SOMMAIRE
+ [Gestion des adhérents](#adherent) Création et validation de l'adhésion
+ [Module de caisse](#caisse)
      *Pour l'encaissement des paiements des particulier. Facture non-nominative. Y compris l'encaissement des cotisations 
      particuliers*
+ [Cloturer la caisse](#cloture)
+ [Créer une facture et enregistrer le paiement](#facture)
      *On fait une facture nominative pour les clients pro, assoc et entreprises, y compris l'encaissement des cotisations 
      pro/assoc/entr**
+ [Imprimer/télécharger une facture](#imprFacture)
+ [Annuler une facture](#annulation) *réservé au manager*
+ [Gestion des tiers](#tiers) *=client. Relier un adhérent à un tiers pour pouvoir éditer une facture*
+ [Exporter des adhérents](#export)
+ [Ajouter un service/produit](#serv-prod)
+ [Faire un devis](#devis)
+ [Entrer une note de frais](#frais)
+ A voir : gestion resssources; encaissement ; mailing

## Info importante
+ Toutes factures validées et toutes ventes enregistrées par la caisse ne peuvent pas être annulées (il faut faire une facture d'avoir).
+ A chaque vente/facture validée doit correspondre un paiement du montant exact de la vente/facture.
       
       exemple : _ je fais une vente de 20€. je reçois un chèque de 20€ : c'est OK
                 _ je fais une vente de 20€.je reçois 10€ en espèce et un chèque 10€  : c'est OK
                 _ je fais deux ventes de 20€ au même client et je reçois un chèque global de 40€.
                   C'est pas bon. Je dois regrouper les deux ventes (=faire une seule vente, 
                   faire une seule facture) 
+ Edition de facture impossible sans associer un tiers à un adhérent
+ Les champs en bleu sont à remplir obligatoirement.


## <a name="adherent"></a>GESTION DES ADHERENTS

### Comment ajouter un nouvel adhérent et enregistrer le paiement de la cotisation (pour un renouvellement passer à l'étape 4)
*A faire uniquement après avoir reçu l'intégralité du paiement.*

1. **Se positionner dans le module Adhérents** (cliquer sur l'icone adhérents située en haut à gauche)
  + cliquer sur "*Nouvel adhérent*" dans la liste à gauche
  + Choisir le type d'adhérent : particulier, association, professionnel ou entreprise
  + Choisir la nature : physique ou moral
  + Entrer nom, prénom,  adresse, mail, téléphone
  + Cocher "oui" si mineur -18ans. Si oui, cocher "oui" si attestation parentale fournie
  + Cocher les différents choix pour réglement intérieur, autorisation image, attestation assurance et convocation AG...
  + Si besoin compléter les champs profession et ajouter des infos
  + Cliquer sur le bouton "*créer adhérent*" : la fiche est créée mais l'adhérent n'est pas encore validé (fiche à l'état de  
  brouillon)

2. **Valider le nouvel adhérent après l'avoir ajouté**
  + Après création  de l'adhérent, on arrive sur sa fiche au stade brouillon.
  + Cliquer sur le bouton "*Valider*" (confirmer par oui dans la boite de dialogue qui s'ouvre)

3. **Créer un tiers**
+ Sur la fiche de l'adhérent cliquer sur "*créer un tiers*"
+ Confirmer et valider

4. **Valider la cotisation**  (nouvelle adhésion ou renouvellement)

     **A faire uniquement après avoir reçu l'intégralité du paiement.**
+ Aller sur la fiche de l'adhérent puis sur l'onglet Adhésions/Cotisations
+ cliquer sur "créer cotisation"
+ Choisir date de début d'adhésion (par défaut pour un renouvellement c'est le lendemain de la date de fin d'adhésion)
+ Pas besoin d'entrer la date de fin (automatiquement 1 an)
+ Entrer le montant de l'adhésion
+ Si besoin modifier le "libellé"
+ "Action complémentaire" : laisser sélectionné le choix  " *Aucun* "
+ Cliquer sur "*créer cotisation*"

5. <a name="cotisation2"></a>**Enregistrer le paiement de la cotisation**  (nouvelle adhésion ou renouvellement)

  + Pour les particuliers, aller dans la caise "Pdv" et choisir choisir le nombre de "cotisations particuliers" vendues.
    Si le client achète en même temps un ou des produits, par exemple un pack 3D, l'ajouter à la vente. 
     
  + Pour les professionelles, associations et entreprises, il faut passer par le module facture. Créer une facture et ajouter 
  le type de cotisations vendues (pro/assoc ou entreprise). Ajouter si besoin des produits complémentaires. Valider la facture    
  puis enregistrer le paiement (se reporter à comment faire une facture) 
          + *attention : Choisir compte "Caisse liquide" pour un paiement en liquide, sinon choisir "Crédit agricole"*

+Compléter les infos suivantes : 
        + Choisir compte "Caisse liquide" pour un paiement en liquide, sinon choisir "Crédit agricole"
        + Choisir le mode de réglement
        + Indiquer la date du paiement
        + (option à voir avec Manager) Si chèque compléter émetteur, banque et numéro et, si virement indiquer le numéro 
        + Valider en cliquant sur "créer cotisation"
  
 
### Comment rechercher un adhérent puis accéder/modifier fiche
+ Se placer dans le module adhérent
+ Dans la colonne de gauche choisir "liste" pour voir tous les adhérents ou bien choisir selon les attributs proposés (à jour...)
+ On peut trier les adhérents suivants les attributs proposés (nom, prenom, etc.) ou directement entrer un nom, un prenom... dans les cases situé au desssus du nom des atrributs. Puis cliquer sur la loupe pour valider le tri.
+ Cliquer sur le numéro de  "Réf." pour accéder à une fiche

### Comment résilier un Adhérent
+ Aller sur la fiche de l'adhérent
+ Cliquer sur résilier (puis valider par oui).

## <a name="caisse"></a> MODULE DE CAISSE (TakePOS) A utiliser avec l'ordinateur de caisse uniquemement

**A utiliser pour les encaissements sans facture nominative** (i.e un tiers particulier générique est alors associé à chaque vente) Possibilité d'éditer un ticket de caisse ou une facture non-nominative.

*Si besoin d'éditer une facture nominative et pour tout client pro, assoc, entreprise il faut **obligatoirement** créer une facture nominative [voir ici](#facture)*

**Ne pas modifier le client : les ventes par la caisse doit toujours être effectuée par le tiers "Client générique caisse"**


+ Lancer le module TakePOS depuis l'onglet " PdV " de Dolibarr
+ Choisir la catégorie du produit/service 
+ Choisir le produit/service vendu. Si pas dans la liste cliquer sur "Produit/Service non prédéfini" ert entrer un libellé et le prix
+ Modifier la quantité si besoin (cliquer sur "Qté" sur la calculette ; modifier et cliquer sur OK (le bouton "Qté" devient "Ok")
+ Appliquer la remise en % si nécessaire (meme principe que pour les quantités)
+ Cliquer " Réglement " 
+ Entrer la somme reçu
+ Cliquer sur le moyen de paiement reçu. **Attention** cet action (= ce click) **va valider définitivement la vente**, elle ne pourra plus être annulée (sauf par un manager)
+ Vérifier que la vente est bien marquée " Payé " (en vert  en haut à gauche sur l'ecran)
+ Impimer le ticket de caisse si besoin
+ Passer à la vente suivant en recommançant ce déroulé à partir de choisir la catégorie de produit/service (pas besoin de cliquer sur le bouton "nouveau").

Si plusieurs moyens de paiment (ex : 10 € espèce + 10€ chèq pour une vente de 20€) sont utilisé pour régler une même vente,  alors il faut saisir plusieurs réglement (ie : on clic sur "Réglement", on indique le montant reçu en espèce puis on clique sur espèce. Il reste donc 10€ à régler. A nouveau on clic sur "Réglement", on indique le montant reçu en chèquepuis on clique sur "chèque")

* Remarque : 
          + Le bouton "nouveau" sert si on veut annuler notre saisi (non validée) d'une vente et repartir d'un écran vierge"


## <a name="cloture"></a> CLOTURER LA CAISSE (en développement)
A faire chaque fin de journée 
+ Aller dans l'onglet "Banque/Caisse" 
+ Puis (sur la gauche) dans POS, choisir "Nouvelle cloture de caisse"
+ Choisir la date
+ Entrer les montants comptablilisés dans la caisse.
+ Vérifier le brouillon
+ Cliquer sur " Enregister et valider " 
+ Imprimer le ticket récapitulatif

## <a name="facture"></a>CREER UNE FACTURE ET ENREGISTRER LE PAIEMENT

Il faut avoir [créer un tiers](#tiers) auparavant.

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
     + Renseigner le "compte à créditer" ("**caisse**" pour une réglement en espèces sinon "**Crédit Agricole**" pour tous 
     les autres modes de réglement)
     + Indiquer la date du paiement
     + Option : si chèque compléter emetteur, banque et numéro et, si virement indiquer le numéro
     + Saisir le montant reçu (si plusieurs factures en attente, vérifier la concordance entre le paiement reçu)
     + Cliquer sur " Payer " (*laisser cocher la case au-dessus*)
     + Confimer en validant


        
Si plusieurs moyens de paiment (ex : 10 € espèce + 10€ chèq pour un facture de 20€) sont utilisé pour régler une même facture,  alors il faut saisir plusieurs réglement (ie : on clic sur "saisir un réglement", on indique le 1er mode de paiement, espèce et le montant 10€ puis on valide. Ensuite retour à la fiche de la facture, à nouveau on clic sur "saisir un réglement", on indique le 2er mode de paiement, le montant et on valide) 

Il est possible d'enregistrer un paiement partiel. La facture passe alors du status "impayée" à "commencée".


## <a name="imprFacture"></a> IMPRIMER/TELECHARGER UNE FACTURE
+ Aller sur la fiche de la facture concernée (ou on peut y accéder par la fiche du tiers)
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
+ Vérifier puis valider la facture d'avoir
+ Si il y a eu un paiement il faut procéder au remboursement : 
             + Cliquer sur "*Saisir Remboursement*"
             + Saisir la date et le mode réglement

**NE JAMAIS** classer une facture comme "**ABANDONNEE**" sauf pour "mauvais payeur" (A toujours valider avec la/le comptable)


## <a name="tiers"></a>GESTION DES TIERS
+ Un tiers est un client/prospect ou un fournisseur. Il peut aussi être un adhérent. 
+ Pour pouvoir éditer une facture, il faut d'abord créer un tiers à partir d'un adhérent. On créer un tiers directement, sans le relié à un adhérent, uniquement pour les tiers non adhérent (ex: une assoc qui loue le herlomaton)

### Créer un tiers à partir de la fiche d'un adhérent
+ Aller sur la fiche de l'adhérent
+ Cliquer sur "créer un tiers" (bouton vert en bas de la fiche)
+ Renseigner/modifier si besoin le nom du tier
+ Valider le tiers

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
+ Ajouter dans : "Vente caisse" (important si on veut que la catégorie apparaisse dans la caisse TakePos)
+ Valider

## <a name="devis"></a>FAIRE UN DEVIS
+ Aller dans le module "Commercial
+ Choisir "nouvelle proposition"
+ remplir les champs puis Valider

## <a name="frais"></a>ENTRER UNE NOTE DE FRAIS
+ Aller dans le module GRH
+ Choisir Nouveau
+ Remplir les champs puis valider

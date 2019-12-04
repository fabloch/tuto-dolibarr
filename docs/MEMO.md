# MEMO

###Caisse Pdv pour l'encaissement des particuliers (pas de facture nominative)

- Ajouter les produits vendus
- saisir le réglement (si plusieurs moyens de paiement, saisir plusieurs réglements du montant correspondant à chaque moyen de paiement).
- A l'appui sur le bouton "espèces" ou chèque", le paiement est définitif (on ne peut plus revenir en arrière)
- Vérifier que l'état de la vente est passé à payé (en vert)
- Si besoin imprimer le ticket de caisse

###Module facture pour l'encaissement des pro/assoc et entreprise (facture nominative)

- Créer une facture au nom du client (= du tiers)
- Ajouter les produits
- Vérifier la facture avec le client avant de valider
- Valider
- Saisir puis valider le réglement.
- Générer la facture. l'enregistrer dans le NAS sous
  /ORGABISATION/compta/compta 2020/factures éditée dolibarr
- Imprimer ou Envoyer la facture par mail (google) au client.

(si plusieurs moyens de paiement sont utilisé, saisir un 1er réglement du montant correspondant au 1er moyen de paiement, puis recommencer avec le 2ème)

### Enregistrement des cotisations (2 étapes)

1. Valider la cotisation

- Créer un nouveau membre si il n'existe pas et le valider. Si c'est un renouvellement aller sur la fiche de l'adhérent
- Sur la fiche adhérent, aller dans l'onglet Adhésion/Cotisation et cliquer sur "créer cotisation"
- Indiquer le montant
- Laisser "aucun" coché
- Cliquer sur "créer cotisation"

2. Enregistrer le paiement

- Pour les particuliers, utiliser le module de caisse Pdv en choississant le produit "cotisation particulier"
- Pour les pro/assoc et entreprise, établisser une facture nominative avec le produit "cotisation pro/assoc" ou "cotisation entreprise"

R: il est possible d'enregistrer sur la même vente ou facture, le paiement de plusieurs cotis ou de cotisation(s)+produit(s), dans le cas ou il y a un seul paiment.

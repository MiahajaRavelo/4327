
## 0.1 Lancer l’application


- [x] <http://localhost:8080/api/plats> affiche du JSON ;
- [x] <http://localhost:5173> affiche l’ardoise avec les plats ;
- [x] vous avez passé une commande depuis l’onglet **Prendre une commande** et la retrouvez dans l’onglet **Commandes**.

## 0.2 Lire le schéma relationnel

Ouvrez `database/01_schema.sql`.

1. 
   * `categorie`(**id**,libelle)
   * `plat`(**id**,nom,prix,#id_categorie)
   * `commande`(**id**, date_commande,numero_table)
   * `commande_ligne`(**id**,#id_commande,#id_plat,quantite,prix_unitaire)
2. 
     car on le client peuvent avoir plusieurs commande c'est a dire que une la commande du client peuvent se multiplier  

3. 
   les lignes de commande qui appartient aux commande sont aussi supprimer avec lui
   
4. Repérez **trois données absurdes** :
   * si 2 client different peuvent reserver le meme table, le restaurant ont beaucoup de table
   * Prix peuvent etre negative
   * Les commandes sont envoye a la cuisine sans qu'on sache **qui** les a envoye les commande

## 0.3 Interroger l’API à la main

5. a\. 201
5. b\. C'est pas de car 200 -> success ok & 201 -> success ok creer
6. a\. qui bloque la suppression : php
 

## Validation du niveau 0

- [x] L’application tourne (API + interface).
- [ ] `reponses-niveau-0.md` répond aux 11 questions et contient le tableau 0.4 complet.
- [ ] Le nom de la gargote est modifié ; *Goûter* existe en base.
- [ ] Un commit `niveau 0 : prise en main`.

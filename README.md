# dlt-blockchain-intro

1-  Un arbre de merkle nécessite une paire de hashes pour produire un nouveau hash parent. 
    Il faut donc a absolument que le nombre de transactions qui produiront le Merkle root soit pair.
    Comment est géré le cas ou le nombre de transactions dans le Block à valider est impair pour générer un Merlke root ?


      Dans le cas où le nombre d'empreintes à combiner est impair,   
      on combine la dernière empreinte avec elle-même.   
      ont dois la concatener avec elle meme pour calculer..


2-  Dans le réseau bitcoin, Comment un nouveau noeud arrive t'il à retrouver ses pairs et ainsi rejoindre le réseau ?  
    Expliquer le processus avec vos propres mots.

      je pense qu il retrouve ses pairs grace au logiciel   
      bitcoinCore qui est un protocole en p2p.
      


3- Pouvez vous nommer au moins une personne qui a ou aurait pu influencer directement ou indirectement la création de Bitcoin par ses travaux 
    (une personne qui n'a pas été nommée dans le cours)?

      W. Feller, "An introduction to probability theory and its applications," 1957
      Hal Finney 1er envoi de btc avec Satoshi Nakamoto
      Bitcoin est une amélioration du concept de b-money, imaginé par Wei Dai en 1999


4- Avec vos propres recherches et grâce aux compétences acquises en cours pouvez vous expliquer 
   comment une Blockchain crée un lien entre ses différents Blocks?
   
      le bloc deja validé emet un hash et le premier qui trouve ce hash   
      pour le bloc suivant est authorisé a ajouter le bloc a la blockchain.



5- Quelle structure de données informatique peut représenter le mieux cette chaine de Block: 
   https://en.wikipedia.org/wiki/List_of_data_structures ?


     Structures à base de hachage Merkle tree



6- Si je souhaite modifier une transaction de 10 bitcoin que j'ai effectué il y a 6 mois en une transaction de 1 Bitcoin, 
   que dois je modifier dans la Blockchain et que dois je mettre en oeuvre pour que cette modification persiste ?
   Est ce possible selon vous ?

    deja il vaudrait mieux modifier a la hausse et non a la baisse.
    il faudrait modifier les données de la transaction hashé stocké   
    du merkle root dans le bloc header, et ensuite modifier   
    tout les headers des blocks suivants deja validé et ,
    de nouveau refaire une preuve de travaille pour chaque bloc..
    tout ca en tenant compte que chaque 10min de nouveu bloc continu de s ajouté.
    bah si ont arrive a pirater quasiment tous les ordinateurs du reseaux distribué   
    en meme temps et avec la puissance de tous les ordinateurs connectés du monde   
    (et les ordinateurs quantique aussi pour le coup)
    ca devrait etre possible imaginairement parlant bien sur...
    Donc non absolument pas realisable actuellement..


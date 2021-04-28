# dlt-blockchain-intro

1-Un arbre de merkle nécessite une paire de hashes pour produire un nouveau hash parent. 
  Il faut donc a absolument que le nombre de transactions qui produiront le Merkle root soit pair.
  Comment est géré le cas ou le nombre de transactions dans le Block à valider est impair pour générer un Merlke root ?


  Dans le cas où le nombre d'empreintes à combiner est impair, on combine la dernière empreinte avec elle-même. 
  ont dois la concatener avec elle meme pour calculer..


2-Dans le réseau bitcoin, Comment un nouveau noeud arrive t'il à retrouver ses pairs et ainsi rejoindre le réseau ?  
  Expliquer le processus avec vos propres mots.

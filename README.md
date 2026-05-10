# Bose

Si comme moi vous avez une enceinte Bose SoundTouch, vous avez été surppris que votre enceinte ne fonctionnait plus.
Apres quelques heures de recherche j'apprends que les touches numérique ne fonctionnaient plus et pourquoi car Bose a décidé d'arréter son service "cloud". 
Bose a en effet annoncé la fin du support pour le 6 mai 2026.
Ca veut dire que votre enceinte va se transformer en brique connectée qui ne se connecte plus à grand chose.

🔧 Comment ça fonctionne techniquement
Chaque enceinte SoundTouch embarque à l'intérieur un serveur web local qui écoute sur :

Le port 8090 : pour les commandes REST (volume, lecture, etc.)

Le port 8080 : pour les notifications en temps réel (WebSocket) 

Le protocole s'appelle "gabbo" et il est complètement documenté par Bose . Avec l'API locale, vous pouvez :

Contrôler le volume

Lire des flux audio (radios internet, musique depuis votre NAS)

Gérer la lecture (play/pause/next/prev)

Créer des zones multiroom

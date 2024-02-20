# TCP-Multi-Threading-
# Serveur TCP Multi-Threaded en Java

Ce projet contient un serveur TCP en Java capable de traiter jusqu'à 10 clients en parallèle. Chaque client envoie une chaîne de caractères au serveur, qui la renvoie inversée après un délai simulé.
  - Le serveur peut gérer jusqu'à 10 clients en parallèle.
   - Chaque client est traité dans un thread séparé, permettant au serveur de continuer à accepter de nouvelles connexions pendant le traitement.

## Démarche

1. **Initialisation :**

   - Le serveur écoute sur le port 8888.
   - Un nouveau thread est créé pour chaque client accepté.

2. **Traitement du client :**

   - Le client envoie une chaîne de caractères au serveur.
   - Le serveur inverse la chaîne de caractères.
   - Un délai de traitement simulé de 2 secondes est ajouté avec `Thread.sleep`.
   - La chaîne inversée est renvoyée au client.

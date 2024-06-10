# Accident Prevention through Real-time Visual and Auditory Artificial Intelligence
Ce projet se concentre sur le développement d'un système de prévention des collisions en temps réel, en exploitant des technologies de pointe en programmation et en traitement de données. Python est le langage principal en raison de sa clarté, de son vaste support de bibliothèque et de sa robustesse dans le traitement des données et des tâches d'apprentissage automatique.

Pour permettre une prévention des collisions robuste, le système exploite la puissance de TensorFlow, PyTorch et OpenCV. Ces frameworks jouent des rôles vitaux dans la modélisation et le déploiement d'algorithmes d'apprentissage en profondeur, cruciaux pour l'analyse prédictive et la prévention des collisions. TensorFlow et PyTorch offrent des fonctionnalités avancées qui permettent au système d'identifier et de prédire avec précision les comportements des objets dans des environnements complexes. Pendant ce temps, OpenCV facilite le traitement en temps réel des données visuelles, permettant une analyse dynamique et une réaction aux entrées visuelles, ce qui est fondamental pour la prédiction et la prévention des collisions.

L'intégration de différents modèles améliore encore les capacités du système. Par exemple, le modèle "[Depth Anything](https://github.com/LiheYoung/Depth-Anything)", conçu pour estimer la profondeur à partir d'images monoculaires, utilise des techniques avancées d'apprentissage automatique. En interprétant et en transformant les images 2D en cartes de profondeur détaillées, ce modèle fournit des informations spatiales essentielles nécessaires pour prédire avec précision les collisions.

![Depth Anything Model Architecture](/images/depth1.png "Depth Anything Model Architecture")

![Depth Anything Example](/images/Image1.png "Depth Anything Example")

En plus de l'estimation de la profondeur, le système utilise (YOLOv8)[https://docs.ultralytics.com/tasks/pose//] pour la détection rapide et précise des poses humaines. Cette capacité est particulièrement cruciale pour la prévention des collisions en temps réel, surtout dans les scénarios où la présence humaine influence considérablement les risques de collision.

![Image avec détection d'objet YOLOv8](/images/Image4.png "Image avec détection d'objet YOLOv8")

Pour améliorer l'évaluation des risques de collision, le projet introduit une nouvelle méthodologie utilisant une segmentation perspective trapézoïdale. Cette segmentation divise l'espace visuel en trois zones distinctes en fonction de la distance des objets, améliorant ainsi la capacité du système à évaluer les niveaux de risque de collision et à prendre des mesures préventives en conséquence.

![Exemple du trapèze appliqué à Depth Anything.](/images/Image2.png "Exemple du trapèze appliqué à Depth Anything")

Le traitement en temps réel est réalisé grâce à des algorithmes optimisés et à du matériel performant. Cela garantit une analyse et une réponse instantanées des données, permettant au système de suivre un flux de traitement rationalisé, de la capture vidéo à la détection des collisions en passant par la génération d'alertes, facilitant ainsi une prise de décision rapide et efficace.

![YOLO et Trapèze](/images/Image3.png "Exemple du trapèze et YOLO appliqyé à une image")

Dans l'ensemble, l'intégration et la réalisation de ce projet représentent une avancée significative dans la technologie de prévention des collisions. Avec des applications allant des véhicules autonomes aux systèmes de sécurité industrielle, le système vise à améliorer la sécurité et l'efficacité dans des environnements dynamiques en exploitant des technologies de pointe et des méthodologies innovantes.

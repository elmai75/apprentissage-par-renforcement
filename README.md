# reinforcement learning_ELMAI

L'apprentissage par renforcement est une méthode d'apprentissage automatique où un agent apprend à prendre des décisions dans un environnement en interagissant avec celui-ci. L'agent reçoit des récompenses ou des pénalités en fonction des actions qu'il prend, ce qui lui permet d'ajuster son comportement pour maximiser les récompenses.

L'apprentissage par renforcement est une branche de l'apprentissage automatique qui s'inspire de la psychologie comportementale. Dans ce type d'apprentissage, un agent est placé dans un environnement et est chargé d'accomplir une tâche spécifique. L'agent interagit avec l'environnement en effectuant des actions, qui peuvent avoir un effet sur l'état de l'environnement. L'agent reçoit ensuite une récompense ou une pénalité en fonction des actions qu'il a prises.

L'objectif de l'agent est d'apprendre à prendre les actions qui maximisent les récompenses qu'il reçoit. Pour cela, il doit explorer différentes stratégies et apprendre à évaluer les récompenses qu'il reçoit en fonction des actions qu'il a prises. Les algorithmes d'apprentissage par renforcement sont conçus pour permettre à l'agent de généraliser à partir des expériences passées et de prendre des décisions optimales dans des situations inconnues.

L'apprentissage par renforcement est utilisé dans de nombreuses applications, telles que la robotique, les jeux vidéo, la publicité en ligne, la gestion des ressources naturelles, la finance, la santé, etc. Les algorithmes les plus couramment utilisés dans l'apprentissage par renforcement comprennent la méthode de Monte-Carlo, la Q-learning, la SARSA, les réseaux de neurones profonds, etc.

Ce Tp est décomposé de 3 parties:

# l'environement Cartpole-v1
 Les tâches de cette partie sont :

- Configuration de  l'environnement CartPole
-  Configuration de l'agent en tant que réseau de neurones simple avec :
  - Une couche entièrement connectée avec 128 unités et une activation ReLU suivie d'une couche de désactivation
  - Une couche entièrement connectée suivie d'une activation softmax
- Répéter 500 fois :
- Réinitialiser l'environnement
- Réinitialiser le tampon
- Répéter jusqu'à la fin de l'épisode :
- Calculer les probabilités d'action
- Échantillonner l'action en fonction des probabilités et stocker sa probabilité dans le tampon
- Faire avancer l'environnement avec l'action
- Calculer et stocker dans le tampon le retour en utilisant gamma=0,99
- Normaliser le retour
- Calculer la perte de politique comme -somme(log(prob) * retour)
- Mettre à jour la politique en utilisant un optimiseur Adam et un taux d'apprentissage de 5e-3

ce modèle est partagé dans la plateforme Hugging facing Hub, dans le lien suivant: https://huggingface.co/Mohamed10/TP1_RL_ELMAI/tree/main


# a2c_sb3_cartpole
Dans cette partie, on va utiliser le package Stable-Baselines3 pour entraîner un bras robotique à l'aide du RL. plusieurs outils largement utilisés pour l'entraînement, la surveillance et le partage de modèles d'apprentissage automatique.

On va utiliser A2c

ce modèle est partagé dans la plateforme Hugging facing Hub, dans le lien suivant: https://huggingface.co/Mohamed10/TP1_RL_ELMAI/tree/main

# a2c_sb3_panda_reach
 Dans cette partie on va utiliser le package Stable-Baselines3 pour entraîner un modèle A2C sur l'environnement PandaReachJointsDense-v2. 500 000 étapes devraient suffire.En suivant  l'environnement avec Weights & Biases.

 le track et la comparaison des expériences est dans le lien suivante: https://wandb.ai/elmaimohamed638/panda-reach-a2c?workspace=user-elmaimohamed638
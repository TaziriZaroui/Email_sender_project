# Email_sender_project
# *Cahier des Charges – Projet Email Sender*

## 1. Contexte et Objectifs

**Contexte :**  
Le projet vise à développer une application web permettant l’envoi d’emails depuis une interface simple et ergonomique. L’objectif est de faciliter la communication par email directement depuis une plateforme web, en garantissant sécurité et fiabilité.

**Objectifs principaux :**  
- Permettre à l’utilisateur d’envoyer des emails à un ou plusieurs destinataires.  
- Assurer la validité et la sécurité des données saisies.  
- Fournir un retour clair sur l’état de l’envoi (succès ou erreur).  
- Créer une interface moderne, ergonomique et responsive.

---

## 2. Périmètre Fonctionnel

| Fonctionnalité              | Description                                      | Priorité |
|------------------------------|------------------------------------------------|----------|
| Saisie de l’email du destinataire | Champ texte avec validation de l’email       | Haute    |
| Saisie du sujet              | Champ texte pour le sujet de l’email           | Haute    |
| Saisie du message            | Zone de texte pour rédiger le corps de l’email | Haute    |
| Bouton d’envoi               | Envoi du message via backend                   | Haute    |
| Feedback utilisateur         | Affichage d’un message “Email envoyé” ou d’erreur | Haute |
| Support des pièces jointes   | Possibilité d’ajouter un fichier               | Moyenne  |
| Responsive Design            | Accessible sur mobile et desktop              | Haute    |
| Sécurité                     | Validation côté client et serveur, protection SMTP | Haute |

---

## 3. Périmètre Technique

**Frontend :**  
- HTML5 pour la structure  
- CSS3 ou Bootstrap pour le style  
- JavaScript pour interactions et validation côté client  
- AJAX (`fetch`) pour communiquer avec le backend

**Backend :**  
- Python + Flask pour le serveur  
- SMTP (Gmail ou autre) pour l’envoi d’emails  
- Gestion des erreurs et retours JSON

**Architecture :**  
Frontend (HTML/CSS/JS)
|
|--- AJAX/Fetch --->
|
Backend (Flask/Python + SMTP)
|
|--- SMTP Server (Gmail, Outlook...) --->
|
Destinataire Email


# rapport-d-analyse-de-sécurité-d-un-site-web
 🔒 Dippu-Tech Inc. – Rapport d’Analyse de Sécurité  
**Projet : Modernisation d’un site web d’entreprise vers une plateforme e-commerce**  
**Auteur : Dippu Claude Cyrille – Analyste en Cybersécurité**  
**Date : 25 novembre – 02 décembre 2024**  
**Classification : CONFIDENTIEL**  

 ### Contexte du projet
L’entreprise **Dippu-Tech Inc.** a initié la refonte de son site vitrine en une **plateforme e-commerce** intégrant :  
- Gestion des commandes et paiements en ligne  
- Gestion des profils clients incluant données personnelles et financières sensibles  
- Intégration des données dans une infrastructure **infonuagique SharePoint**  

Cette transformation représente une opportunité stratégique, mais expose également l’organisation à des **risques de sécurité majeurs** liés à la confidentialité, l’intégrité et la disponibilité des données.

---

### Objectifs de l’analyse
- Évaluer les risques de sécurité liés à la modernisation du site web  
- Identifier les vulnérabilités critiques dans l’architecture et les processus  
- Fournir des recommandations concrètes à court, moyen et long terme  

---

### Portée (scope)
✅ Données sensibles clients (PII, informations financières)  
✅ Architecture technique et gestion des accès  
✅ Sécurité des transactions et conformité (ex : PCI-DSS)  
✅ Protection contre les cybermenaces  
✅ Conformité réglementaire  

Hors portée : aspects esthétiques, ergonomie, infrastructure physique interne.  

---

 ### Résultats de l’analyse
Estimation du niveau de risque global : ÉLEVÉ**  

### Principales anomalies identifiées
1. Données sensibles stockées **sans chiffrement**  
2. Transactions en ligne non conformes aux standards **PCI-DSS**  
3. Site web basé sur une technologie **obsolète**, absence de HTTPS obligatoire  
4. Absence de **sauvegarde et plan de reprise** en cas de sinistre  
5. Pas de **gestion centralisée des journaux d’audit** dans SharePoint  
6. Gestion des permissions d’accès insuffisante (**risque d’abus interne**)  
7. Absence de **tests de pénétration** (niveau de risque : Moyen)  

---

 ### Recommandations

Court terme (immédiat)
- Implémentation du **chiffrement AES-256** des données sensibles  
- Sécurisation des paiements (chiffrement en transit + MFA)  
- Forcer l’utilisation de **HTTPS** sur toutes les connexions  
- Mise en place de **sauvegardes automatiques** sécurisées  
- Réduction des permissions selon le **principe du moindre privilège**  
- Conformité avec **PCI-DSS**  
- MFA pour tous les comptes administratifs  

### Moyen terme (3 mois)
- Déploiement d’une solution **IAM (Identity & Access Management)**  
- Élaboration d’un **Plan de Continuité des Activités (PCA)** et **Plan de Reprise après Sinistre (PRS)**  
- Mise à jour régulière des systèmes et composants  

### Long terme (6 mois)
- Audits de sécurité récurrents  
- Mise en place d’une **surveillance comportementale automatisée (IA)**  
- Automatisation de la gestion des permissions utilisateurs  
- Réalisation régulière de **tests de pénétration**  

### Compétences démontrées
- Analyse de risque et évaluation des menaces  
- Gestion de la sécurité des données sensibles (PII, informations financières)  
- Mise en conformité avec des standards de sécurité (**PCI-DSS**)  
- Élaboration de recommandations stratégiques et techniques  
- Connaissance de la sécurité infonuagique (**SharePoint**)  
- Définition de plans **PCA/PRS** et mise en place d’**IAM**  
- Implémentation de bonnes pratiques en **chiffrement (AES-256, HTTPS, MFA)**  


 🛠️ Technologies & Normes de sécurité
- **Chiffrement :** AES-256, TLS/HTTPS  
- **Conformité :** PCI-DSS  
- **Gestion des accès :** IAM, MFA, principe du moindre privilège  
- **Infonuagique :** Microsoft SharePoint  
- **Surveillance :** Journaux d’audit centralisés, détection comportementale  


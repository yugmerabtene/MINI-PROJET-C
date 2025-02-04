### 📌 Énoncé : Distributeur Automatique de Billets (DAB) en C  

Vous devez développer une application en ligne de commande en langage C qui simule le fonctionnement d'un distributeur automatique de billets (DAB). L’application devra permettre à un utilisateur de :  

- Insérer une carte (via un numéro de carte simulé).  
- Saisir un code PIN.  
- Consulter le solde de son compte.  
- Retirer une somme d’argent (en respectant le solde disponible et un plafond de retrait).  
- Quitter l’application en toute sécurité.  

L'application fonctionnera sans base de données, en utilisant uniquement des structures et des fichiers pour stocker les informations des utilisateurs.  

---

### 🔥 User Stories  

#### 🏦 **Authentification**  
**En tant qu’utilisateur**, je veux insérer ma carte via un numéro de carte unique et entrer mon code PIN, afin d’accéder à mon compte en toute sécurité.  

**Critères d’acceptation :**  
- L’application demande un numéro de carte et un code PIN.  
- Si les informations sont incorrectes après 3 tentatives, le compte est bloqué.  

---

#### 💰 **Consultation du Solde**  
**En tant qu’utilisateur**, je veux pouvoir consulter le solde de mon compte, afin de savoir combien d’argent est disponible.  

**Critères d’acceptation :**  
- L’application affiche mon solde après authentification.  

---

#### 💸 **Retrait d’Argent**  
**En tant qu’utilisateur**, je veux pouvoir retirer de l’argent, afin d’utiliser mes fonds.  

**Critères d’acceptation :**  
- L’utilisateur peut choisir un montant à retirer.  
- Le retrait ne doit pas dépasser le solde disponible.  
- Il y a un plafond de retrait fixé (ex. : 500€ par jour).  
- Après le retrait, le solde est mis à jour.  

---

#### 🔐 **Déconnexion**  
**En tant qu’utilisateur**, je veux pouvoir quitter l’application en toute sécurité, afin de protéger mon compte.  

**Critères d’acceptation :**  
- Une option permet de quitter le programme proprement.  
- Toutes les données sont sauvegardées correctement avant la fermeture.  

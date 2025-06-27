# Ansible Role: quiz

Ce rôle Ansible permet de déployer automatiquement l'application Node.js **quiz-ansible** sur un système Linux basé sur **Debian/Ubuntu** ou **RedHat/Rocky Linux**.

## 📦 Fonctionnalités

- Mise à jour des paquets système
- Installation de Git et Node.js
- Clonage du dépôt GitHub contenant l'application
- Installation des dépendances via `npm`
- Build de l'application
- Lancement du serveur local avec `serve`

## 🔧 Compatibilité

| Distribution | Supportée |
|--------------|------------|
| Debian       | ✅         |
| Ubuntu       | ✅         |
| Rocky Linux  | ✅         |
| RedHat       | ✅         |

## 📁 Structure du rôle

roles/
└── quiz/
├── defaults/
│ └── main.yml
├── tasks/
│ └── main.yml
├── meta/
│ └── main.yml
└── README.md


## 🛠️ Variables par défaut

Aucune variable personnalisable pour l’instant.

## 🚀 Utilisation

Dans un playbook Ansible :

```yaml
- name: Déployer l'application quiz-ansible
  hosts: all
  become: yes
  roles:
    - ymed95.quiz

Installation depuis Ansible Galaxy
ansible-galaxy install ymed95.quiz

Références
https://github.com/franklin-tutorials/quiz-ansible.git

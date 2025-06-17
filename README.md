# install-sidestore-on-linux
# 🐧 Installer SideStore sur iPhone à partir de Linux (Ubuntu)

> Un guide simple, rapide et 100 % autonome pour installer SideStore depuis Ubuntu.  
> ✅ Compatible iOS 17.0 → 18.5 *(⚠️ iOS 18.6 non encore testé — mise à jour à venir)*  
> 🔧 Sans macOS, sans VM, sans jailbreak.

![OS Support](https://img.shields.io/badge/OS-Linux%20(Ubuntu%2022.04%2B)-orange)
![iOS Support](https://img.shields.io/badge/iOS-17.0--18.5-green)
![Jailbreak](https://img.shields.io/badge/jailbreak-non%20requis-blue)
![Statut](https://img.shields.io/badge/statut-fonctionnel-brightgreen)
![Discord](https://img.shields.io/discord/1120610893288335490?label=SideStore%20Discord&logo=discord)

---

## 📦 Dépendances à installer

Avant de commencer, exécute ces commandes dans ton terminal :

```bash
sudo apt update
sudo apt install software-properties-common
sudo add-apt-repository universe -y

sudo apt-get install binutils python3-pip python3-requests python3-keyring \
git gir1.2-appindicator3-0.1 usbmuxd libimobiledevice6 libimobiledevice-utils \
wget curl libavahi-compat-libdnssd-dev zlib1g-dev unzip usbutils \
libhandy-1-dev gir1.2-notify-0.7 psmisc
```

---

## 🚀 Lancer l’installation

Clone ce dépôt ou télécharge ses fichiers, puis exécute le script :

```bash
python3 main.py
```

Le script détecte automatiquement ton iPhone connecté via USB et installe :

- L’app SideStore (.ipa)
- Le profil nécessaire (automatiquement injecté dans l’iPhone)

✅ **Aucune manipulation manuelle via Safari ou Réglages n’est requise.**

---

## 📱 Finalisation sur l’iPhone

Une fois le script terminé :

1. L’app **SideStore** apparaîtra sur l’écran d’accueil  
2. Va dans **Réglages > VPN et gestion de l’appareil**  
3. Active la **confiance** pour le profil installé automatiquement  
4. Lance l’app SideStore, c’est prêt !

---

## 🔁 Re-signature automatique

- SideStore permet de re-signer automatiquement les apps chaque semaine  
- Le Companion Linux assure la communication avec ton iPhone via USB ou Wi-Fi  
- Laisse-le simplement tourner en arrière-plan

---

## ❓ Dépannage

| Problème                  | Solution                                                   |
|---------------------------|------------------------------------------------------------|
| iPhone non détecté        | Vérifie ton câble, déverrouille l’iPhone, autorise l’accès |
| Signature échouée         | Vérifie que le Companion tourne et que ton Apple ID est correct |
| Rien ne se passe          | Redémarre le script avec `python3 main.py`                |

---

## 💬 Liens utiles

- 🌐 Site officiel SideStore : [https://sidestore.io](https://sidestore.io)  
- 💬 Discord officiel : [https://discord.gg/RgpFBX3Q3k](https://discord.gg/RgpFBX3Q3k)

---

## 📸 Illustration

```markdown
<p align="center">
  <img src="assets/sidestore-linux-install.png" width="90%" alt="Installation SideStore Linux">
</p>
```

> *(Tu peux mettre ici une image dans `/assets/sidestore-linux-install.png`)*

---

## ⭐️ Merci

Si ce guide t’a été utile, pense à laisser une ⭐️ et à le partager !

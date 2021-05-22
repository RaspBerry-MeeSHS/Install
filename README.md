# Install

https://raspberry-pi.fr/raspberry-pi-sans-ecran-sans-clavier/

[memoCmd](https://fr.wikipedia.org/wiki/Commandes_Unix)
- Maj  
  ``sudo apt update``  
  ``sudo apt upgrade``  

-Gestion compte  
  ``sudo adduser``  
  [ubuntu doc](https://doc.ubuntu-fr.org/adduser)  
  ``sudo usermod -aG sudo nickname``  
  ``sudo visudo``

- Gestion prompt  
  [zsh]()  
  [omyzsh](https://github.com/ohmyzsh/ohmyzsh/wiki/Cheatsheet)  
  ``sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"``  
  [tmux](https://github.com/tmux/tmux/wiki)

- Pi-hole  
  - avoir definit une plage IP pour chaque utilisation
    - [tuto IP fixe rasp](https://raspberry-pi.fr/ip-locale-fixe/)
    - mettre le routeur 192.168.1.254 en source DNS dans Pi-hole
      - |  Ports   |  Utilité |  
      - |  :----:  |  :----:  |  
      - |    1     |    1     |
      - |   254    |   Box    |
  - changer sur chaque poste l'adresse ip du DNS
  - (si possible) changer le DHCP  
  ``curl -sSL https://install.pi-hole.net | bash``  
  [Doc](https://docs.pi-hole.net/)
  
- WireGuard
  ``sudo apt install wireguard``
  [Doc](https://www.wireguard.com/)

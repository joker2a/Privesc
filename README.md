# Privesc



#4 scripts pour élévation de privilèges lors de vos pentests


Quand on arrive à exploiter la machine d’une cible lors d’un pentest, souvent on se trouve avec les droits d’un utilisateur normal, du coup on commence à chercher un moyen pour élever nos privilèges sur la machine afin de pouvoir aller encore plus loin dans notre pentest.


#######Linenum



Linenum est un script qui effectue près de 65 contrôles et retourne plein d’informations utiles, par exemple : liste des utilisateurs root, vérifie si les mots de passe sont sauvegardés dans /etc/passwd, informations sur le réseau, vérifie sur l’utilisateur a des droits sudo avec ou sans mot de passe ou si le répertoire /home de l’utilisateur root est accessible ou pas et beaucoup plus [0] ! Linenum est disponible sur sur Github :



git clone https://github.com/rebootuser/LinEnum

######Linuxprivchecker



Linuxprivchecker quant à lui vérifie et liste la config de la machine (taches cron, version du noyau, points de montages, entrées fstab, liste les utilisateurs, sudoers, vérifie les permissions des fichiers…), à la fin il retourne une liste des exploits qui peuvent vous garantir des droits root.


wget http://www.securitysift.com/download/linuxprivchecker.py


######Linux Exploit Suggester



Comme son l’indique, ce script check la version du noyau du système et va chercher sur tout les exploits affectant cette version. 


git clone https://github.com/PenturaLabs/Linux_Exploit_Suggester.git

######Unix-Privesc-checker



Ce script permet de trouver les mauvaises configurations et les permissions des fichiers qui peuvent vous garantir des droits d’administrateur !


git clone https://github.com/pentestmonkey/unix-privesc-check.git

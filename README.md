# Le chiffrement d'un message avec le module Crypto_project (by ialy 501)

Le module correspond a crypte un message que l'autre personne destinée puisse le lire a l'aide d'une cle

### Le principe du chiffrement asymétrique 

Naruto voudrait pouvoir correspondre secrètement avec Hinata , sans que Sakura ne puisse lire les messages que Hinata lui envoie. Naruto génère un jeu de deux clés de chiffrement:

- une clé publique , qu'il envoie à Hinata, et qui permettra à Hinata de chiffrer les messages qu'elle enverra à Naruto 
- une clé privée, qu'il conserve précieusement pour lui, et qui lui permettra de déchiffrer les messages chiffrés par Hinata  avec sa clé publique.

Naruto peut distribuer la clé publique à autant de personne qu'il le souhaite, cette clé ne sert qu'à chiffrer les messages !
Si Naruto veut pouvoir chiffrer les messages qu'il envoie à Hinata, il faut que Hinata génère un autre jeu de clés, et qu'elle lui donne sa clé publique.


## Installer le module Crypto


### installer python

```sh
sudo apt-get install python3
```
	sudo apt-get install python3


### installer crypto

```sh
sudo apt-get install python3-crypto
```
		

## Quelque details a suivre 


### git le projet 


```sh
git clone https://github.com/ialy501/crypto_project.git
```

### installer des fichier dans crypto_project

aller dans le dossier crypto_project
```sh
cd crypto_project/
```

installer les 5 fichiers(tocrypt, crypted, todecrypt, decrypted, key)
```sh
mkdir tocrypt
mkdir todecrypt
mkdir decrypted
mkdir todecrypt
mkdir key
```

### Mettre le message coder sur le dossier tocrypt

aller dans le fichier tocrypt
```sh
cd crypto_project/tocrypt
```

creer un fichier text (ex: mess.txt)
```sh
touch mess.txt
```
ecrire le message dans le fichier text (mess.txt)


### Donner les droit d'execution au script

aller dans le fichier source (src)
```sh
cd crypto_project/src
```
droit d'execution:
```sh
chmod +x crypt.sh
chmod +x decrypt.sh
```


## execution du module cryto 


### Donner les droit d'execution au script

aller dans le fichier crypto_project
```sh
cd crypto_project/
```

droit d'execution:
```sh
chmod +x install.sh
chmod +x unstall.sh
```

### INSTALL

Commencer le cryptage du message
```sh
cd crypto_project/
./install.sh
```


### cryptage de message


verifier le cryptage est effectue
command:

```sh
sudo systemctl status crypt.sh.service
```


### decryptage de message


verifier le decryptage est effectue
command:

```sh
sudo systemctl status decrypt.service
```

## UNSTALL

```sh
cd crypto_project/
./unstall.sh
```



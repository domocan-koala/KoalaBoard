# KoalaBoard

![Koalaboard Domocan](/3D_dessus.jpg)

## Présentation

La KoalaBoard permet d'intégrer facilement la technologie ARM Cortex-M3 dans le système domotique [Domocan Master Édition](https://www.abcelectronique.com/bigonoff/forum/forumdisplay.php?fid=22). Ses deux connecteurs regroupent l’intégralité des entrées et sorties disponibles pour accueillir une [carte fille](https://github.com/domocan-koala/KoalaBoard_Carte-fille-template) complémentaire qui viendra spécialiser son utilisation dans votre installation. Les options disponibles se configurent grâce à des jumpers en fonction des besoins de l’utilisateur et de la carte fille qui va lui être associée.

## Caractéristiques techniques

* Alimentation 5V micro USB
* LPC1768 cadencé à 100MHz
* Connecteur JTAG 2x10 pins
* USB Slave
* Deux drivers CAN (*SN65HVD230*)
* Mémoire EEPROM (*24LC512*)
* Buzzer
* Support de pile 2032 et quartz pour le RTC
* Une led USB/INFO

## Configuration des jumpers

* **JP1** : Sélection de l'alimentation. (*Sans jumper, la carte doit être alimentée par la carte fille*)
* **JP2** : Active le Buzzer. (*La carte fille ne peut plus utiliser P1.20*)
* **JP3** : Active la LED USB/INFO. (*La carte fille ne peut plus utiliser P1.18*)
* **JP4** et **JP5** : Active la mémoire EEPROM. (*Ainsi que les deux résistances de pullup 4.7K*)
* **JP6**, **JP7**, **JP8** et **JP9** : Active l'USB Slave. (*La carte fille ne peut plus utiliser P0.29, P0.30, P1.30 et P2.09*)
* **JP10** et **JP11** : Active CAN1. (*La carte fille ne peut plus utiliser P0.00 et P0.01*)
* **JP12** et **JP13** : Active CAN2. (*La carte fille ne peut plus utiliser P0.04 et P0.05*)
* **JP14** : Active la LED POWER
* **JP15** : Active la résistance de terminaison CAN2
* **JP16** : Active la résistance de terminaison CAN1


## Historique
	
	* 23/02/18 V1.0 : Première version mise en ligne
## Quel est l'interêt du titlepack?
N'importe quand vous voulez recalculer les ombres d'anciennes versions de Maniaplanet, ou convertir des cartes d'anciens jeux Trackmania, ce titlepack peut facilement le faire en masse.

## Qu'est-ce qu'un MapType?
C'est un script spécial qui dit so la carte est construite correctement. Les cartes qui ne respectent pas la condition requise est interdite par le jeu à jouer en solo et multi.

## Mais pourquoi MapType?
Cette fonctionnalité a été concue exprès pour convertir correctement les map Platform, Stunt et Puzzle de TM1 à TM², mais cela peut être utilisé de bien d'autres manières, évidemment. Par exemple, en rendant le maps jouable si leur "MapType" est perdu, etc.

## Comment utiliser cet outil?
Tout d'abord, vous devez spécifier le dossier dans lequel sont localisées vos maps, à  l'intérieur de Maps/. Vous pouvez aussi ne rien spécifier afin de calculer les ombres de toutes vos maps. Ensuite, vous pouvez optionnelement spécifier le "MapType" qui s'appliquera à ces maps, ou bien mettre en pause cette fonctionnalité grâce a la case verte dans le coin. Finalement, vous êtes prêt pour cliquer sur Compute Them All. Pour arrêter le processus, cliquer sur le bouton Terminate dans le menu. Vous avez 2 secondes pour le cliquer entre chaque map. Si vous êtes en plein calcul d'ombres, vous pouvez simplement cliquer sur le bouton Retour (rien ne sera cassé de cette façon) et vous serez renvoyé au menu principal où vous pourrez cliquer Terminate. **Note: Les ombres seront non calculées mais le MapType sera changé.**

## Quels sont les problèmes exacts causés par l'annulation de l'enregistrement de cartes qui ont déjà eu leur ombres calculées?
Le dossier de map précédent contenant les ombres calculées peut parfois être remplacé par un autre n'en contenant aucunes, ce qui pourrait même rendre les choses plus lentes que faire le travail manuellement. Cependant, mettre en pause ceci rend l'outil utilisable pour le changement de masse de MapType, où n'importe quoi de ce type. Dans ce cas, je propose quand même de faire une sauvegarde de vos cartes. Pour une sécurité maximale, je conseille de garder cette fonctionnalité activée.

## En quoi est-ce meilleur que /calculateallshadows?
Vous avez raison, /calculateallshadows marche, mais vous n'avez aucune idée où en est le processus, ni aucun contrôle sur ce dernier. Auparavant, vous pouviez aussi répliquer la même fonctionnalité de cet outil avec quelques commandes supllémentaires, mais depuis MP4.1, la plupart de ces commandes ont été cassées. (merci Nadeo)

## J'ai remarqué que les ombres de ma map ne sont pas calculées en Hautes, mais en Defaut. Pourquoi?
Cela a du être choisi en raison de choses techniques. Si vous calculez les ombres en plus hautes que Defaut, les données ne sont pas enregistrées dans le fichier, mais dans votre cache, ce qui veut dire que les autres joueurs ne verront pas les ombres calculées en Hautes. Si vous voulez les calculer en Hautes, je vous recommande de le faire à part uniquement sur les maps où vous en avez vraiment besoin.

## Mes maps utilisent un autre "MapType" que Race. Que devrais-je faire pour garder le "MapType" original pour toutes mes maps?
Dans l'étape "MapType" de l'outil, cliquez sur la petite case dans le coin. La fonctionnalité sera mise en pause. Recliquer remettra la fonctionnalité en cours.

## J'ai converti une map Stadium de TM1, mais plusieurs blocks ont soudainement disparu. Pourquoi?
Moi non plus, je ne suis pas sûr, mais je considère cela comme un bug de Maniaplanet, qui arrive la plupart du temps pour les sculptures. Cela arriverait de toute façon si vous convertissiez manuellement. Actuellement, je suis en train d'essayer de trouver une solution. Pour l'instant, vous n'avez aucune autre option que de les placer manuellement (au coût de perdre l'auteur original de la map si ce n'est pas vous)

## J'ai minimisé mon jeu, mais le calcul d'ombres n'a pas avancé après avoir checké. Pourquoi ça s'est juste arrêté?
Quand vous cliquez sur le bouton pour minimiser en haut a droite de votre écran, tous les scripts qui font le calcul d'ombres freezent. Vous devez Alt+Tab ou switcher d'application autrement depuis le jeu pour garder le processus de calcul d'ombres actif.

## Après le calcul d'ombres, la taille des maps est très petite, super! Était-ce prévu?
En réalité, non. Les ombres n'étaient pas enregistrées dans le fichier de la carte. Cela arrive habituellement quand les cartes ont déjà eu leurs ombres calculées auparavant. Vous pouvez checker votre dossier de Cache dans C:/ProgramData/ManiaPlanet/Cache et enlever les fichiers .Bump.LightMap.zip. Ils devraient être les plus récents. Si vous n'êtes pas sûrs, vous pouvez aussi videz le cache entièrement dans les paramètres de Maniaplanet, ce qui marchera tout aussi bien.

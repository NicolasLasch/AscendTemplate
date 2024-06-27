Template téléchargable pour setup directement l'environement pour programmer un mod pour Ascend.

Informations sur l'installation des sources pour les moddeurs
==============================
Ce code suit la méthodologie d'installation de Minecraft Forge. Il appliquera
quelques petits correctifs au code source vanille de MCP, vous donnant accès à certaines données et fonctions dont vous avez besoin pour construire un mod réussi.
à certaines des données et fonctions dont vous avez besoin pour construire un mod réussi.

Notez également que les correctifs sont construits à partir du code source MCP "non renommé" (aka
SRG Names) - ce qui signifie que vous ne pourrez pas les lire directement avec du
code normal.

Processus d'installation :
==============================

Etape 1 : Ouvrez votre ligne de commande et naviguez jusqu'au dossier où vous avez extrait le fichier zip.

Étape 2 : Vous avez le choix.
1. Ouvrez IDEA, et importez le projet.
2. Sélectionner votre fichier build.gradle et le faire importer.
3. Exécuter la commande suivante : `gradlew genIntellijRuns` (`./gradlew genIntellijRuns` si vous êtes sur Mac/Linux)
4. Rafraîchir le projet Gradle dans IDEA si nécessaire.

Si à un moment donné il vous manque des librairies dans votre IDE, ou si vous rencontrez des problèmes, vous pouvez
lancer `gradlew --refresh-dependencies` pour rafraîchir le cache local. `gradlew clean` pour tout remettre à zéro
{cela n'affecte pas votre code} et recommencer le processus.

Noms de mappage :
=============================
Par défaut, le MDK est configuré pour utiliser les noms de mapping officiels de Mojang pour les méthodes et les champs
dans la base de code Minecraft. Ces noms sont couverts par une licence spécifique. Tous les moddeurs doivent connaître cette licence.
Si vous n'êtes pas d'accord avec cette licence, vous pouvez changer vos noms de mapping pour d'autres noms crowdsourcés dans votre fichier
build.gradle. Pour le texte de la licence le plus récent, référez-vous au fichier de mapping lui-même, ou à la copie de référence ici :
https://github.com/MinecraftForge/MCPConfig/blob/master/Mojang.md

Ressources supplémentaires :
=========================
Documentation de la communauté : http://mcforge.readthedocs.io/en/latest/gettingstarted/
Vidéo d'installation de LexManos : https://www.youtube.com/watch?v=8VEdtQLuLO0
Forum de la Forge : https://forums.minecraftforge.net/
Forge Discord : https://discord.gg/UvedJ9m
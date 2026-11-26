# Application QCM avec le thème « Lecture GPS : petits plans »

Copie de l'application QCM (variante allégée) avec un thème supplémentaire : 48 petits plans, six familles de questions (type, élément tolérancé, éléments de référence, référence spécifiée, zone de tolérance, contraintes de situation). Corrections avec schémas.
`QCM_GPS_complet` ajoute le second thème « vrais plans » (28 exercices), à diffuser ensuite.

Reproduire l'intégration sur une autre version de l'application :
`python3 integrer_qcm.py index_source.html index_sortie.html gps_petits.js [gps_vrais.js]`
(scripts et modules dans `GPS_lecture_bdd/interface_qcm/`). L'intégration ajoute un module, deux entrées THEMES et ORDER, un peu de CSS et l'affichage du schéma de correction (`fbHtml`).
Stockage : mêmes clés que l'application (préfixe `sub-` pour la variante allégée).

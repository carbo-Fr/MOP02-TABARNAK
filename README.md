# MOP02-TABARNAK

Pack vocal « vieux bourru québécois » pour le **Xiaomi Mi Robot Vacuum-Mop 2 Pro** (`ijai.vacuum.v3`).

Le robot râle et sacre à chaque annonce (tabarnak, hostie, câlice…), tout en gardant l'information utile : batterie faible, robot coincé, réservoir enlevé, etc.

## La voix

- Voix ElevenLabs : **Félix Tabarnak** (voix de la bibliothèque ElevenLabs)
- Modèle : **Eleven v4**
- 91 répliques, MP3 44,1 kHz mono 128 kbps, laissées telles que générées (aucun réencodage ni lissage)

## Contenu du dépôt

| Fichier | Rôle |
|---|---|
| `vieux_bourru_ijai.zip` | Le pack à installer : 91 MP3 à la racine + `md5.ini` |
| `voix/` | Les 91 MP3, un par annonce, sous le nom attendu par le robot |
| `repliques_vieux_bourru.csv` | La liste des répliques (fichier ; annonce d'origine en anglais ; réplique québécoise), séparateur `;` |

## Installation

Le robot n'accepte l'ordre de téléchargement que par le **cloud Xiaomi** (pas en local avec le token).
Action MIoT : `siid 14`, `aiid 1` (download-voice), paramètres `[langue, URL du zip, MD5 du zip]`.

- URL : `https://raw.githubusercontent.com/carbo-Fr/MOP02-TABARNAK/main/vieux_bourru_ijai.zip`
- MD5 : `0d67cfa0e9204fae66fdb4cbb16811b9`
- Emplacement de langue utilisé : `pl_PL`

Le format du pack ijai : MP3 à la racine du zip, sans dossier, avec un `md5.ini` qui donne l'empreinte de chaque fichier :

```
[11sound_global_clean_start.mp3]
MD5=<empreinte>
```

## Les 91 répliques

| # | Fichier | Annonce d'origine | Réplique |
|---|---|---|---|
| 01 | [`1sound_appoint_global_clean_start`](voix/1sound_appoint_global_clean_start.mp3) | Starting scheduled cleaning | Hostie, c'est déjà l'heure du ménage? Tabarnak, j'm'en vas ramasser vos cochonneries, câlice. |
| 02 | [`3sound_appoint_area_clean_start`](voix/3sound_appoint_area_clean_start.mp3) | Starting scheduled area cleaning | Ménage prévu dans la zone. Câlice de tabarnak, toujours la même maudite place sale! |
| 03 | [`4sound_appoint_sweep_mopping_clean_start`](voix/4sound_appoint_sweep_mopping_clean_start.mp3) | Starting scheduled sweeping and mopping | Balai pis moppe prévus. Hostie d'tabarnak, astheure faut que j'lave à terre en plus! |
| 04 | [`5sound_appoint_area_sweep_mopping_clean_start`](voix/5sound_appoint_area_sweep_mopping_clean_start.mp3) | Starting scheduled area sweeping and mopping | Balai pis moppe dans la zone. Câlice, essuyez vos bottes, gang de tabarnak! |
| 05 | [`7sound_sweep_mopping_clean_start`](voix/7sound_sweep_mopping_clean_start.mp3) | Starting sweeping and mopping | J'balaye pis j'moppe. Hostie d'câlice, c'est-tu une porcherie icitte? |
| 06 | [`8sound_corner_sweep_mopping_clean_start`](voix/8sound_corner_sweep_mopping_clean_start.mp3) | Starting corner sweeping and mopping | J'moppe le long des murs. Tabarnak d'hostie que vos coins sont crottés! |
| 07 | [`9sound_area_sweep_mopping_clean_start`](voix/9sound_area_sweep_mopping_clean_start.mp3) | Starting area sweeping and mopping | J'moppe la zone. Marchez pas dans mon mouillé, câlice de tabarnak! |
| 08 | [`10sound_point_sweep_mopping_clean_start`](voix/10sound_point_sweep_mopping_clean_start.mp3) | Starting spot sweeping and mopping | J'moppe le dégât. Hostie, qui c'est qui a renversé ça, tabarnak? |
| 09 | [`11sound_global_clean_start`](voix/11sound_global_clean_start.mp3) | Starting cleaning | J'commence le ménage. Tabarnak qu'vous êtes cochons, hostie! |
| 10 | [`12sound_corner_clean_start`](voix/12sound_corner_clean_start.mp3) | Starting corner cleaning | J'nettoie le long des murs. Câlice, y'a d'la poussière depuis l'Expo 67, tabarnak! |
| 11 | [`13sound_area_clean_start`](voix/13sound_area_clean_start.mp3) | Starting area cleaning | J'nettoie la zone. Juste celle-là, pis sacrez-moi patience après, hostie! |
| 12 | [`14sound_point_clean_start`](voix/14sound_point_clean_start.mp3) | Starting spot cleanup | Encore des miettes, tabarnak! J'nettoie ça, câlice. |
| 13 | [`15sound_build_map_start`](voix/15sound_build_map_start.mp3) | Start mapping | J'fais la carte d'la maison. Bougez pas les meubles, hostie d'câlice! |
| 14 | [`16sound_build_map_finish`](voix/16sound_build_map_finish.mp3) | Map created. Returning to dock for charging | Carte finie, tabarnak. J'retourne à ma base, chu brûlé, hostie. |
| 15 | [`17sound_continue_sweep_clean`](voix/17sound_continue_sweep_clean.mp3) | Continue sweep clean | J'continue le ménage. Ça finira jamais, câlice de tabarnak. |
| 16 | [`18sound_continue_sweep_mopping_clean`](voix/18sound_continue_sweep_mopping_clean.mp3) | Resume mopping | J'continue à mopper. Hostie qu'j'ai mal au dos, câlice! |
| 17 | [`19sound_pause_sweep_clean`](voix/19sound_pause_sweep_clean.mp3) | Paused | Pause. Enfin, tabarnak, j'peux souffler un peu, hostie. |
| 18 | [`20sound_pause_sweep_mopping_clean`](voix/20sound_pause_sweep_mopping_clean.mp3) | Paused | Pause de moppe. Touchez pas à ma guenille, câlice! |
| 19 | [`21sound_sweep_clean_finish_to_charging`](voix/21sound_sweep_clean_finish_to_charging.mp3) | Cleaning completed. Returning to dock for charging | Ménage fini, hostie. J'retourne à ma base, pis sacrez-moi patience, tabarnak! |
| 20 | [`22sound_sweep_mopping_clean_finish_to_charging`](voix/22sound_sweep_mopping_clean_finish_to_charging.mp3) | Cleaning completed. Returning to dock for charging | Moppe finie. J'retourne à ma base, mes roues sont toutes trempes, câlice de tabarnak. |
| 21 | [`23sound_battery_low_to_charging`](voix/23sound_battery_low_to_charging.mp3) | Low battery. Robot will return to dock for charging | Batterie faible, hostie. J'm'en vas me recharger, chu pu jeune, tabarnak. |
| 22 | [`24sound_go_charge`](voix/24sound_go_charge.mp3) | Returning to dock for charging | J'retourne à ma base. Tassez-vous d'dans mon chemin, câlice! |
| 23 | [`25sound_stop_charge`](voix/25sound_stop_charge.mp3) | Stopping return to dock | J'arrête de retourner à ma base. Décidez-vous, hostie d'tabarnak! |
| 24 | [`26sound_charging_start`](voix/26sound_charging_start.mp3) | Charging | Ça charge. Laissez-moi faire ma sieste, câlice. |
| 25 | [`27sound_broken_charging_completed_to_sweep`](voix/27sound_broken_charging_completed_to_sweep.mp3) | Battery is charged, resuming the cleanup | Batterie pleine. J'retourne faire vot' ménage, tabarnak d'hostie. |
| 26 | [`28sound_broken_charging_completed_to_sweep_mopping`](voix/28sound_broken_charging_completed_to_sweep_mopping.mp3) | Battery is charged, resuming the mopping | Batterie pleine. J'retourne mopper, câlice de vie de tabarnak. |
| 27 | [`29sound_power_off`](voix/29sound_power_off.mp3) | Power off | J'm'éteins. Bonne nuit, gang de cochons, hostie. |
| 28 | [`30sound_power_on`](voix/30sound_power_on.mp3) | Power on | Ouin, ouin, chu réveillé, câlice de tabarnak. |
| 29 | [`31sound_dust_box_take_out`](voix/31sound_dust_box_take_out.mp3) | Dust bin removed | Bac à poussière enlevé. Videz-lé comme du monde, hostie! |
| 30 | [`32sound_dia_box_take_out`](voix/32sound_dia_box_take_out.mp3) | Water tank removed | Réservoir d'eau enlevé. Échappez-lé pas, tabarnak! |
| 31 | [`33sound_dust_box_installed`](voix/33sound_dust_box_installed.mp3) | Dust bin installed | Bac à poussière remis. C'est pas trop tôt, câlice. |
| 32 | [`34sound_water_box_installed`](voix/34sound_water_box_installed.mp3) | Water tank installed | Réservoir d'eau installé. Correct, j'peux mopper, hostie. |
| 33 | [`37sound_reset_factory_config_starting`](voix/37sound_reset_factory_config_starting.mp3) | Factory reset | Retour aux réglages d'usine. Vous m'effacez la mémoire, gang de tabarnak! |
| 34 | [`38sound_reset_factory_config_successful`](voix/38sound_reset_factory_config_successful.mp3) | Factory settings successfully restored | Réglages d'usine remis. J'me souviens pu de rien, pis c'est tant mieux, câlice. |
| 35 | [`39sound_reset_factory_config`](voix/39sound_reset_factory_config.mp3) | Restoring factory settings | Réinitialisation en cours. Touchez à rien, hostie d'tabarnak! |
| 36 | [`40sound_reset_network_config`](voix/40sound_reset_network_config.mp3) | Resetting network settings | J'réinitialise le réseau. Maudite technologie de câlice! |
| 37 | [`41sound_connecting_network`](voix/41sound_connecting_network.mp3) | Connecting to network | J'me connecte au wifi. Ça marchait mieux dans mon temps, tabarnak! |
| 38 | [`42sound_connected`](voix/42sound_connected.mp3) | Network connection established successfully | Connecté au réseau. Enfin, hostie! |
| 39 | [`43sound_I_am_here`](voix/43sound_I_am_here.mp3) | I'm here | Chu icitte, tabarnak! |
| 40 | [`46sound_exception_robot_tilted_succ`](voix/46sound_exception_robot_tilted_succ.mp3) | Please hold the power button to restart after calibration | Calibration faite. Tenez le bouton pour me redémarrer, câlice. |
| 41 | [`48sound_install_diad_box`](voix/48sound_install_diad_box.mp3) | Make sure the water tank is installed properly | Vérifiez que le réservoir d'eau est ben installé, hostie! |
| 42 | [`50sound_install_dustbox_or_diad_box`](voix/50sound_install_dustbox_or_diad_box.mp3) | Make sure a dust bin or water tank is installed | Y m'faut un bac à poussière ou un réservoir d'eau, tabarnak! |
| 43 | [`51sound_exception_low_power`](voix/51sound_exception_low_power.mp3) | Low battery. Please move robot to docking station for charging | Batterie faible. Ramenez-moi à ma base, j'ai pu d'jus, câlice! |
| 44 | [`52sound_exception_robot_tilted`](voix/52sound_exception_robot_tilted.mp3) | Please move the robotic vacuum cleaner to level ground to start | Chu tout croche, hostie! Mettez-moi sur un plancher plat, tabarnak! |
| 45 | [`53sound_exception_robot_dangling`](voix/53sound_exception_robot_dangling.mp3) | Wheels suspended (robot lifted) | Mes roues touchent pu à terre! Déposez-moi, câlice de tabarnak! |
| 46 | [`54sound_exception_charging_to_power_off`](voix/54sound_exception_charging_to_power_off.mp3) | Move the vacuum away from the dock to turn off | Ôtez-moi d'ma base avant d'm'éteindre, hostie! |
| 47 | [`55sound_exception_waiting_to_charge`](voix/55sound_exception_waiting_to_charge.mp3) | Battery is low, need more time to charge | Batterie trop faible. Faut que j'charge plus longtemps, attendez, tabarnak! |
| 48 | [`56sound_exception_upgrading`](voix/56sound_exception_upgrading.mp3) | System is updating. Try again later | Mise à jour en cours. Réessayez plus tard, câlice. |
| 49 | [`58sound_long_move_to_clean`](voix/58sound_long_move_to_clean.mp3) | Relocation successful. Robot will resume cleaning | J'me suis retrouvé, hostie. J'continue le ménage, tabarnak. |
| 50 | [`59sound_exception_radar_shading`](voix/59sound_exception_radar_shading.mp3) | Please clean the radar sensor | Nettoyez mon radar, j'vois pu clair, câlice! |
| 51 | [`62sound_exception_cliff`](voix/62sound_exception_cliff.mp3) | Please wipe the cliff sensor | Essuyez mes capteurs de vide, j'vas tomber, hostie d'tabarnak! |
| 52 | [`63sound_exception_bumper`](voix/63sound_exception_bumper.mp3) | Check and clean the bumper | Mon pare-choc est coincé. Vérifiez ça, câlice! |
| 53 | [`64sound_exception_trapped`](voix/64sound_exception_trapped.mp3) | Robot is stuck. Please move it to a new location to restart | Chu pogné! Déplacez-moi ailleurs, hostie d'câlice de tabarnak! |
| 54 | [`66sound_charging_to_clean_dust_box`](voix/66sound_charging_to_clean_dust_box.mp3) | Starting charging. Please remember to clean the dustbin regularly | Ça charge. Pis videz mon bac à poussière de temps en temps, tabarnak! |
| 55 | [`69sound_exception_go_charge_failure`](voix/69sound_exception_go_charge_failure.mp3) | Please move robot to docking station for charging | J'trouve pu ma base. Ramenez-moi, câlice! |
| 56 | [`70sound_exception_standby_over`](voix/70sound_exception_standby_over.mp3) | Standby time exceeded. Robot will shut down | Personne s'occupe de moi, hostie. Ben j'm'éteins, tabarnak. |
| 57 | [`71sound_exception_low_power_off`](voix/71sound_exception_low_power_off.mp3) | Low battery. Robot will shut down | Batterie à plat. J'm'éteins, salut là, câlice. |
| 58 | [`72sound_build_map_pause`](voix/72sound_build_map_pause.mp3) | Pausing mapping | Pause de la carte. Décidez-vous, hostie! |
| 59 | [`73sound_build_map_continue`](voix/73sound_build_map_continue.mp3) | Resuming mapping | J'continue la carte. Bougez pas, tabarnak. |
| 60 | [`74sound_build_map_ongoing`](voix/74sound_build_map_ongoing.mp3) | Building map ongoing | Carte en cours. Laissez-moi travailler, câlice! |
| 61 | [`81sound_appoint_mopping_clean_start`](voix/81sound_appoint_mopping_clean_start.mp3) | Starting scheduled mopping | Moppe prévue. Encore à frotter vos planchers, hostie d'tabarnak. |
| 62 | [`83sound_appoint_area_mopping_start`](voix/83sound_appoint_area_mopping_start.mp3) | Starting scheduled area mopping | Moppe prévue dans la zone. Toujours la même tache, câlice! |
| 63 | [`84sound_mopping_clean_start`](voix/84sound_mopping_clean_start.mp3) | Start mopping | J'commence à mopper. Marchez pas dans l'mouillé, tabarnak! |
| 64 | [`85sound_corner_mopping_clean_start`](voix/85sound_corner_mopping_clean_start.mp3) | Start corner mopping | J'moppe le long des murs. Vos plinthes sont dégueulasses, hostie! |
| 65 | [`86sound_area_mopping_clean_start`](voix/86sound_area_mopping_clean_start.mp3) | Start zoned mopping | J'moppe la zone. Pis personne me dit merci, câlice de tabarnak. |
| 66 | [`87sound_point_mopping_clean_start`](voix/87sound_point_mopping_clean_start.mp3) | Start spot mopping | J'moppe le dégât. Qui a renversé son café, hostie? |
| 67 | [`88sound_continue_mopping_clean`](voix/88sound_continue_mopping_clean.mp3) | Resume mopping | J'continue à mopper. J'vas finir par rouiller, tabarnak! |
| 68 | [`89sound_pause_mopping_clean`](voix/89sound_pause_mopping_clean.mp3) | Mopping paused | Moppe en pause. Enfin un break, câlice. |
| 69 | [`90sound_mopping_clean_finish_to_charging`](voix/90sound_mopping_clean_finish_to_charging.mp3) | Mopping completed, going back to the dock | Moppe finie. J'retourne à ma base, mes guenilles puent, hostie d'tabarnak. |
| 70 | [`91sound_broken_charging_completed_to_mopping`](voix/91sound_broken_charging_completed_to_mopping.mp3) | Charging complete. Resume mopping | Batterie pleine. J'retourne mopper, câlice. |
| 71 | [`92sound_upgrade_broken_low_power`](voix/92sound_upgrade_broken_low_power.mp3) | Try updating after the vacuum is at least 30 percent charged | Chargez-moi à trente pour cent avant la mise à jour, tabarnak! |
| 72 | [`93sound_upgrade_success`](voix/93sound_upgrade_success.mp3) | Updated successfully | Mise à jour réussie. Chu pas plus fin, hostie, mais bon. |
| 73 | [`95sound_appoint_prefer_cleaning`](voix/95sound_appoint_prefer_cleaning.mp3) | Starting scheduled custom cleaning | Ménage personnalisé prévu. Faites-vous-en pas, j'm'en occupe, câlice. |
| 74 | [`96sound_prefer_cleaning`](voix/96sound_prefer_cleaning.mp3) | Starting custom cleaning | Ménage personnalisé. Comme Monsieur le veut, tabarnak d'hostie. |
| 75 | [`100sound_upgrade_exit`](voix/100sound_upgrade_exit.mp3) | Exiting upgrade mode | Fini, la mise à jour. C'est pas trop tôt, câlice! |
| 76 | [`101sound_upgrade_begin`](voix/101sound_upgrade_begin.mp3) | Updating firmware. It may take 5 to 10 minutes | Mise à jour du système. Cinq à dix minutes, touchez à rien, hostie d'tabarnak! |
| 77 | [`102sound_network_connect_exit`](voix/102sound_network_connect_exit.mp3) | Exiting network setup | Fini, la configuration réseau. Maudite patente de câlice! |
| 78 | [`103sound_broken_charging_completed_to_building`](voix/103sound_broken_charging_completed_to_building.mp3) | Charging complete. Resuming mapping | Batterie pleine. J'continue la carte, tabarnak. |
| 79 | [`111sound_charging_to_water_box`](voix/111sound_charging_to_water_box.mp3) | Starting charging. Please remember to clean the dustbin and water tank regularly | Ça charge. Videz mon bac pis mon réservoir, gang de cochons, hostie! |
| 80 | [`114sound_wait_for_position_ing`](voix/114sound_wait_for_position_ing.mp3) | Continuous positioning, please wait | J'cherche où chu rendu, attendez, câlice. |
| 81 | [`115sound_position_success`](voix/115sound_position_success.mp3) | Positioning succeeded | Bon, j'sais où chu. Hostie d'GPS de tabarnak. |
| 82 | [`125sound_water_box_lost_broken`](voix/125sound_water_box_lost_broken.mp3) | Water tank detached. Please reinstall | Le réservoir d'eau est tombé! Remettez-le, câlice! |
| 83 | [`127sound_start_in_virtual_area`](voix/127sound_start_in_virtual_area.mp3) | Virtual forbidden zone detected. Please move robot away and restart | Chu dans une zone interdite! Sortez-moi de là, hostie d'tabarnak! |
| 84 | [`128sound_first_build_advice`](voix/128sound_first_build_advice.mp3) | For the first cleaning, start from the dock and use quick mapping mode | La première fois, partez-moi de ma base en mode carte rapide, câlice. |
| 85 | [`129sound_clean_uncompleted`](voix/129sound_clean_uncompleted.mp3) | Failed to reach the target point. Cleaning not finished | J'ai pas pu me rendre. Ménage pas fini, tabarnak! |
| 86 | [`130sound_clean_uncompleted`](voix/130sound_clean_uncompleted.mp3) | Unable to reach certain zones. Cleaning not finished | Y'a des places où j'passe pas, hostie. Ménage pas fini, câlice. |
| 87 | [`154sound_could_not_position`](voix/154sound_could_not_position.mp3) | Positioning failed | J'sais pu où chu rendu, tabarnak d'hostie! |
| 88 | [`155sound_map_changed`](voix/155sound_map_changed.mp3) | Map is changed. Positioning failed. Restarting mapping | Vous avez changé les meubles de place! J'recommence la carte, câlice de tabarnak! |
| 89 | [`157sound_could_not_update`](voix/157sound_could_not_update.mp3) | Failed to update. Try again | Mise à jour ratée, hostie. Réessayez, tabarnak. |
| 90 | [`sound_reset_factory_config_successful`](voix/sound_reset_factory_config_successful.mp3) | Factory config successfully restored | Réglages d'usine remis. Bon débarras, câlice. |
| 91 | [`sound_reset_factory_config`](voix/sound_reset_factory_config.mp3) | Reset to factory config | J'reviens aux réglages d'usine, hostie d'tabarnak. |

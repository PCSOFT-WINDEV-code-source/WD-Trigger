  
<span style="font-family:Arial sans-serif;font-size:16px;">WD Trigger</span>

  
<span style="font-family:Arial sans-serif;font-size:14px;">Cet exemple montre comment utiliser les triggers avec WINDEV.</span>

<span style="font-family:Arial sans-serif;font-size:14px;">Un trigger est une procédure en WLangage appelée automatiquement par le moteur HFSQL à chaque exécution d'une fonction HFSQL. </span>

  
<span style="font-family:Arial sans-serif;font-size:14px;">Dans cet exemple, nous abordons deux thèmes principaux :</span>

<span style="font-family:Arial sans-serif;font-size:14px;">1/ comment brancher un trigger sur une fonction HFSQL</span>

<span style="font-family:Arial sans-serif;font-size:14px;">2/ quel code utiliser dans la fonction appelée par le trigger.</span>

  
<span style="font-family:Arial sans-serif;font-size:14px;">Résumé de l'exemple livré avec WINDEV : </span>

<span style="font-family:Arial sans-serif;font-size:14px;">Cette application permet de saisir les notes de frais des collaborateurs d'une société.</span>

<span style="font-family:Arial sans-serif;font-size:14px;">Deux modes sont utilisables :</span>

<span style="font-family:Arial sans-serif;font-size:14px;">- le mode avec les droits en lecture/écriture </span>

<span style="font-family:Arial sans-serif;font-size:14px;">- le mode avec les droits en lecture seulement. </span>

<span style="font-family:Arial sans-serif;font-size:14px;">Ce sont les triggers qui permettront de contrôler l'accès aux fichiers en fonction du mode en cours. </span>

<span style="font-family:Arial sans-serif;font-size:14px;">Dans l'exemple, les triggers permettent également d'écrire dans un fichier journal les différents événements.</span>

<span style="font-family:Arial sans-serif;font-size:14px;">Ce fichier journal est directement consultable dans l'application. </span>

  
  
<span style="font-family:Arial sans-serif;font-size:14px;">( \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ ° \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ )</span>

  
<span style="font-family:Arial sans-serif;font-size:10px;">Conditions d'utilisation :</span>

<span style="font-family:Arial sans-serif;font-size:10px;">Le programme est fourni dans un but didactique.</span>

<span style="font-family:Arial sans-serif;font-size:10px;">L'utilisation de ce programme s'effectue sous la responsabilité de son utilisateur. La responsabilité de PC SOFT ne pourra en aucun cas être mise en cause si le programme ne fonctionne pas tel que vous l'attendez, ou pour quelque raison que ce soit. </span>

<span style="font-family:Arial sans-serif;font-size:10px;">Tout détenteur d'une licence WINDEV 28 enregistrée est autorisé à modifier ce programme, et est autorisé à l'inclure dans une ou plusieurs de ses applications. Dans ces cas, toute mention se rapportant à PC SOFT, à WinDev ou à WebDev devra être supprimée, afin qu'aucun doute ne puisse subsister dans l'esprit d'un utilisateur final.</span>

<span style="font-family:Arial sans-serif;font-size:10px;">Il est interdit de diffuser ou vendre ce programme exemple sans modification substantielle, ou sans l'inclure dans une application de taille substantielle.</span>

<span style="font-family:Arial sans-serif;font-size:10px;">Le support technique pour ce programme exemple est accessible à travers le service "Assistance Directe" uniquement.</span>

<span style="font-family:Arial sans-serif;font-size:10px;">Attention: si plusieurs personnes sont susceptibles d'avoir consulté ce programme, il se peut que le programme ait été modifié! </span>

<span style="font-family:Arial sans-serif;font-size:10px;">Assurez-vous d'étudier une version originale de ce programme.</span>

  
  
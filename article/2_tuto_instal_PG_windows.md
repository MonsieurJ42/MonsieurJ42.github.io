# Tuto installation PostgreSQL et PostGIS sur Windows 10

<!-- wp:paragraph -->
<p>Pour mon premier tuto nous allons voir une installation basique mais pourtant diablement utile, l’installation du SGBD <strong>PostgreSQL</strong> et de son extension spatiale <strong>PostGIS</strong> sur un OS <strong>Windows 10</strong>. Je présenterai l’installation MacOS et Linux à une autre occasion. Je ferai surement une deuxième partie de tuto ou je rentrerai dans les détails d’utilisations. </p>
<!-- /wp:paragraph -->

<!-- wp:paragraph {"align":"right"} -->
<p class="has-text-align-right"><em>Baptmen suis bien, ceci est pour toi.</em></p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3>Télécharger l’utilitaire d’installation</h3>
<!-- /wp:heading -->

<!-- wp:image {"id":80,"sizeSlug":"large"} -->
<figure class="wp-block-image size-large"><a href="https://postgresql.org" target="_blank"><img src="https://monsieurgis.files.wordpress.com/2020/09/capture1.png?w=1024" alt="" class="wp-image-80"/></a></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Pour ceci rendez-vous sur le site <strong><a rel="noreferrer noopener" href="http://postgresql.org" target="_blank">postgresql.org</a></strong>, et allez dans la section <strong>download </strong>puis<strong> Windows</strong> et télécharger une version récente. Personnellement; à l’heure de l’écriture de ce tuto, je travaille sur la 11. Une version 13 est disponible depuis le 24 septembre 2020, mais nous allons installer la <strong>version 12</strong>, la dernière en date avec laquelle <strong>PostGIS</strong> est compatible.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>En cliquant sur le lien «&nbsp;<em><strong>Download the installer</strong></em>&nbsp;» vous arriverez sur le site de <strong>EnterpriseDB</strong>.</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":81,"sizeSlug":"large"} -->
<figure class="wp-block-image size-large"><img src="https://monsieurgis.files.wordpress.com/2020/09/capture2.png?w=1024" alt="" class="wp-image-81"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Oui vous pouvez compiler vous-même <strong>PostgreSQL</strong>, mais des gens l’ont déjà fait pour vous en réduisant l’installation à un simple <strong>.exe</strong> alors pourquoi se priver&nbsp;? Téléchargez ensuite la version souhaitez, pour moi ce sera la <strong>12.4 Windows x86-64</strong>.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3>Installation de PostgreSQL</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><em>Petite précision, afin de mener tout cela a bien vous devez disposer d’accès administrateur sur votre PC (en même temps si vous n’avez pas d’accès admin à votre PC vous disposez sûrement d’un service qui peut vous faire l’installation).</em></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Exécutez le fichier que vous venez de récupérer, et acceptez le popup admin. Il va alors installer ses dépendances C++ si vous n’en disposez pas déjà, pour ensuite vous ouvrir l’utilitaire d’installation.</p>
<!-- /wp:paragraph -->

<!-- wp:image {"align":"left","id":82,"width":389,"height":305,"sizeSlug":"large"} -->
<figure class="wp-block-image alignleft size-large is-resized"><img src="https://monsieurgis.files.wordpress.com/2020/09/capture3.png?w=552" alt="" class="wp-image-82" width="389" height="305"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Cliquez alors sur suivant. Vous devez alors spécifier le <strong>répertoire d’installation</strong>. Choisissez le bien, vos bases de données et extension y seront stockée. Personnellement j’ai de la place sur mon disque système je vais donc garder le chemin par défaut au sein du «&nbsp;<em>Program Files</em>&nbsp;». Si votre mémoire est défaillante, notez votre emplacement d’installation, vous en aurez besoin plus tard.</p>
<!-- /wp:paragraph -->

<!-- wp:spacer {"height":"30px"} -->
<div style="height:30px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:spacer -->

<!-- wp:paragraph -->
<p>Vous arrivez ensuite à la «&nbsp;S<em>élection des composants</em>&nbsp;», je vais vous les détaillez rapidement, mais globalement vous pouvez tout installer ou appliquer mon choix personnel&nbsp;:</p>
<!-- /wp:paragraph -->

<!-- wp:jetpack/tiled-gallery {"align":"","columnWidths":[[50,50]],"ids":[83,84]} -->
<div class="wp-block-jetpack-tiled-gallery is-style-rectangular"><div class="tiled-gallery__gallery"><div class="tiled-gallery__row"><div class="tiled-gallery__col" style="flex-basis:50%"><figure class="tiled-gallery__item"><img alt="" data-height="432" data-id="83" data-link="https://monsieurgis.wordpress.com/capture4/" data-url="https://monsieurgis.files.wordpress.com/2020/09/capture4.png" data-width="552" src="https://monsieurgis.files.wordpress.com/2020/09/capture4.png" data-amp-layout="responsive"/></figure></div><div class="tiled-gallery__col" style="flex-basis:50%"><figure class="tiled-gallery__item"><img alt="" data-height="432" data-id="84" data-link="https://monsieurgis.wordpress.com/capture5/" data-url="https://monsieurgis.files.wordpress.com/2020/09/capture5.png" data-width="552" src="https://monsieurgis.files.wordpress.com/2020/09/capture5.png" data-amp-layout="responsive"/></figure></div></div></div></div>
<!-- /wp:jetpack/tiled-gallery -->

<!-- wp:heading {"level":4} -->
<h4>PostgreSQL Server</h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>C’est le composant principal à installer parce que sans <em><strong>Server</strong></em> pas de base de données.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->
<h4>pgAdmin 4</h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>N’étant pas un informaticien barbu, j’aime bien disposer d’une <strong>GUI</strong> (<em>Graphical User Interface</em>), parce que travailler sur le terminal c’est classe, mais nous somme au XXIème siècle. <strong>pgAdmin</strong> vous facilitera largement l’administration / organisation de votre serveur de données et la création de vos requêtes. Nous avons dorénavant droit, avec la <strong>version 4</strong>, à une application marchant sur un web-serveur et se lançant dans votre navigateur (je vous rassure ça s’installe tout seul et ça marche tout seul, pas de paramétrage d’un Apache ou d’un Tomcat ici).</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->
<h4>Stack Builder</h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Un bon outil pour la gestion d’extension, mais personnellement il est bloqué par le proxy de mon université du coup je ne l’utilise pas. Je vous montrerai donc l’installation de <strong>PostGIS</strong> en contournant ceci.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->
<h4>Command Line Tools</h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Très, très, très important, cette partie vas vous installer tous les outils de gestion de sauvegarde, d’import de données ainsi qu’une console <strong>psql</strong>... Tout du moins je crois que ça fait ça, je n’ai jamais fait d’installation sans.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Lorsque votre sélection est faite vous pouvez cliquer sur suivant.</p>
<!-- /wp:paragraph -->

<!-- wp:spacer {"height":"60px"} -->
<div style="height:60px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:spacer -->

<!-- wp:image {"align":"left","id":86,"width":414,"height":325,"sizeSlug":"large"} -->
<figure class="wp-block-image alignleft size-large is-resized"><img src="https://monsieurgis.files.wordpress.com/2020/09/capture6.png?w=552" alt="" class="wp-image-86" width="414" height="325"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Vous vous souvenez quand je vous ai dit que le répertoire d’installation était important car il contenait vos bases de données&nbsp;? Et bien j’ai menti, vous pouvez choisir ou stocker vos données. Mais si vous êtes une tête percée, légèrement désorganiser comme moi, garder celui par défaut, soit un répertoire «&nbsp;<strong>data</strong>&nbsp;» au sein de votre répertoire d’installation puis cliquez sur suivant.</p>
<!-- /wp:paragraph -->

<!-- wp:spacer {"height":"30px"} -->
<div style="height:30px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:spacer -->

<!-- wp:paragraph -->
<p>Vous arrivez alors à la création du premier <strong>superutilisateur</strong>. Celui-ci prendra comme identifiant <strong>postgres</strong> et le mot de passe que vous lui indiquez. En cliquant sur suivant vous arriverez sur le port d’écoute de votre serveur, laissez 5432 (à moins que vous soyez une craque en administration de réseaux).</p>
<!-- /wp:paragraph -->

<!-- wp:jetpack/tiled-gallery {"columnWidths":[[50,50]],"ids":[88,89]} -->
<div class="wp-block-jetpack-tiled-gallery aligncenter is-style-rectangular"><div class="tiled-gallery__gallery"><div class="tiled-gallery__row"><div class="tiled-gallery__col" style="flex-basis:50%"><figure class="tiled-gallery__item"><img alt="" data-height="432" data-id="88" data-link="https://monsieurgis.wordpress.com/capture7/" data-url="https://monsieurgis.files.wordpress.com/2020/09/capture7.png" data-width="552" src="https://monsieurgis.files.wordpress.com/2020/09/capture7.png" data-amp-layout="responsive"/></figure></div><div class="tiled-gallery__col" style="flex-basis:50%"><figure class="tiled-gallery__item"><img alt="" data-height="432" data-id="89" data-link="https://monsieurgis.wordpress.com/capture8/" data-url="https://monsieurgis.files.wordpress.com/2020/09/capture8.png" data-width="552" src="https://monsieurgis.files.wordpress.com/2020/09/capture8.png" data-amp-layout="responsive"/></figure></div></div></div></div>
<!-- /wp:jetpack/tiled-gallery -->

<!-- wp:paragraph -->
<p>Choisissez votre langue locale (celle qui vas servir à l'encodage de la base) et cliquez sur suivant pour obtenir un résumé de l’installation. Vous pouvez alors faire deux fois suivant pour lancer l’installation de <strong>PostgreSQL</strong>, (ça peut être un peu long) et vous avez terminé… l’installation, les choses sérieuses commence.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3>Initialisé PostgreSQL</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>La première étape va être de mettre à jour votre <strong>PATH</strong> car pour l’instant si vous souhaitez accéder à <strong>PostgreSQL</strong> via le terminal vous devriez obtenir ça&nbsp;:</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":91,"sizeSlug":"large"} -->
<figure class="wp-block-image size-large"><img src="https://monsieurgis.files.wordpress.com/2020/09/capture9.png?w=979" alt="" class="wp-image-91"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Pour cela récupérer le chemin d’accès au dossier <strong>bin</strong> de votre installation <strong>PostgreSQL</strong> (je vous ai dit de le noter). Aller en suite dans les paramètres du système (Win + R&nbsp;: <strong>Système</strong> ou en cliquant sur le lien «&nbsp;<strong>Information Système</strong>&nbsp;», dans la section du même nom, de la partie «&nbsp;<strong>Système</strong>&nbsp;» des Paramètres de Windows) pour ouvrir la fenêtre <strong>Système</strong> (à droite)&nbsp;:</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":92,"sizeSlug":"large"} -->
<figure class="wp-block-image size-large"><img src="https://monsieurgis.files.wordpress.com/2020/09/capture10.png?w=1024" alt="" class="wp-image-92"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Cliquez sur «&nbsp;<strong>Modifier les paramètres</strong>&nbsp;» (vous devez être admin encore une fois). Ceci ouvrira la fenêtre suivante&nbsp;:</p>
<!-- /wp:paragraph -->

<!-- wp:image {"align":"center","id":93,"width":389,"height":499,"sizeSlug":"large"} -->
<figure class="wp-block-image aligncenter size-large is-resized"><img src="https://monsieurgis.files.wordpress.com/2020/09/capture11.png?w=412" alt="" class="wp-image-93" width="389" height="499"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Allez dans l’onglet «&nbsp;<strong>Paramètres Système avancées</strong>&nbsp;» et cliquez sur «&nbsp;<strong>Variables d’environnement…</strong>&nbsp;»&nbsp;et sélectionné «&nbsp;<strong>Path</strong>&nbsp;» dans la section «&nbsp;<strong>Variables Système</strong>&nbsp;» et cliquez sur «&nbsp;<strong>Modifier…</strong>&nbsp;». Faite « <strong>Nouveau </strong>» et ajouter le chemin du dossier <strong>bin</strong> suscité&nbsp;:</p>
<!-- /wp:paragraph -->

<!-- wp:jetpack/tiled-gallery {"columnWidths":[[59.17932,40.82068]],"ids":[96,97]} -->
<div class="wp-block-jetpack-tiled-gallery aligncenter is-style-rectangular"><div class="tiled-gallery__gallery"><div class="tiled-gallery__row"><div class="tiled-gallery__col" style="flex-basis:59.17932%"><figure class="tiled-gallery__item"><img alt="" data-height="687" data-id="96" data-link="https://monsieurgis.wordpress.com/capture12/" data-url="https://monsieurgis.files.wordpress.com/2020/09/capture12.png" data-width="1049" src="https://monsieurgis.files.wordpress.com/2020/09/capture12.png" data-amp-layout="responsive"/></figure></div><div class="tiled-gallery__col" style="flex-basis:40.82068%"><figure class="tiled-gallery__item"><img alt="" data-height="501" data-id="97" data-link="https://monsieurgis.wordpress.com/capture13/" data-url="https://monsieurgis.files.wordpress.com/2020/09/capture13.png" data-width="527" src="https://monsieurgis.files.wordpress.com/2020/09/capture13.png" data-amp-layout="responsive"/></figure></div></div></div></div>
<!-- /wp:jetpack/tiled-gallery -->

<!-- wp:paragraph -->
<p>Dans cette partie «&nbsp;<strong>Variables d’environnement…</strong>&nbsp;» ajoutée aussi les variables suivantes&nbsp;:</p>
<!-- /wp:paragraph -->

<!-- wp:list -->
<ul><li><strong>PGDATA&nbsp;</strong>: Chemin vers le répertoire data</li><li><strong>PGHOME </strong>: Chemin vers le répertoire de version de PostgreSQL</li><li><strong>PGPORT </strong>: 5432</li></ul>
<!-- /wp:list -->

<!-- wp:image {"id":100,"sizeSlug":"large"} -->
<figure class="wp-block-image size-large"><img src="https://monsieurgis.files.wordpress.com/2020/09/capture28.png?w=598" alt="" class="wp-image-100"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Ensuite validez toutes les fenêtres. Dorénavant la commande «&nbsp;psql&nbsp;» dans le terminal devrait vous donner ceci :</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":101,"sizeSlug":"large"} -->
<figure class="wp-block-image size-large"><img src="https://monsieurgis.files.wordpress.com/2020/09/capture14.png?w=979" alt="" class="wp-image-101"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Si vous rentrez le mot de passe que vous avez créé vous devriez obtenir une erreur, car oui vous n’êtes rien pour le serveur (je parle de votre nom d'utilisateur Windows). Pour s’assurer que tout marche entrer la commande&nbsp;:</p>
<!-- /wp:paragraph -->

<!-- wp:preformatted -->
<pre class="wp-block-preformatted">psl -U postgres</pre>
<!-- /wp:preformatted -->

<!-- wp:paragraph -->
<p>L'option  «&nbsp;<strong>-U</strong>» stipule le nom d'utilisateur pour la connexion, En entrant le mot de passe créer plus tôt vous devriez obtenir ceci&nbsp;:</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":103,"sizeSlug":"large"} -->
<figure class="wp-block-image size-large"><img src="https://monsieurgis.files.wordpress.com/2020/09/capture15.png?w=979" alt="" class="wp-image-103"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Vous êtes connecté à la base par défaut <strong>postgres</strong>, via l’utilsateur par défaut <strong>postgres</strong>. Vous pouvez quitter la console psql en entrant «&nbsp;exit&nbsp;» et fermé votre terminal. On ne devrait plus trop avoir à utiliser celui-ci.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Vous pouvez alors lancer l’application <strong>pgAdmin4</strong>. Lors de son premier lancement l’application vas vous demander un <strong>mot de passe maitre</strong>, car celle-ci vas stocker plusieurs mots de passe utilisateur, on ne lésine jamais sur un peu plus de sécurité.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Vous obtiendrez alors ceci&nbsp;:</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":104,"sizeSlug":"large"} -->
<figure class="wp-block-image size-large"><img src="https://monsieurgis.files.wordpress.com/2020/09/capture16.png?w=1024" alt="" class="wp-image-104"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Je ne vous ferai pas une présentation complète de l’application ici, cela fera peut-être le sujet d’un autre article.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Si vous cliquez sur l’arborescence de droite vous allez déployer la liste de vos serveur (normalement un seul pour l’instant) et ses <strong>bases</strong>. <strong>PgAdmin</strong> vas vous demander de vous connecter avec l’utilisateur <strong>postgres</strong>, entrez donc votre mot de passe. Vous arriverez ici&nbsp;(j’ai déployé une partie de l’arborescence) :</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":106,"sizeSlug":"large"} -->
<figure class="wp-block-image size-large"><img src="https://monsieurgis.files.wordpress.com/2020/09/capture17-1.png?w=1024" alt="" class="wp-image-106"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Nous allons alors créer votre identité dans le serveur, parce que ce n’est pas une bonne pratique d’utiliser <strong>postgres</strong>. Cliquez-droit sur «&nbsp;<strong>Login/Group Role</strong>&nbsp;» et aller dans <strong>Create</strong> -&gt; <strong>Login/Group Role…</strong></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Dans l’onglet «&nbsp;<strong>General</strong>&nbsp;» baptisez-vous. Dans l’onglet «&nbsp;<strong>Definition&nbsp;</strong>» vous pouvez attribuer un mot de passe, et gérer l’expiration, ceci sera utile quand vous gérerez des utilisateurs sur votre base. Pour l’instant choisissez juste votre mot de passe.</p>
<!-- /wp:paragraph -->

<!-- wp:jetpack/tiled-gallery {"columnWidths":[[51.03017,48.96983]],"ids":[108,109]} -->
<div class="wp-block-jetpack-tiled-gallery aligncenter is-style-rectangular"><div class="tiled-gallery__gallery"><div class="tiled-gallery__row"><div class="tiled-gallery__col" style="flex-basis:51.03017%"><figure class="tiled-gallery__item"><img alt="" data-height="658" data-id="108" data-link="https://monsieurgis.wordpress.com/capture18-1/" data-url="https://monsieurgis.files.wordpress.com/2020/09/capture18-1.png" data-width="743" src="https://monsieurgis.files.wordpress.com/2020/09/capture18-1.png" data-amp-layout="responsive"/></figure></div><div class="tiled-gallery__col" style="flex-basis:48.96983%"><figure class="tiled-gallery__item"><img alt="" data-height="659" data-id="109" data-link="https://monsieurgis.wordpress.com/capture19/" data-url="https://monsieurgis.files.wordpress.com/2020/09/capture19.png" data-width="714" src="https://monsieurgis.files.wordpress.com/2020/09/capture19.png" data-amp-layout="responsive"/></figure></div></div></div></div>
<!-- /wp:jetpack/tiled-gallery -->

<!-- wp:paragraph -->
<p>L’onglet privilège vous permettra de gérer les droits de vos utilisateurs&nbsp;:</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->
<h4>Can Login?</h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Permet de gérer si un utilisateur peut se connecter à la base, vous utiliserez cette restriction de droit par exemple si vous créez un utilisateur invité permanent, et que vous le prêtez à durer limité à quelqu’un.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->
<h4>Superuser?</h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Un <strong>superuser</strong> à absolument tous les droits d’administration sur le serveur, à utiliser avec parcimonie. Globalement seul vous devriez être <strong>superuser</strong>, ou seulement vos administrateurs de confiance. Le validé, validera tous les autres droits.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->
<h4>Create roles? Create databases?</h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Le premier permet de créer des utilisateurs avec au maximum les mêmes droits que le créateur du rôle, le second des bases de données qui sont au minimum accessible à tous les <strong>superusers</strong>. Par une commande SQL vous pouvez donner ces droits indépendamment.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->
<h4>Update Catalogs?</h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Donnez-le-vous, mais ne le donnez à personne si vous ne savez pas ce qu’il fait.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->
<h4>Inherit rights from the parent roles?</h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Un utilisateur créer avec ce droit aura tous les droits de son créateur, notamment les droits d’accès aux bases de données.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->
<h4>Can initiate streaming replication and backups?</h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Un droit qui permet de lancer les fonctions de <strong>PostgreSQL</strong> de gestion des <strong>backups</strong> et autres joyeusetés.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Si vous créer votre propre utilisateurs, donnez-vous tous les droits (vous êtes chez vous tout de même)</p>
<!-- /wp:paragraph -->

<!-- wp:image {"align":"center","id":111,"sizeSlug":"large"} -->
<figure class="wp-block-image aligncenter size-large"><img src="https://monsieurgis.files.wordpress.com/2020/09/capture20.png?w=708" alt="" class="wp-image-111"/></figure>
<!-- /wp:image -->

<!-- wp:spacer {"height":"30px"} -->
<div style="height:30px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:spacer -->

<!-- wp:paragraph -->
<p>Vous pouvez passer tous les autres onglets, mais jetez un œil à «&nbsp;<strong>SQL</strong>&nbsp;». Celui-ci vous montre la requête en <strong>langage SQL</strong> qui est passé au serveur. Car oui tous ceci peut aussi se faire par une commande. Comme tous ce que l’on va faire par la suite. Cliquez alors sur «&nbsp;<strong>save</strong>&nbsp;».</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Maintenant nous allons créer une connexion à au serveur via <strong>pgAdmin</strong> qui ne passe pas par l’utilisateur <strong>postgres</strong>, mais par votre identifiant fraichement créé. Commencez par vous déconnecter du serveur par un clic droit sur celui-ci «&nbsp;<strong>PostgreSQL 12</strong>&nbsp;» (ou autre chose si vous n’avez pas installer la version 12)</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Vous pouvez alors soit modifier cette connexion au serveur (clic-droit propriété), soit en créer une nouvelle. Je vais pour ma part en créer une nouvelle, cela permet d'avoir toujours une connexion au serveur avec l'utilisateur <strong>postgres</strong> sous la main.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Faite une clic droit sur <strong>servers</strong> -&gt;&nbsp;<strong>Create</strong> -&gt; <strong>Server</strong>&nbsp;:</p>
<!-- /wp:paragraph -->

<!-- wp:image {"align":"center","id":112,"sizeSlug":"large"} -->
<figure class="wp-block-image aligncenter size-large"><img src="https://monsieurgis.files.wordpress.com/2020/09/capture21.png?w=512" alt="" class="wp-image-112"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Nommé votre connexion, puis aller dans l’onglet «&nbsp;<strong>connection</strong>&nbsp;». Ici vous devez préciser l’<strong>IP de l’hôte</strong> de votre serveur, ou <strong>localhost</strong> si le serveur est sur votre PC, le <strong>port de connexion</strong>, le <strong>nom d’utilisateur</strong>, et son <strong>mot de passe</strong>, et vous pouvez sauvegarder celui-ci pour vous faciliter la tâche. Laissé <strong>postgres</strong> pour la «&nbsp;<strong>Maintenance Database</strong>&nbsp;». Vous pouvez faire «&nbsp;<strong>Save</strong>&nbsp;»</p>
<!-- /wp:paragraph -->

<!-- wp:image {"align":"center","id":114,"sizeSlug":"large"} -->
<figure class="wp-block-image aligncenter size-large"><img src="https://monsieurgis.files.wordpress.com/2020/09/capture22.png?w=510" alt="" class="wp-image-114"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Vous êtes ainsi connecté à votre serveur, via votre utilisateur. Vous pouvez maintenant créer une base de données. Une autre bonne pratique, on n’utilise pas la base de données <strong>postgres</strong> si ce n’est pour gérer les extensions.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Faites un clic droit sur «&nbsp;<strong>Databases</strong>&nbsp;» puis «&nbsp;<strong>Create</strong>&nbsp;», nommé votre base et vous avez terminé. Vous pouvez voir la <strong>requête SQL</strong> qui est envoyé au serveur pour créer la base dans l’<strong>onglet SQL</strong>.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Nous avons ainsi terminé l’initialisation de base, plus que quelques réglages et une installation et ce tuto sera terminé.</p>
<!-- /wp:paragraph -->

<!-- wp:heading -->
<h2>Optimisation</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Nous allons voir deux choses maintenant avant d’installer PostGIS, comment optimiser son serveur de données. Il fut un temps ou optimiser son serveur était une vraie plaie, puis des gens ont mis en ligne un outil très pratique <strong><a href="http://pgtune.leopard.in.ua/#/">PG</a><a rel="noreferrer noopener" href="http://pgtune.leopard.in.ua/#/" target="_blank">Tune</a></strong>. Sur le Site vous renseigner les caractéristiques de votre machine, ou de ce que vous souhaitez allouer à <strong>PostgreSQL</strong>, et vous cliquez sur «&nbsp;<strong>generate</strong>&nbsp;».</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":117,"sizeSlug":"large"} -->
<figure class="wp-block-image size-large"><img src="https://monsieurgis.files.wordpress.com/2020/09/capture24.png?w=1024" alt="" class="wp-image-117"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Ensuite vous pouvez soit modifier à la main le fichier <strong>postgresql.conf</strong>, qui se trouve dans le dossier data de votre installation, en recherchant dans celui-ci les paramètres à modifier. Vous pouvez aussi récupérer les commandes SQL qui sont générées sur le site dans l’onglet «&nbsp;<strong>alter system</strong>&nbsp;»…</p>
<!-- /wp:paragraph -->

<!-- wp:image {"align":"left","id":118,"sizeSlug":"large"} -->
<figure class="wp-block-image alignleft size-large"><img src="https://monsieurgis.files.wordpress.com/2020/09/capture25.png?w=442" alt="" class="wp-image-118"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>et les exécuter dans une fenêtre de requête de <strong>pgAdmin </strong>ou encore les exécuter dans un terminal psql. Pour ouvrir une fenêtre de requête dans pgAdmin il suffit de cliquer sur le bouton «<strong>query tool</strong> ».</p>
<!-- /wp:paragraph -->

<!-- wp:spacer {"height":"33px"} -->
<div style="height:33px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:spacer -->

<!-- wp:image {"id":120,"sizeSlug":"large"} -->
<figure class="wp-block-image size-large"><img src="https://monsieurgis.files.wordpress.com/2020/09/capture26.png?w=1024" alt="" class="wp-image-120"/></figure>
<!-- /wp:image -->

<!-- wp:image {"align":"left","id":121,"sizeSlug":"large"} -->
<figure class="wp-block-image alignleft size-large"><img src="https://monsieurgis.files.wordpress.com/2020/09/capture27.png?w=394" alt="" class="wp-image-121"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>On va s’arrêter un instant sur <strong>pgAdmin</strong> tout de même. Dans un premier temps je me suis positionné sur «&nbsp;<strong>MaBase</strong>&nbsp;» dans l’arborescence à gauche, j’ai ensuite cliqué sur le bouton «&nbsp;<strong>Query Tool</strong>&nbsp;» afin d’ouvrir un onglet de requête qui exécutera les commandes passées au sein de «&nbsp;<strong>MaBase</strong>&nbsp;». J’y ai ensuite copié les lignes «&nbsp;<strong>ALTER SYSTEM</strong>&nbsp;» que m’a donné <strong>PGTune</strong>. Il faut ensuite exécuter avec le bouton «&nbsp;<strong>play</strong>&nbsp;» ou avec la touche <strong>F5</strong> chaque commande une par une (en sélectionnant le texte), car les commandes «&nbsp;<strong>ALTER SYSTEM</strong>&nbsp;» ne s’exécute pas en bloc.</p>
<!-- /wp:paragraph -->

<!-- wp:spacer {"height":"32px"} -->
<div style="height:32px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:spacer -->

<!-- wp:paragraph -->
<p>A savoir ces commandes auraient tout aussi bien pu être passé au sein de la base <strong>postgres</strong>.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Il faut ensuite redémarrer votre serveur via le service <strong>postgresql</strong> dans le <strong>gestionnaire de tâches</strong> ou via la commande&nbsp;:</p>
<!-- /wp:paragraph -->

<!-- wp:preformatted -->
<pre class="wp-block-preformatted">pg_ctl restart</pre>
<!-- /wp:preformatted -->

<!-- wp:heading -->
<h2>Installation de PostGIS</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Dernière étape pour faire du SIG dans une base <strong>PostgreSQL</strong>, installer <strong>PostGIS</strong>. Pour ceci rendez-vous sur le site de <a href="https://postgis.net/" target="_blank" rel="noreferrer noopener">postgis.net</a>.</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":123,"sizeSlug":"large"} -->
<figure class="wp-block-image size-large"><img src="https://monsieurgis.files.wordpress.com/2020/09/capture30.png?w=1024" alt="" class="wp-image-123"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Vous y trouverez toutes les information pour l'installation, ils vous conseilleront d’utiliser <strong>StackBuider</strong>, mais comme indiqué en amont celui-ci est capricieux. Vous pouvez donc vous rendre sur les serveur de téléchargement de l’<strong><a rel="noreferrer noopener" href="http://download.osgeo.org/postgis/windows/" target="_blank">OSGeo</a></strong>, afin de récupérer un <strong>setup</strong> correspondant à votre version de <strong>PostgreSQL</strong> à l’adresse suivante : <a rel="noreferrer noopener" href="http://download.osgeo.org/postgis/windows/" target="_blank">download.osgeo.org/postgis/windows/</a></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Ici nous allons télécharger le <strong>setup</strong> pour <strong>PG12</strong>. Télécharger le fichier .<strong>exe</strong> et lancer le. Accepter de donnée femme, enfant et tous vos organes à PostGIS (non c’est juste la licence en fait).</p>
<!-- /wp:paragraph -->

<!-- wp:image {"align":"center","id":124,"sizeSlug":"large"} -->
<figure class="wp-block-image aligncenter size-large"><img src="https://monsieurgis.files.wordpress.com/2020/09/capture31.png?w=499" alt="" class="wp-image-124"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Sélectionné seulement PostGIS</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Et le répertoire d’installation de votre serveur <strong>PostgreSQL</strong></p>
<!-- /wp:paragraph -->

<!-- wp:jetpack/tiled-gallery {"columnWidths":[[50,50]],"ids":[125,126]} -->
<div class="wp-block-jetpack-tiled-gallery aligncenter is-style-rectangular"><div class="tiled-gallery__gallery"><div class="tiled-gallery__row"><div class="tiled-gallery__col" style="flex-basis:50%"><figure class="tiled-gallery__item"><img alt="" data-height="388" data-id="125" data-link="https://monsieurgis.wordpress.com/capture32/" data-url="https://monsieurgis.files.wordpress.com/2020/09/capture32.png" data-width="499" src="https://monsieurgis.files.wordpress.com/2020/09/capture32.png" data-amp-layout="responsive"/></figure></div><div class="tiled-gallery__col" style="flex-basis:50%"><figure class="tiled-gallery__item"><img alt="" data-height="388" data-id="126" data-link="https://monsieurgis.wordpress.com/capture33/" data-url="https://monsieurgis.files.wordpress.com/2020/09/capture33.png" data-width="499" src="https://monsieurgis.files.wordpress.com/2020/09/capture33.png" data-amp-layout="responsive"/></figure></div></div></div></div>
<!-- /wp:jetpack/tiled-gallery -->

<!-- wp:paragraph -->
<p>PostGIS vas alors s’installer dans celui-ci. Il vous demandera s’il peut définir ses propre <strong>variables d’environnements</strong> de <strong>GDAL</strong> si vous n’en avait pas créer. Validez tout ceci. Il souhaitera aussi activer la sortie de raster, validez ceci aussi.</p>
<!-- /wp:paragraph -->

<!-- wp:image {"align":"center","id":129,"sizeSlug":"large"} -->
<figure class="wp-block-image aligncenter size-large"><img src="https://monsieurgis.files.wordpress.com/2020/09/capture35.png?w=499" alt="" class="wp-image-129"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Vous pouvez ensuite cliquer sur «&nbsp;<strong>close</strong>&nbsp;» et <strong>redémarrer</strong> une nouvelle fois votre serveur.</p>
<!-- /wp:paragraph -->

<!-- wp:preformatted -->
<pre id="block-7f7b77d5-414a-4721-ae2b-a6463ac4b002" class="wp-block-preformatted">pg_ctl restart</pre>
<!-- /wp:preformatted -->

<!-- wp:paragraph -->
<p>Dernière étapes, activé l’extension dans votre serveur. Pour cela rien de plus simple il vous suffit de copier les lignes de commandes SQL, que vous trouverez <a rel="noreferrer noopener" href="https://postgis.net/windows_downloads/" target="_blank">ici</a>, dans la fenêtre de requête de pgAdmin.</p>
<!-- /wp:paragraph -->

<!-- wp:preformatted -->
<pre class="wp-block-preformatted">CREATE EXTENSION postgis;
CREATE EXTENSION postgis_raster;
CREATE EXTENSION postgis_sfcgal;
CREATE EXTENSION address_standardizer;
CREATE EXTENSION fuzzystrmatch;
CREATE EXTENSION postgis_topology;
CREATE EXTENSION postgis_tiger_geocoder;
CREATE EXTENSION pgrouting;</pre>
<!-- /wp:preformatted -->

<!-- wp:paragraph -->
<p>Si vous avez fait et que comme moi vous avez installé la <strong>version 13</strong> de <strong>PostgreSQL</strong> vous obtiendrez ceci&nbsp;:</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":132,"sizeSlug":"large"} -->
<figure class="wp-block-image size-large"><img src="https://monsieurgis.files.wordpress.com/2020/09/capture37.png?w=752" alt="" class="wp-image-132"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Et avec une version 12 compatible, avec PostGIS vous obtiendrez ceci :</p>
<!-- /wp:paragraph -->

<!-- wp:image {"id":133,"sizeSlug":"large"} -->
<figure class="wp-block-image size-large"><img src="https://monsieurgis.files.wordpress.com/2020/09/capture38.png?w=667" alt="" class="wp-image-133"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>A savoir, si vous n'avez pas d'installation de <strong>GDAL </strong>vous aurez probablement quelques soucis avec les fonction de raster. Nous verrons donc dans un prochain article l'installation de celui-ci.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Félicitation vous avez désormais une base de données <strong>PostgreSQL</strong> et son extension <strong>PostGIS</strong> opérationnel sur votre ordinateur. Vous trouverez toutes le commandes SQL de <strong>PostgreSQL</strong> <a rel="noreferrer noopener" href="https://www.postgresql.org/docs/12/index.html" target="_blank">ici</a> et pour <strong>PostGIS</strong> <a rel="noreferrer noopener" href="https://postgis.net/docs/manual-3.0/" target="_blank">ici</a>.</p>
<!-- /wp:paragraph -->
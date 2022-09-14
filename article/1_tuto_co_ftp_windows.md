# Tutoriel de connexion à un FTP dans Windows

<!-- wp:paragraph -->
<p>Les <strong>FTP</strong> sont parmi nous, ils sont utilisés au quotidien dans nos relations avec l'IGN. Pour s'y connecter aisément on utilise bien souvent le logiciel <strong>FileZila</strong>. Ce magnifique logiciel à l'interface n'ayant pas bougée d'un iota depuis Windows XP. Il marche très bien, certes, mais il est aussi possible de connecter directement un serveur <strong>FTP</strong> à l'<strong>explorateur de fichier</strong> de Windows. Pratique quand on utilise les même serveurs quotidiennement.</p>
<!-- /wp:paragraph -->

<!-- wp:heading -->
<h2>La démarche de connexion</h2>
<!-- /wp:heading -->

<!-- wp:heading {"level":3} -->
<h3>1ère étape</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Dans un premier temps il vous faut ouvrir l'explorateur de fichier. Ensuite il vous suffit de réaliser un clic droit sur "<strong>Ordinateur</strong>" et choisir l'option "<strong>Ajouter un emplacement réseau</strong>"</p>
<!-- /wp:paragraph -->

<!-- wp:image {"align":"center","id":165,"sizeSlug":"large","linkDestination":"none"} -->
<figure class="wp-block-image aligncenter size-large"><img src="https://monsieurgis.files.wordpress.com/2021/01/1_2.png?w=788" alt="" class="wp-image-165"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Ce qui vous fait arriver sur l'utilitaire d'ajout d'emplacement réseau. Il vous suffit alors de cliquer sur suivant...</p>
<!-- /wp:paragraph -->

<!-- wp:image {"align":"center","id":166,"sizeSlug":"large","linkDestination":"none"} -->
<figure class="wp-block-image aligncenter size-large"><img src="https://monsieurgis.files.wordpress.com/2021/01/2.png?w=595" alt="" class="wp-image-166"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>et de choisir la seul option possible "<strong>Choisissez un emplacement réseau personnalisé</strong>"</p>
<!-- /wp:paragraph -->

<!-- wp:image {"align":"center","id":168,"sizeSlug":"large","linkDestination":"none"} -->
<figure class="wp-block-image aligncenter size-large"><img src="https://monsieurgis.files.wordpress.com/2021/01/3.png?w=595" alt="" class="wp-image-168"/></figure>
<!-- /wp:image -->

<!-- wp:heading {"level":3} -->
<h3>2ème étape</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>Il vous faut ensuite renseigner l'<strong>adresse</strong> <strong>hôte</strong> du serveur FTP... </p>
<!-- /wp:paragraph -->

<!-- wp:image {"align":"center","id":170,"sizeSlug":"large","linkDestination":"none"} -->
<figure class="wp-block-image aligncenter size-large"><img src="https://monsieurgis.files.wordpress.com/2021/01/4.png?w=595" alt="" class="wp-image-170"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>puis à l'étape suivante l'<strong>identifiant</strong>.</p>
<!-- /wp:paragraph -->

<!-- wp:image {"align":"center","id":171,"sizeSlug":"large","linkDestination":"none"} -->
<figure class="wp-block-image aligncenter size-large"><img src="https://monsieurgis.files.wordpress.com/2021/01/5.png?w=595" alt="" class="wp-image-171"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Il ne vous reste plus qu'à valider et ouvrir votre nouvel <strong>emplacement réseau</strong>.</p>
<!-- /wp:paragraph -->

<!-- wp:image {"align":"center","id":173,"sizeSlug":"large","linkDestination":"none"} -->
<figure class="wp-block-image aligncenter size-large"><img src="https://monsieurgis.files.wordpress.com/2021/01/6.png?w=595" alt="" class="wp-image-173"/></figure>
<!-- /wp:image -->

<!-- wp:heading {"level":3} -->
<h3>3ème étape</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>A la première ouverture, le <strong>mot de passe</strong> associé à l'identifiant vas vous être demandé, si la case "<strong>mémoriser les identifiants</strong>" est cochée, ceci ne vous sera plus demandé.</p>
<!-- /wp:paragraph -->

<!-- wp:image {"align":"center","id":175,"sizeSlug":"large","linkDestination":"none"} -->
<figure class="wp-block-image aligncenter size-large"><img src="https://monsieurgis.files.wordpress.com/2021/01/7_2.png?w=482" alt="" class="wp-image-175"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Voilà ! Votre <strong>FTP</strong> est accessible depuis l'explorateur de fichier.</p>
<!-- /wp:paragraph -->

<!-- wp:image {"align":"center","id":177,"sizeSlug":"large","linkDestination":"none"} -->
<figure class="wp-block-image aligncenter size-large"><img src="https://monsieurgis.files.wordpress.com/2021/01/8.png?w=793" alt="" class="wp-image-177"/></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Si vous avez des scrupules en terme de sécurité par rapport à l'enregistrement d'un identifiant et d'un mot de passe, vous pouvez en faire fit ! Dans tous les cas le protocole ftp est une passoire, les identifiants voyagent en claire, car votre ordinateur contacte le serveur hôte via une adresse qui suit ce format : ftp://<strong>identifiant</strong>:<strong>mdp</strong>@<strong>hote</strong></p>
<!-- /wp:paragraph -->

<!-- wp:heading -->
<h2>Quelques informations de connexion à des serveurs FTP ouvert de l'IGN</h2>
<!-- /wp:heading -->

<!-- wp:heading {"level":6} -->
<h6>OrthoHR libre&nbsp;(des dalles d'otho-image à 20cm) :</h6>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li><strong>Hôte</strong>&nbsp;: ftp://ftp3.ign.fr</li><li><strong>Identifiant</strong> : ORTHO_HR_ext</li><li><strong>Mot de passe</strong> : Ithacah6ophai2vo</li></ul>
<!-- /wp:list -->

<!-- wp:heading {"level":6} -->
<h6>BD Carto libre (les fond cartographique de l'IGN, à ne pas confondre avec le scan25*)</h6>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li><strong>Hôte</strong>&nbsp;: ftp://ftp3.ign.fr</li><li><strong>Identifiant</strong> : BD_CARTO_ext</li><li><strong>Mot de passe</strong> : Oor4el8aeM3io0Ji</li></ul>
<!-- /wp:list -->

<!-- wp:heading {"level":6} -->
<h6>BD ALTI libre (des dalles de MNT à 25m) :</h6>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li><strong>Hôte</strong>&nbsp;: ftp://ftp3.ign.fr</li><li><strong>Identifiant</strong>&nbsp;: BD_ALTI_ext</li><li><strong>Mot de passe</strong> : docoazeecoosh1Ai</li></ul>
<!-- /wp:list -->

<!-- wp:heading {"level":6} -->
<h6>RGE ALTI libre (des dalles de MNT à 5m) :</h6>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li><strong>Hôte</strong>&nbsp;: ftp:// ftp3.ign.fr</li><li><strong>Identifiant</strong>&nbsp;: RGE_ALTI_ext</li><li><strong>Mot de passe</strong>&nbsp;: Thae5eerohsei8ve</li></ul>
<!-- /wp:list -->

<!-- wp:paragraph -->
<p>* La fédération française de randonnée refuse que soit diffusé gratuitement le tracé des GR. Du coup le Scan 25 ne peut pas être diffusé car les tracé des chemins comporte l'information "GR#"</p>
<!-- /wp:paragraph -->

[Retour A propos](https://monsieurj42.github.io/index)
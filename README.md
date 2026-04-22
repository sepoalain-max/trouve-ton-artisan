# trouve-ton-artisan
RÉGION AUVERGNE-RHÔNE-ALPES Dossier de projet – 2024/2025
Trouve ton artisan
Plateforme de mise en relation avec les artisans
de la région Auvergne-Rhône-Alpes
Devoir bilan — Formation Développeur Web & Web Mobile
Titre Professionnel RNCP Niveau 5
React.js · Node.js / Express · MySQL / Sequelize · Bootstrap · Sass · Figma
Étudiant(e) : [Votre prénom NOM]
Formateur(trice) : [Nom du formateur]
Trouve ton artisan — Dossier de projet Région Auvergne-Rhône-Alpes
Sommaire
1. Contexte du projet ....................................... 3
1.1 Présentation de l'entreprise .......................... 3
1.2 Expression des besoins ................................ 4
1.3 Contraintes techniques ................................ 4
1.4 Livrables attendus .................................... 5
2. Maquettes Figma .......................................... 6
2.1 Maquette mobile (Mobile First) ........................ 6
2.2 Maquette tablette ..................................... 7
2.3 Maquette bureau ....................................... 7
3. Base de données .......................................... 8
3.1 Modèle Conceptuel de Données (MCD) .................... 8
3.2 Modèle Logique de Données (MLD) ....................... 9
3.3 Modèle Physique – Scripts SQL ......................... 9
4. Sécurité ................................................ 11
4.1 Mesures frontend ..................................... 11
4.2 Mesures backend / API ................................ 12
4.3 Infrastructure ....................................... 13
5. Veille sur les vulnérabilités ........................... 14
6. Liens du projet ......................................... 15
TROUVE TON ARTISAN — 2 —
2024 – 2025
Trouve ton artisan — Dossier de projet Région Auvergne-Rhône-Alpes
1. Contexte du projet
1.1 Présentation de l'entreprise
La région Auvergne-Rhône-Alpes est l'une des plus grandes et des plus dynamiques de France. Elle
couvre 12 départements dans le quart sud-est du pays et dispose d'antennes administratives à Lyon et à
Clermont-Ferrand. C'est avec l'antenne lyonnaise (101 cours Charlemagne, CS 20033, 69269 Lyon Cedex
02) que s'est déroulée la relation client dans le cadre de ce projet.
L'artisanat occupe une place prépondérante dans le tissu économique régional : près d'un tiers des
entreprises de la région sont des entreprises artisanales. On en recensait 221 000 en 2021, faisant
d'Auvergne-Rhône-Alpes l'une des régions les plus artisanales de France. La région souhaite entretenir et
développer cet engouement via la création d'une plateforme numérique dédiée.
■ Coordonnées de l'antenne de Lyon
101 cours Charlemagne – CS 20033 – 69269 LYON CEDEX 02 – France
Tél. : +33 (0)4 26 73 40 00
Site : https://www.auvergnerhonealpes.fr
1.2 Expression des besoins
La région Auvergne-Rhône-Alpes souhaite disposer d'une plateforme web permettant aux particuliers de
trouver facilement un artisan qualifié et de le contacter directement. Les besoins exprimés se structurent
ainsi :
• Référencer les artisans : Afficher les artisans par catégorie (Bâtiment, Services, Fabrication,
Alimentation) avec leurs coordonnées, spécialité, note et localisation.
• Moteur de recherche : Permettre aux utilisateurs de rechercher un artisan par nom depuis le header
du site.
• Fiche artisan complète : Afficher une fiche détaillée avec photo, description, note, site web et un
formulaire de contact.
• Formulaire de contact : Envoyer un e-mail directement à l'artisan (nom, email, objet, message). Une
réponse doit être apportée sous 48h.
• Accessibilité universelle : Le site doit être conforme WCAG 2.1 pour être accessible à tous (seniors,
personnes en situation de handicap…).
• Mobile First & responsive : Le site doit fonctionner de manière optimale sur mobile, tablette et
ordinateur de bureau.
1.3 Contraintes techniques
Le cahier des charges impose une stack technique précise ainsi que des exigences qualitatives strictes :
Couche Technologies imposées
Maquettage Figma (responsive : mobile, tablette, bureau)
TROUVE TON ARTISAN — 3 —
2024 – 2025
Trouve ton artisan — Dossier de projet Région Auvergne-Rhône-Alpes
Frontend React.js + Bootstrap 5 + Sass (Mobile First)
Backend / API Node.js + Express + Sequelize (ORM)
Base de données MySQL (ou MariaDB) – accès exclusif via l'API
Versionning Git + GitHub (repository public ou privé)
IDE Visual Studio Code
Accessibilité Norme WCAG 2.1 (niveau AA minimum)
Hébergement Site déployé et accessible en ligne
Qualité code Code propre, commenté, indenté, validé W3C
1.4 Livrables attendus
À l'issue du projet, les livrables suivants doivent être remis :
✓ Ce dossier PDF structuré (page de garde, sommaire, en-tête/pied de page)
✓ Les maquettes Figma (captures d'écran + lien vers le projet complet)
✓ La présentation de la base de données (MCD, MLD)
✓ La liste des mesures de sécurité mises en place (détaillées)
✓ La description de la veille sur les vulnérabilités de sécurité
✓ Le lien vers le repository GitHub contenant : code source, scripts SQL (.sql), README.md
✓ Le lien vers le site hébergé et accessible en ligne
TROUVE TON ARTISAN — 4 —
2024 – 2025
Trouve ton artisan — Dossier de projet Région Auvergne-Rhône-Alpes
2. Maquettes Figma
Les maquettes ont été réalisées dans Figma en adoptant une approche Mobile First, conformément aux
exigences du cahier des charges. Trois formats ont été déclinés : mobile (375 px), tablette (768 px) et bureau
(1280 px). La charte graphique de la région Auvergne-Rhône-Alpes a été respectée (police Graphik, palette
de couleurs officielle).
Lien vers le projet Figma complet : https://www.figma.com/votre-lien-de-projet
2.1 Maquette mobile (375 px) – Mobile First
[Capture d'écran Figma – Mobile – Page d'accueil]
Hero, guide étapes, artisans du mois, bandeau chiffres clés
→ Lien Figma complet : https://www.figma.com/votre-projet
[Capture d'écran Figma – Mobile – Liste artisans]
Cards en colonne unique, filtres catégories en haut
→ Lien Figma complet : https://www.figma.com/votre-projet
[Capture d'écran Figma – Mobile – Fiche artisan]
Photo, étoiles, formulaire de contact en bas de page
→ Lien Figma complet : https://www.figma.com/votre-projet
[Capture d'écran Figma – Mobile – Page 404]
Illustration SVG + bouton retour accueil
→ Lien Figma complet : https://www.figma.com/votre-projet
2.2 Maquette tablette (768 px)
[Capture d'écran Figma – Tablette – Page d'accueil]
Catégories en grille 2×2, artisans du mois en 2 colonnes
→ Lien Figma complet : https://www.figma.com/votre-projet
TROUVE TON ARTISAN — 5 —
2024 – 2025
Trouve ton artisan — Dossier de projet Région Auvergne-Rhône-Alpes
[Capture d'écran Figma – Tablette – Liste artisans]
Sidebar catégories gauche + grille 2 colonnes
→ Lien Figma complet : https://www.figma.com/votre-projet
[Capture d'écran Figma – Tablette – Fiche artisan]
Colonne principale + sidebar droite informations
→ Lien Figma complet : https://www.figma.com/votre-projet
2.3 Maquette bureau (1280 px)
[Capture d'écran Figma – Bureau – Page d'accueil]
Catégories 4 colonnes, artisans du mois 3 colonnes, hero full-width
→ Lien Figma complet : https://www.figma.com/votre-projet
[Capture d'écran Figma – Bureau – Liste artisans]
Sidebar + grille 3 colonnes, recherche en header
→ Lien Figma complet : https://www.figma.com/votre-projet
[Capture d'écran Figma – Bureau – Fiche artisan]
Layout 2 colonnes 8/4, formulaire contact intégré
→ Lien Figma complet : https://www.figma.com/votre-projet
Note : insérer ici les captures d'écran Figma réelles avant la remise du dossier. Les placeholders ci-dessus indiquent
l'emplacement et le contenu de chaque maquette.
TROUVE TON ARTISAN — 6 —
2024 – 2025
Trouve ton artisan — Dossier de projet Région Auvergne-Rhône-Alpes
3. Base de données
3.1 Modèle Conceptuel de Données (MCD)
Le MCD a été élaboré en notation Merise. Il identifie 3 entités et 2 associations selon les règles de gestion
métier :
• Un artisan apparaît dans une seule spécialité (association 1,1 côté artisan).
• Une spécialité est rattachée à une seule catégorie (association 1,1 côté spécialité).
• Une catégorie regroupe plusieurs spécialités (cardinalité 1,n côté catégorie).
• Une spécialité peut concerner zéro ou plusieurs artisans (cardinalité 0,n).
Entité Attributs Rôle
CATEGORIE
(clé : idCategorie)
nom, slug, icone Niveau supérieur : Bâtiment, Services, Fabrication, Alimentation
SPECIALITE
(clé : idSpecialite)
nom
(+ FK categorie)
Niveau intermédiaire : ex. Plomberie, Coiffure, Poterie…
ARTISAN
(clé : idArtisan)
nom, prenom, email,
telephone, adresse, ville,
codePostal, siteWeb,
apropos, note, photo,
artisanDuMois
(+ FK specialite)
Entité principale référencée sur la plateforme
Tableau 1 – Entités du MCD et leurs attributs principaux
Association Cardinalité CATEGORIE Cardinalité SPECIALITE Cardinalité ARTISAN
regroupe 1,n 1,1 —
exerce — 0,n 1,1
Tableau 2 – Associations et cardinalités Merise
3.2 Modèle Logique de Données (MLD)
La traduction du MCD en MLD donne les 3 relations suivantes :
categorie (id, nom, slug, icone)
specialite (id, nom, #categorie_id)
artisan (id, nom, prenom, email, telephone, adresse, ville, code_postal, site_web,
apropos, note, photo, artisan_du_mois, #specialite_id)
Conventions : souligné = clé primaire (PK) | # = clé étrangère (FK)
3.3 Modèle Physique – Scripts SQL
Deux scripts SQL ont été produits et versionnés dans le repository GitHub :
TROUVE TON ARTISAN — 7 —
2024 – 2025
Trouve ton artisan — Dossier de projet Région Auvergne-Rhône-Alpes
• scripts/create_database.sql — crée la base de données et les 3 tables avec contraintes (clés
primaires, clés étrangères avec ON DELETE RESTRICT, index FULLTEXT sur nom/prenom/ville,
CHECK sur la note et le code postal).
• scripts/seed_database.sql — insère le jeu d'essai complet : 4 catégories, 14 spécialités et 14 artisans
répartis sur toute la région.
Extrait du script de création (table artisan) :
CREATE TABLE artisan (
id INT UNSIGNED NOT NULL AUTO_INCREMENT,
nom VARCHAR(120) NOT NULL,
email VARCHAR(180) NOT NULL UNIQUE,
ville VARCHAR(100) NOT NULL,
code_postal CHAR(5) NOT NULL,
note DECIMAL(3,1) NOT NULL DEFAULT 0.0,
artisan_du_mois TINYINT(1) NOT NULL DEFAULT 0,
specialite_id INT UNSIGNED NOT NULL,
PRIMARY KEY (id),
UNIQUE KEY uq_email (email),
FULLTEXT KEY ft_search (nom, prenom, ville),
FOREIGN KEY (specialite_id) REFERENCES specialite(id)
ON DELETE RESTRICT ON UPDATE CASCADE,
CHECK (note >= 0 AND note <= 5)
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4;
TROUVE TON ARTISAN — 8 —
2024 – 2025
Trouve ton artisan — Dossier de projet Région Auvergne-Rhône-Alpes
4. Sécurité
La sécurité est un axe prioritaire pour les collectivités territoriales. Les mesures suivantes ont été mises en
place sur l'ensemble de la stack (frontend React, API Node.js et configuration serveur).
4.1 Mesures frontend (React)
Mesure Mise en œuvre Intérêt
Validation formulaire
côté client
express-validator dans l'API + validation JS
(regex email, longueur min/max des champs)
avec messages d'erreur ARIA liés aux champs
Empêche l'envoi de données malformées et informe l'u
Protection XSS Échappement automatique de toutes les valeurs
affichées via JSX (React escape par défaut).
.escape() dans express-validator côté API
Empêche l'injection de scripts malveillants dans le DOM
Honeypot anti-spam Champ caché _website dans le formulaire
(visually-hidden, tabIndex=-1).
Rejet si le champ est rempli côté API
Les bots remplissent tous les champs ; le honeypot les
Liens externes sécurisés rel="noopener noreferrer" sur tout lien
ouvrant un nouvel onglet (site web artisan)
Empêche la page externe d'accéder à window.opener
Variables d'environnement URL de l'API dans .env (VITE_API_URL)
Non committé (.gitignore)
Évite d'exposer des URLs internes dans le dépôt public
4.2 Mesures backend / API (Node.js + Express)
Mesure Mise en œuvre Intérêt
Authentification
par clé API
En-tête X-API-Key obligatoire sur toutes
les routes /api/*. Comparaison via
crypto.timingSafeEqual (longueur constante)
Limite l'accès à l'API à la seule application autorisée. L
Helmet.js Positionne automatiquement 11 en-têtes HTTP
(CSP, X-Frame-Options, HSTS, X-Content-Type…)
Protège contre le clickjacking, le sniffing MIME, le cros
CORS strict Origines autorisées listées dans ALLOWED_ORIGINS
(variable d'environnement). Rejet des autres
Empêche des sites tiers de consommer l'API depuis le
Rate limiting 100 req/15 min par IP (général)
10 envois/heure par IP (formulaire contact)
Protège contre le brute-force, le scraping et les attaque
Validation stricte
(express-validator)
Validation + sanitisation de chaque paramètre
(query, param, body) avec messages d'erreur
explicites (HTTP 422)
Prévient l'injection SQL, le XSS et garantit l'intégrité de
Payload limité express.json({ limit: '10kb' }) Protège contre les attaques par payload massif (body b
Logs Morgan Format 'dev' en développement,
'combined' (Apache) en production
Traçabilité des requêtes pour détecter les comporteme
Variables secrets .env pour DB_PASSWORD, API_KEY, MAIL_PASS
Non committé (.gitignore)
Les secrets ne sont jamais exposés dans le code sourc
TROUVE TON ARTISAN — 9 —
2024 – 2025
Trouve ton artisan — Dossier de projet Région Auvergne-Rhône-Alpes
ORM Sequelize Toutes les requêtes SQL passent par Sequelize
(requêtes paramétrées, pas de SQL brut)
Prévient les injections SQL en utilisant systématiqueme
4.3 Infrastructure & configuration serveur
Mesure Mise en œuvre Intérêt
HTTPS / TLS Certificat SSL/TLS via Let's Encrypt
(renouvellement automatique via Certbot)
Chiffre le trafic entre le navigateur et le serveur. Obliga
En-tête HSTS Strict-Transport-Security positionné par Helmet
(max-age=31536000; includeSubDomains)
Force le navigateur à n'utiliser que HTTPS pour ce dom
En-tête CSP Content-Security-Policy limitant les sources
d'assets autorisées (scripts, styles, images)
Empêche le chargement de ressources malveillantes e
Isolation base
de données
MySQL accessible uniquement en localhost
(pas d'accès externe au port 3306)
La BDD n'est pas exposée sur Internet, réduisant drast
TROUVE TON ARTISAN — 10 —
2024 – 2025
Trouve ton artisan — Dossier de projet Région Auvergne-Rhône-Alpes
5. Veille sur les vulnérabilités de sécurité
Une veille active a été menée tout au long du projet sur les vulnérabilités susceptibles d'affecter la stack
technique utilisée (Node.js, Express, React, MySQL, npm). Les sources consultées sont les suivantes :
• CVE (Common Vulnerabilities and Exposures) – https://cve.mitre.org
• OWASP Top 10 2021 – https://owasp.org/Top10
• npm audit – exécuté systématiquement après chaque ajout de dépendance
• Snyk Vulnerability Database – https://security.snyk.io
• GitHub Security Advisories – https://github.com/advisories
• Node.js Security Releases – https://nodejs.org/en/blog/vulnerability
Vulnérabilités identifiées et mesures correctives
Vulnérabilité Description Correction appliquée
OWASP A01
Contrôle d'accès
défaillant
Risque d'accès non autorisé à l'API (lecture des données artisans, spam du formulaire de contact sans authentification Mise en place d'une clé API (X-API-Key) avec comparaison en temps c
OWASP A03
Injection
Injection SQL via les paramètres de recherche (?search=) ou les champs du formulaire de contact Utilisation exclusive de Sequelize (requêtes paramétrées). Validation +
OWASP A05
Mauvaise config.
sécurité
En-têtes HTTP par défaut d'Express exposent la version du serveur (X-Powered-By) et n'activent pas CSP ni HSTS Helmet.js positionne automatiquement les en-têtes de sécurité. X-Pow
OWASP A07
Auth. défaillante
Absence de limite de tentatives sur le formulaire de contact (spam, abus) Rate limiting à 10 envois/heure par IP (express-rate-limit) + honeypot a
CVE-2023-45857
npm : axios
Fuite du header Authorization en cas de redirection cross-origin (axios < 1.6.0) Utilisation de fetch natif (pas d'axios). Si ajout ultérieur, verrouiller axios
Tabnapping Lien vers site web artisan ouvrant un nouvel onglet : la page cible peut accéder à window.opener et rediriger l'onglet pa Ajout systématique de rel="noopener noreferrer" sur tous les liens targ
Tableau 3 – Vulnérabilités identifiées et corrections appliquées
■ Processus de veille continu
npm audit est exécuté à chaque ajout de dépendance. Les alertes GitHub Dependabot sont activées sur le repository
pour détecter automatiquement les nouvelles vulnérabilités dans les dépendances. Une revue manuelle de l'OWASP
Top 10 est effectuée en début et en fin de projet.
TROUVE TON ARTISAN — 11 —
2024 – 2025
Trouve ton artisan — Dossier de projet Région Auvergne-Rhône-Alpes
6. Liens du projet
Ressource Lien / URL
Repository GitHub https://github.com/votre-username/trouve-ton-artisan
Site en ligne (frontend) https://trouve-ton-artisan.votre-domaine.fr
API (endpoint santé) https://api.trouve-ton-artisan.fr/health
Maquettes Figma https://www.figma.com/votre-lien-de-projet
Référence Auvergne-Rhône-Alpes https://www.auvergnerhonealpes.fr
WCAG 2.1 https://www.w3.org/TR/WCAG21/
Validateur W3C HTML https://validator.w3.org
Validateur W3C CSS https://jigsaw.w3.org/css-validator/
Tableau 4 – Liens et ressources du projet
■ Contenu du repository GitHub
• /src — Code source React (frontend)
• /trouve-ton-artisan-api — Code source Node.js/Express (backend)
• /scripts/create_database.sql — Script de création de la BDD
• /scripts/seed_database.sql — Script d'alimentation (jeu d'essai)
• README.md — Prérequis, installation et lancement du projet
Dossier réalisé dans le cadre du titre professionnel Développeur Web & Web Mobile (RNCP Niveau 5) — Région
Auvergne-Rhône-Alpes — 2024 / 2025
TROUVE TON ARTISAN — 12 —
2024 – 2025

# acheter proxy : choisir entre facturation par IP et par Go, vérifier le ciblage et éviter de payer du trafic inutilisé

Personne ne tape « acheter proxy » par curiosité théorique. Il y a presque toujours une tâche derrière : surveiller des pages de résultats, comparer des prix sur une marketplace, faire tourner plusieurs comptes, vérifier une campagne publicitaire depuis un autre pays. Et une question très concrète : combien ça coûte, sur quelle unité on est facturé, et est-ce qu'on peut tester avant de sortir la carte.

Le problème, c'est que le rayon « proxy » est illisible. Certains prestataires affichent « à partir de 2 $/Go » alors que ce tarif ne s'applique qu'au palier de volume le plus élevé. D'autres facturent à l'IP, d'autres au port, d'autres à l'abonnement mensuel. Résultat : on compare des prix qui ne mesurent pas la même chose.

9Proxy est un bon cas d'école parce qu'il ne vend qu'un seul type de ressource — du résidentiel — mais sous deux logiques de facturation opposées. Comprendre cette différence règle à peu près 80 % de la question « quel proxy acheter ».

## Ce qu'on achète vraiment quand on achète un proxy

Trois familles cohabitent sur le marché, et elles ne se font pas bloquer de la même manière :

- **Centre de données** : rapide, bon marché, mais l'IP appartient à un hébergeur. Les sites protégés la repèrent vite.
- **Résidentielle** : l'IP sort d'une connexion domestique réelle, chez un fournisseur d'accès classique. C'est ce que les sites voient comme « un visiteur normal ».
- **Mobile** : l'IP vient d'un réseau opérateur. Le plus difficile à bloquer, et le plus cher.

9Proxy reste sur le résidentiel. La plateforme annonce un pool de plus de 20 millions d'IP dans plus de 90 pays, avec du ciblage par pays, région, ville, code postal et fournisseur d'accès. Côté protocoles, HTTP(S) et SOCKS5 sont pris en charge, et la page d'accueil du prestataire met en avant un taux de disponibilité de 99,95 %.

Ce qu'il faut retenir : vous n'achetez pas « de la vitesse ». Vous achetez une réputation d'IP. C'est ce qui explique l'écart de prix avec un proxy de centre de données, et c'est aussi pourquoi la question de l'unité de facturation devient centrale.

## Par IP ou par Go : la seule décision qui change réellement la facture

Les deux modèles de 9Proxy ne servent pas les mêmes usages, et le choisir à l'envers est la manière la plus rapide de gaspiller son budget.

👉 [Voir les deux modèles de facturation sur 9Proxy](https://bit.ly/9-Proxy)

### Facturation à l'IP : débit illimité, durée de vie limitée

Vous achetez un lot d'IP — 100 minimum. Chaque IP activée donne un débit illimité : vous ne comptez pas les gigaoctets. Les IP non utilisées, elles, n'expirent jamais, ce qui veut dire qu'un lot acheté aujourd'hui reste disponible dans six mois si vous ne l'avez pas consommé.

La contrepartie est technique. Une IP résidentielle vit de quelques heures à environ 24 heures. Elle ne tourne pas automatiquement toute seule : la rotation doit passer par le proxy à rotation automatique, configurable sur des ports choisis. Et surtout, ce modèle impose l'application 9Proxy sur votre machine pour la redirection de port locale. Ce n'est pas un `user:password` à coller dans un script.

### Facturation au Go : endpoints illimités, compteur qui tourne

Le modèle au Go inverse la logique. Vous ne payez pas des IP, vous payez du volume. Le dashboard génère autant d'endpoints que vous voulez, vous ne consommez que les gigaoctets réellement transférés. Sessions au choix : rotation à chaque requête ou session « sticky » qui garde la même sortie pendant la durée configurée. Authentification par identifiant/mot de passe ou par liste blanche d'IP. Tout se fait depuis le navigateur, sans installation.

Deux restrictions à connaître avant d'acheter :

- **180 jours de validité** pour tous les paliers Go standards. Le trafic non consommé est perdu à l'échéance.
- Les paliers Entreprise suppriment cette limite de temps, mais démarrent à 3 000 Go.

### Comment trancher en trente secondes

Posez-vous une seule question : est-ce que la valeur de votre tâche dépend de garder la **même** IP, ou est-ce que vous envoyez un grand nombre de requêtes vers des cibles variées ?

Session à préserver (compte social, panier e-commerce, authentification, plateforme qui surveille la cohérence de connexion) → facturation à l'IP. Trafic large et dispersé (SERP, veille tarifaire, vérification publicitaire, polling d'API) → facturation au Go. Beaucoup d'utilisateurs finissent par prendre un pack combiné, qui mélange les deux sur la même facture.

## Les tarifs 9Proxy après la hausse du 1er juin 2026

9Proxy a annoncé sa première révision tarifaire depuis le lancement, entrée en vigueur le 1er juin 2026. Elle ne touche que les packs à l'IP et les packs combinés. Les paliers au Go sont restés identiques. Les tarifs ci-dessous reflètent la grille après ajustement.

| Modèle | Pack | Prix unitaire | Total | Validité |
| --- | --- | --- | --- | --- |
| Résidentiel par IP | 100 IP | 0,24 $/IP | 24 $ | IP non utilisées sans expiration |
| Résidentiel par IP | 500 IP | 0,144 $/IP | 72 $ | IP non utilisées sans expiration |
| Résidentiel par IP | 1 000 IP + 500 IP offertes | 0,084 $/IP | 126 $ | IP non utilisées sans expiration |
| Résidentiel par IP | 2 500 IP | 0,084 $/IP | 210 $ | IP non utilisées sans expiration |
| Résidentiel par IP | 5 000 IP | 0,072 $/IP | 360 $ | IP non utilisées sans expiration |
| Résidentiel par IP | 15 000 IP | 0,048 $/IP | 720 $ | IP non utilisées sans expiration |
| Résidentiel par IP | 25 000 IP | 0,035 $/IP | 863 $ | IP non utilisées sans expiration |
| Résidentiel par IP | 50 000 IP | 0,029 $/IP | 1 438 $ | IP non utilisées sans expiration |
| Business IP | 100 000 IP | 0,023 $/IP | 2 300 $ | IP non utilisées sans expiration |
| Business IP | 200 000 IP | 0,021 $/IP | 4 140 $ | IP non utilisées sans expiration |
| Business IP | 500 000 IP | 0,018 $/IP | 8 625 $ | IP non utilisées sans expiration |
| Trafic résidentiel (Go) | 5 Go | 3,00 $/Go | 15 $ | 180 jours |
| Trafic résidentiel (Go) | 50 Go + 5 Go offerts | 2,10 $/Go | 105 $ | 180 jours |
| Trafic résidentiel (Go) | 100 Go | 1,50 $/Go | 150 $ | 180 jours |
| Trafic résidentiel (Go) | 200 Go | 1,00 $/Go | 200 $ | 180 jours |
| Trafic résidentiel (Go) | 1 000 Go | 0,80 $/Go | 800 $ | 180 jours |
| Trafic résidentiel (Go) | 2 000 Go | 0,75 $/Go | 1 500 $ | 180 jours |
| Entreprise Go | 3 000 Go | 0,72 $/Go | 2 160 $ | illimitée |
| Entreprise Go | 6 000 Go | 0,70 $/Go | 4 200 $ | illimitée |
| Entreprise Go | 10 000 Go | 0,68 $/Go | 6 800 $ | illimitée |
| Pack combiné | Starter — 100 IP + 5 Go | — | 30 $ | 180 jours (partie Go) |
| Pack combiné | Popular — 1 500 IP + 50 Go | — | 180 $ | 180 jours (partie Go) |
| Pack combiné | Pro — 5 000 IP + 500 Go | — | 720 $ | 180 jours (partie Go) |

👉 [Comparer ces packs et choisir le vôtre](https://bit.ly/9-Proxy)

Un détail qui saute aux yeux dans ce tableau : le prix par Go tombe à 0,68 $ sur le palier Entreprise à 10 000 Go, soit près de 4,4 fois moins que l'entrée de gamme. C'est la structure classique du marché — mais l'écart est ici particulièrement marqué, et il explique pourquoi les pages marketing affichent « à partir de 0,68 $/Go » alors que la majorité des acheteurs paieront entre 1 $ et 3 $/Go. Le 1 000 + 500 IP du côté IP fonctionne sur le même principe : le pack intermédiaire est le seul à embarquer un bonus.

## Ciblage : ce qui est inclus et ce qui ne l'est pas

Le ciblage est souvent l'endroit où les devis explosent chez d'autres prestataires. Chez 9Proxy, la documentation officielle indique un ciblage par pays, État/région, ville, code postal et FAI, accessible directement dans le générateur de proxies. Le mode de session se choisit au même endroit : rotation ou sticky.

Deux points pratiques :

1. Un pool mondial de 20 millions d'IP ne se répartit pas uniformément. Sur un petit marché, vous recyclerez les mêmes sorties plus vite que sur un grand pays.
2. Si votre cible exige une ville précise et que la documentation ne la mentionne pas comme disponible, testez avant d'acheter un gros volume. Le ciblage ville dépend de la profondeur réelle du pool local, pas du menu déroulant.

## Paiement : cartes, crypto, portefeuilles mobiles

9Proxy accepte les cartes bancaires classiques, plusieurs cryptomonnaies (USDT, BTC, ETH, LTC, DOGE et d'autres), ainsi qu'Alipay, Apple Pay et Google Pay. Les comparateurs tiers signalent un bonus automatique de +5 % d'IP pour les paiements en cryptomonnaie — utile si vous détenez déjà des stablecoins, sans intérêt si vous payez par carte.

À noter aussi : le programme partenaire de 9Proxy est présenté comme reversant jusqu'à 15 % de commission et offrant une remise aux utilisateurs parrainés. Concrètement, si vous arrivez par un lien d'invitation, la remise éventuelle est appliquée au moment de la commande — vérifiez le montant affiché dans le récapitulatif avant de valider, plutôt que de vous fier à un pourcentage annoncé ailleurs.

## Essai, remboursement et codes : ce qui existe vraiment

C'est la partie où il faut être précis, parce que beaucoup d'articles promettent des essais gratuits qui n'existent pas.

- **Pas d'essai gratuit standard.** 9Proxy indique proposer un essai limité aux nouveaux utilisateurs, selon les disponibilités, sur demande auprès du support. Précisez si vous voulez tester le modèle IP ou le modèle Go, la réponse dépend de cette information.
- **Politique de remboursement étroite.** Les conditions publiées couvrent essentiellement les IP qui meurent en quelques dizaines de secondes. Ce n'est pas une garantie satisfait ou remboursé.
- **Codes et distributions ponctuelles.** Le prestataire organise régulièrement des distributions de codes donnant 1 Go ou un petit lot d'IP gratuites, généralement sur des forums et communautés affiliées, avec un code par compte. Ça permet de tester la qualité réelle du réseau sans sortir d'argent, à condition de tomber au bon moment.

Autrement dit : considérez votre première commande comme un test payant. Le pack à 15 $ (5 Go) ou le pack de 100 IP à 24 $ servent exactement à ça.

## Équipe, entreprise et revente

Le programme Entreprise débloque trois choses qui n'existent pas sur les paliers standards : une validité de trafic illimitée, un mode équipe (un propriétaire plus jusqu'à cinq membres, avec partage de trafic sans expiration à l'intérieur de l'équipe) et des contrôles par membre avec journal d'activité. Pour une agence qui fait tourner plusieurs clients sur la même facture, c'est la différence entre un compte partagé bricolé et des quotas séparés.

9Proxy propose par ailleurs des conditions revendeur avec tarification de gros. À examiner uniquement si vous revendez déjà du proxy à vos propres clients : cela ajoute une couche de gestion dont vous n'avez pas besoin pour un usage interne.

## Les erreurs qui coûtent le plus cher

1. **Acheter un gros palier Go pour le prix au Go.** À 180 jours de validité, 2 000 Go non consommés représentent 1 500 $ de solde qui disparaît. Le palier optimal est celui que vous consommez réellement, pas celui qui affiche le meilleur tarif unitaire.
2. **Choisir la facturation au Go pour une session à préserver.** Une session sticky n'est pas une IP dédiée : si votre cas d'usage exige de garder la même sortie pendant des heures, le modèle IP est fait pour ça.
3. **Oublier l'application desktop.** Sur le modèle IP, l'absence d'installation bloque purement et simplement l'usage — pas de contournement côté dashboard.
4. **Attendre un abonnement mensuel.** Il n'y en a pas. Vous rechargez un solde, vous ne souscrivez pas un plan.
5. **Comparer des prix au Go entre prestataires sans regarder la validité.** Deux offres à 2 $/Go ne valent pas la même chose si l'une expire en 30 jours et l'autre en 180.

## Acheter, étape par étape

1. Créez le compte via un lien d'invitation, puis validez votre adresse e-mail.
2. Décidez du modèle : packs à l'IP (débit illimité, application requise) ou trafic au Go (dashboard, endpoints illimités).
3. Choisissez le palier le plus petit qui couvre votre charge réelle — 100 IP ou 5 Go suffisent pour juger la qualité du réseau sur vos cibles.
4. Réglez par carte, crypto ou portefeuille mobile, et vérifiez le récapitulatif de commande.
5. Modèle IP : installez l'application, activez vos IP, configurez la rotation si besoin. Modèle Go : passez directement au générateur dans le dashboard et extrayez vos endpoints.

👉 [Créer un compte 9Proxy et choisir votre pack](https://bit.ly/9-Proxy)

## Questions fréquentes

**Peut-on acheter un seul proxy à l'unité ?** Non. Le plus petit pack IP contient 100 IP et le plus petit pack de trafic 5 Go. Il n'y a pas d'achat à l'unité.

**Quelle est la différence concrète entre rotation et sticky ?** En rotation, chaque requête part d'une nouvelle IP. En sticky, la même sortie est conservée pendant la durée de session que vous avez définie. Le choix se fait dans le générateur, pas à l'achat.

**Les IP inutilisées expirent-elles ?** Non, sur le modèle à l'IP le solde non consommé reste disponible. En revanche, une IP activée ne vit que de quelques heures à environ 24 heures.

**Le trafic Go expire-t-il vraiment à 180 jours ?** Oui sur les paliers standards. Les paliers Entreprise à partir de 3 000 Go suppriment cette limite.

**Faut-il une compétence technique particulière ?** Pour le modèle Go, non : le dashboard génère des chaînes de connexion prêtes à copier, avec des exemples de code. Pour le modèle IP, il faut accepter d'installer une application de bureau et de comprendre la redirection de port.

**Le support répond-il ?** 9Proxy annonce un support humain 24/7. Sur un premier achat, c'est surtout utile pour demander l'essai limité ou vérifier une disponibilité de ciblage avant de payer un gros volume.

Le vrai arbitrage, au fond, n'est pas « quel prestataire ». C'est : est-ce que mon usage repose sur des sessions à maintenir ou sur du volume à faire passer ? Répondez à cette question avant de comparer les prix, et vous éviterez d'acheter le mauvais type de pack — ce qui reste, sur ce marché, la dépense la plus facile à regretter.

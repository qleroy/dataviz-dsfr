# Data visualisation et Dashboard DSFR avec cas d’usages tirés de data.gouv

Proposer un outil open-source de data visualisation/BI,
rebrandé avec le Design System de l’Etat,
qui constituera une alternative mature, viable, convaincante à des solutions à la va-vite via Excel comme à des solutions commerciales comme Tableau. 
Nous choisirons un outil open source avec un front exposé dans un navigateur web
permettant de créer des tableaux de bord composés de plusieurs « charts » ou graphiques 
avec la possibilité pour l’utilisateur de créer son dashboard et le mettre en forme via l’interface, i.e. sans coder.
Nous choisirons ensuite des jeux de données ouverts intéressants à explorer
pour faire des cas d’usages convaincants, par exemple des réutilisations de données data.gouv
Le choix de l’outil et un travail de comparaison de l’état de l’art,
des forces et faiblesses des outils open-sources identifiés,
peut déjà constituer une part importante du travail.

Mon expérience m’oriente vers Apache Superset en l’agrémentant du catalogue d’Apache ECharts, la discussion est grande ouverte.

- intérêt commun aux administrations : communiquer des données d'activité, de réponses à une consultation publique ou sondages (questionnaires de satisfaction Service Public+), faciliter la réutilisation des données, faciliter l’exploitation des données, la communication via des données
- répondre à un besoin immédiat et concret : je remarque dans mon administration une barrière à l'entrée trop grande pour utiliser des outils de visualisation, des données non visualisées ne sont pas exploitées
- reposer sur des données et un code source accessibles aux administrations : les projets Apache Superset et Apaches ECharts sont dans le giron de l'Apache Software Foundation. Apache Superset est inscrit dans le SILL.
- La problématique identifiée : certaines administrations (e.g. DGFIP) ont choisi Tableau, d'autres Excel, d'autres n'ont pas d'outil de visualisation à portée de main, un outil/une recommendation interministériel(le) mettrait tout le monde d'accord
- Exemples de cas d’usage : contrôle de gestion, tableaux de bord pour des directrices et directeurs, suivi d'activité d'un département, analyse de résultats de sondage, visualisation et analyse exploratoire de données ouvertes de data.gouv, 
- Les objectifs : démocratiser et faire rayonner  un outil de dataviz/BI open-source et gratuit pour les administrations, faire monter en compétence les agents publics pertinents sur la visualisation de données, développer un outil interministériel de visualisation de données. Proposer un rebranding customisé avec le Système de Design de l’Etat et la possibilité de personnaliser avec un logo de sa direction. Apporter la preuve par l’exemple de l’intérêt, la qualité, la maturité, la fiabilité de l’outil sur des jeux de données disponibles sur data.gouv.fr. Proposer un bouton « Explorer » permettant d’accéder à un tableau de bord pour visualiser les données depuis data.gouv, à la manière de ce que fait le portail de données de la DGFIP. (développer un POC d'intégration de charts du catalogue d'Apache ECharts dans des dashboards Apache Superset)
- Les profils recherchés : développeur Front (javascript), Data Engineer ?

Sources :
DSFR / Charte graphique de l’Etat
- https://www.10pourcent.etalab.gouv.fr/projets/designsystemetat/
- https://www.systeme-de-design.gouv.fr/
- https://www.gouvernement.fr/charte/charte-graphique-les-fondamentaux/introduction
Cas d’usages Services Publics +, Data.gouv et DGFIP
- https://www.plus.transformation.gouv.fr/recherche-de-resultats
- https://www.data.gouv.fr/fr/pages/spd/reference/
- https://www.data.gouv.fr/fr/pages/onboarding/reutilisateurs/
- https://www.data.gouv.fr/fr/datasets/transparence-sur-la-qualite-des-services-publics/https://data.economie.gouv.fr/pages/accueil/ Portail données de la DGFIP
- https://data.economie.gouv.fr/explore/dataset/controle_techn/analyze/?disjunctive.cct_code_dept&disjunctive.cat_vehicule_libelle&disjunctive.cat_energie_libelle&sort=cct_code_dept&dataChart=eyJxdWVyaWVzIjpbeyJjaGFydHMiOlt7InR5cGUiOiJjb2x1bW4iLCJmdW5jIjoiQVZHIiwieUF4aXMiOiJwcml4X3Zpc2l0ZSIsInNjaWVudGlmaWNEaXNwbGF5Ijp0cnVlLCJjb2xvciI6IiMxZjJiNTAifV0sInhBeGlzIjoiY2F0X2VuZXJnaWVfbGliZWxsZSIsIm1heHBvaW50cyI6IiIsInRpbWVzY2FsZSI6IiIsInNvcnQiOiJzZXJpZTEtMSIsInNlcmllc0JyZWFrZG93blRpbWVzY2FsZSI6bnVsbCwiY29uZmlnIjp7ImRhdGFzZXQiOiJjb250cm9sZV90ZWNobiIsIm9wdGlvbnMiOnsiZGlzanVuY3RpdmUuY2N0X2NvZGVfZGVwdCI6dHJ1ZSwiZGlzanVuY3RpdmUuY2F0X3ZlaGljdWxlX2xpYmVsbGUiOnRydWUsImRpc2p1bmN0aXZlLmNhdF9lbmVyZ2llX2xpYmVsbGUiOnRydWUsInNvcnQiOiJjY3RfY29kZV9kZXB0In19fV0sImRpc3BsYXlMZWdlbmQiOnRydWUsImFsaWduTW9udGgiOnRydWUsInRpbWVzY2FsZSI6IiJ9  Exemple d’analyse « in the browser » depuis la plateforme de données de la DGFIP
- https://data.economie.gouv.fr/explore/dataset/prix-carburants-fichier-instantane-test-ods-copie/map/?location=5,46.44217,2.412&basemap=jawg.light Autre exemple avec de la cartographie

Etat de l’art Outils open-source de dataviz
Advocacy for Apache Superset & Apache ECharts
- https://preset.io/blog/apache-superset-vs-tableau/
- https://preset.io/blog/2021-4-1-why-echarts/
- https://docs.preset.io/docs/chart-walkthroughs
- https://github.com/orgs/apache/projects/201/views/1 Project board for Superset 3.0 (pour 2023)
- https://github.com/apache/superset
- https://github.com/apache/echarts
- https://github.com/apache/superset/issues/10418 SIP 50 (Superset Improvement Proposal 50, daté du 24/07/2020)
- https://superset.apache.org/docs/contributing/creating-viz-plugins
- https://preset.io/blog/building-custom-viz-plugins-in-superset-v2/

Exemples ECharts
- https://echarts.apache.org/examples/en/editor.html?c=scatter-aggregate-bar&lang=js Catalogue ECharts
- https://echarts.apache.org/examples/en/editor.html?c=line-race
- https://echarts.apache.org/examples/en/editor.html?c=geo-svg-custom-effect Carte
- https://echarts.apache.org/examples/en/editor.html?c=gauge-temperature
- https://echarts.apache.org/examples/en/editor.html?c=pie-nest Donut


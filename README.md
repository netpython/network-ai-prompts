# Network AI Prompts

**15 prompts complets en français pour administrateurs et ingénieurs réseau.**

Chaque prompt cadre une mission précise avec ses données d’entrée, ses étapes d’analyse, son livrable et un critère de qualité. Les scénarios couvrent le diagnostic, la conception, la sécurité, les changements et l’automatisation.

`15 missions` · `6 catégories` · `Données à renseigner` · `Livrables définis`

## Choisir un prompt

| ID | Mission | Catégorie |
| --- | --- | --- |
| 01 | [Trier un incident réseau en cours](prompts/diagnostic/01-triage-incident.md) | diagnostic |
| 02 | [Diagnostiquer une session BGP ou un préfixe manquant](prompts/diagnostic/02-bgp-routes.md) | diagnostic |
| 03 | [Diagnostiquer OSPF et sa convergence](prompts/diagnostic/03-ospf-convergence.md) | diagnostic |
| 04 | [Tracer une panne VLAN, STP ou EtherChannel](prompts/diagnostic/04-switching-campus.md) | diagnostic |
| 05 | [Analyser un VPN IPsec établi mais inutilisable](prompts/diagnostic/05-vpn-ipsec.md) | diagnostic |
| 06 | [Distinguer une panne DHCP d’une panne DNS](prompts/diagnostic/06-dhcp-dns.md) | diagnostic |
| 07 | [Analyser une lenteur WAN avec des mesures exploitables](prompts/diagnostic/07-performance-wan.md) | diagnostic |
| 08 | [Concevoir une architecture réseau argumentée](prompts/architecture/08-concevoir-architecture.md) | architecture |
| 09 | [Revoir une demande d’ouverture firewall](prompts/securite/09-revue-regle-firewall.md) | securite |
| 10 | [Auditer une configuration avec preuves et priorités](prompts/securite/10-audit-configuration.md) | securite |
| 11 | [Construire un plan de migration et son retour arrière](prompts/changements/11-plan-migration.md) | changements |
| 12 | [Spécifier et développer un programme Python NetOps](prompts/automatisation/12-programme-python-netops.md) | automatisation |
| 13 | [Créer un playbook Ansible réseau exploitable](prompts/automatisation/13-playbook-ansible.md) | automatisation |
| 14 | [Évaluer la capacité et préparer un renouvellement](prompts/exploitation/14-capacite-et-renouvellement.md) | exploitation |
| 15 | [Rédiger un RCA fondé sur les preuves](prompts/exploitation/15-rapport-rca.md) | exploitation |

## Utilisation

1. Ouvre le fichier correspondant à ta mission.
2. Copie son bloc « Prompt prêt à copier » dans ton assistant IA.
3. Remplace les champs comme `{{PLATEFORME_AF}}` par ton contexte ou par « inconnu ».
4. Ajoute les extraits anonymisés pertinents avec leur heure, leur équipement et leur provenance.
5. Examine les conclusions et les commandes avant utilisation, puis fournis les nouvelles observations avec la relance proposée.

Pour une panne encore mal localisée, commence par le [triage incident](prompts/diagnostic/01-triage-incident.md). Pour un besoin déjà cadré, utilise directement le prompt spécialisé.

## Ce que tu trouveras dans chaque fichier

- Une situation d’utilisation concrète.
- Un prompt autonome incluant rôle, contexte, méthode et format de résultat.
- Des emplacements pour les sorties CLI, configurations, mesures ou contraintes.
- Un critère permettant d’évaluer la réponse et une relance pour poursuivre le travail.

## Préparer les données

Utilise des alias cohérents pour les sites et équipements. Si tu remplaces les adresses, conserve les masques, relations de sous-réseau, translations et appartenances VRF utiles au problème. Retire mots de passe, jetons, PSK et clés privées avant de transmettre des extraits.

Les informations techniques conservées doivent respecter les règles de ton organisation et du service IA utilisé. Fournis la version du système et le mode d’exécution des commandes pour permettre une réponse adaptée.

## Statut et évaluation

Ces prompts ont été rédigés pour ce dépôt et relus pour leur couverture technique et leur structure. Leur efficacité dépend du modèle, des données et du contexte. Aucun classement de modèles ou benchmark comparatif n’est revendiqué.

Une réponse satisfaisante cite ses preuves, expose ses inconnues et définit une validation concrète. Pour le code et les playbooks, distingue vérification statique, essai hors ligne et exécution sur un équipement pilote.

Le catalogue et les liens locaux ont été vérifiés. Les résultats produits par une IA restent à contrôler avant application.

## Revue de changement

Avant toute MEP, utilise le [prompt de revue de changement réseau](prompts/exploitation/16-revue-changement.md) pour vérifier les prérequis, risques, contrôles et rollback.

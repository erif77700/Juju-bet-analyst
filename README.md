# JUJU BET ANALYST — version mobile, hébergement Streamlit Cloud

## Important
Cette version est conçue pour être déployée depuis un navigateur de téléphone, sans ordinateur.
Il faut créer des comptes GitHub, Streamlit Community Cloud, OpenAI et Tavily. Les clés API
peuvent générer des frais selon l'utilisation et les forfaits.

## Étape 1 — Extraire le ZIP sur Android
Télécharge le ZIP, puis ouvre **Mes fichiers > Téléchargements** et appuie sur le ZIP pour l'extraire.
Tu dois obtenir `app.py`, `requirements.txt` et `README.md`.

## Étape 2 — Envoyer les trois fichiers sur GitHub
1. Dans Chrome, ouvre https://github.com et crée un compte/connecte-toi.
2. Crée un nouveau dépôt nommé `juju-bet-analyst`.
3. Pour une configuration simple, choisis **Public**. Les clés ne seront PAS placées dans le dépôt.
4. Ouvre le dépôt, puis **Add file > Upload files**.
5. Sélectionne les trois fichiers extraits (pas le ZIP), puis valide avec **Commit changes**.
   Si le sélecteur Android ne permet pas de sélectionner plusieurs fichiers, recommence l'opération
   fichier par fichier. Ne publie jamais tes clés API.

## Étape 3 — Déployer sur Streamlit
1. Ouvre https://share.streamlit.io et connecte-toi avec GitHub.
2. Appuie sur **Create app**.
3. Sélectionne le dépôt `juju-bet-analyst`, la branche `main` et le fichier `app.py`.
4. Dans **Advanced settings > Secrets**, ajoute les deux lignes ci-dessous avec TES clés réelles :

   OPENAI_API_KEY = "ta_cle_openai"
   TAVILY_API_KEY = "ta_cle_tavily"

5. Appuie sur **Deploy** et attends la fin de la construction. L'app recevra une URL en `streamlit.app`.

## Étape 4 — Créer l'icône sur ton Samsung
1. Ouvre l'URL de l'app dans Chrome.
2. Appuie sur le menu ⋮ de Chrome.
3. Choisis **Ajouter à l'écran d'accueil** ou **Installer l'application** si cette option apparaît.
4. Donne-lui le nom JUJU BET ANALYST et confirme.

## Où obtenir les clés
- OpenAI : https://platform.openai.com/api-keys
- Tavily : https://app.tavily.com/

## Dépannage
- Si le déploiement échoue, ouvre les logs de l'app dans Streamlit et lis la première erreur.
- Si l'app indique que les clés manquent, vérifie App settings > Secrets et redémarre l'app.
- Ne partage jamais les clés API et ne les mets jamais dans un fichier GitHub.
- Les résultats web peuvent être incomplets ou contradictoires. Vérifie les sources originales.
- Cette application n'effectue aucun pari et ne garantit aucun résultat sportif.

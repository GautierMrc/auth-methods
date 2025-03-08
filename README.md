





Créer le projet avec Compose : 
composer create-project symfony/skeleton auth-methods


Nettoyer le dossier parent des dossier inutiles
rm -rf public/ var/

Déplacer le projet au bon endroit
mv auth-methods/* .

Déplacer aussi les ficheirs cachés
mv auth-methods/.* .

Vérifier qu'il n'ya plus de fichiers 
ls -al auth-methods/

Supprimer le dossier inutile
rm -rf auth-methods/



Installer git si vous ne l'avez pas : 
apt update && apt install -y git

------------------------------------------

Créer un fichier .gitignore à la racine : 

### Symfony ###
# Logs and cache
/var/
/logs/
/tmp/

# Environment variables and security keys
/.env
/.env.local
/.env.*.local
/.env.test
/.env.test.local

# Ignore secret files
/config/secrets/*.yaml
/config/secrets/**/

# Vendor and dependencies
/vendor/
/node_modules/

# Build and artifacts
/public/build/
/public/uploads/

# IDE and editor settings
/.idea/
/.vscode/
/*.swp
/.project
/.settings
/.buildpath
/.phpunit.result.cache

# Composer files
/composer.lock

# Symfony binary (if used)
/symfony.lock
/.symfony/cache/
/.symfony/var/

# Docker files (if using Docker)
/docker/
/docker-compose.override.yml

# PHPUnit and test artifacts
/phpunit.xml
/phpunit.xml.dist
/tests/_output/
/tests/_support/_generated/
/coverage/
/coverage.xml
/.phpunit.result.cache

# Ignore database files (if using SQLite)
/var/data/*.sqlite
/var/data/*.sqlite-journal

# Ignore CI/CD related files
/.github/
/.gitlab-ci.yml

# Ignore user-specific files
/.DS_Store
/.bash_history
/.npm/


supprimez les anciens ficheirs git s'ils existent :
rm -rf .git

Puis lancer un git init







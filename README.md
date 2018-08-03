# symfony4 tutorial from knpuniversity
#https://knpuniversity.com/screencast/symfony

composer require server
composer require annotations
composer require sec-checker --dev
composer require twig
composer require profiler --dev
composer require debug --dev
composer unpack debug
composer require asset
composer require knplabs/knp-markdown-bundle

./bin/console server:run
./bin/console security:check
./bin/console debug:router
./bin/console debug:autowiring
./bin/console debug:container --show-private
./bin/console debug:container --show-private log
./bin/console debug:config framework
./bin/console config:dump KnpMarkdownBundle
./bin/console config:dump framework
./bin/console cache:pool:clear cache.app
./bin/console cache:warmup
./bin/console cache:clear
./bin/console debug:container --parameters


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
composer require nexylan/slack-bundle php-http/guzzle6-adapter
composer require maker --dev

./bin/console about
./bin/console config:dump framework
./bin/console config:dump KnpMarkdownBundle
./bin/console cache:clear
./bin/console cache:pool:clear cache.app
./bin/console cache:warmup
./bin/console debug:autowiring
./bin/console debug:container --parameters
./bin/console debug:container --show-private
./bin/console debug:container --show-private log
./bin/console debug:container nexy_slack.client
./bin/console debug:config framework
./bin/console debug:router
./bin/console make:command
./bin/console security:check
./bin/console server:run


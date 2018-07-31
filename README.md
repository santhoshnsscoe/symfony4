# symfony4 tutorial from knpuniversity
#https://knpuniversity.com/screencast/symfony

composer require server
./bin/console server:run

composer require annotations

composer require sec-checker --dev
./bin/console security:check

composer require twig

composer require profiler --dev

composer require debug --dev
composer unpack debug

composer require asset

./bin/console debug:router

./bin/console debug:autowiring

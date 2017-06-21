node {
stage "Checkout"
  checkout scm
stage "composer"
  sh 'getcomposer.sh'
  sh 'composer install'
stage "Build"
  sh 'vendor/bin/phpunit'
  sh 'vendor/bin/behat'
}

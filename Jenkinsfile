node {
stage "Checkout"
  checkout scm
stage "Composer"
  sh 'composer install'
stage "Build"
  sh 'bin/vendor/phpunit'
  sh 'bin/vendor/behat'
}

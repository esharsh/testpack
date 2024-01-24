## apicept
api codeception test package

## For version push use below commands
- git tag v1.0.0
- git push origin v1.0.0

## Version : 1.0.0
Description : Create Sample test package with sample test api files.

## Introduction 
api codeception test package

## Instructions

First, install this package:

    composer require esharsh/testpack

Next, copy this code to composer.json file script section

    "scripts": {
       "post-update-cmd": [
            "echo 'Copying directory...'",
            "cp -r ./vendor/esharsh/testpack/src/tests ./tests",
            "echo 'Directory copied successfully.'"
        ]
    },

Hit below command to run the api test

    ./vendor/bin/codecept run -v

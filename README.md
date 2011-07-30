#DRUPAL 7.x Project Cookie Cutter#

this is a repository that can be used for cloning to start a drupal project with my own customized hacks.

## parameters.php ##
Parameters is a definitions file for keeping outside of the repository. This way you can define all sensitive things like passwords and hash salts outside of your repository so they're not available on github. settings.php does an include on parameters.php by a symbolic link to import your definitions into the project at runtime. 

## settings.php ##
The hacks in settings.php are an include  of parameters.php and mostly defining default databases for 4 different environments (prodution, staging, testing and development). The database definitions uses the constants defined in parameters php as the values for the database connections.

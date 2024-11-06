# installing craft manually

this is using composer
`composer create-project craftcms/craft my-craft-project`

`cd my-craft-project`

`cp .env.example.dev .env`

UPDATE the .env with the correct credentials
Create database:
update details to the .env

`composer install`

If you get an error then fix them maybe by installing the required extensions e.g

`sudo apt-get install php8.3-bcmath`

then composer install again if there was an error in composer install

next:
`php craft setup`

follow the instructions !

finally:
`php craft serve`

Go to vender/craftcms/cms/src/helpers/App.php line 1371

comment 1371-1470 and jump to config/project/project.yaml and update to the required version i.e solo,pro,enterprise

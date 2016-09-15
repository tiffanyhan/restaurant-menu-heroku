In order to open the restaurant menus page:

- make sure you have Vagrant and VirtualBox installed on your machine
- navigate to the project directory in your command line
- type the command: 'vagrant init' in order to initialize a Vagrant
  environment
- type the command 'vagrant up' to start the Vagrant environment
- login to the Vagrant machine using the command: 'vagrant ssh'

- navigate back to the project directory within the new
  Vagrant environment using the commands: 'cd /vagrant'
  and 'cd catalog'

- type command 'python finalproject.py'
- in a web browser, navigate to localhost:5000

- creators of restaurants can edit and delete restaurants and
  their menu items by logging in via facebook or google.
  loggin in will give you access to the admin view of the
  restaurant menu pages you are the owner of.

JSON Endpoint Info:

- to see JSON endpoints for all restaurants,
  navigate to localhost:5000/restaurants/JSON
- to see JSON endpoints for a restaurant's menu items,
  navigate to localhost:5000/restaurant/<int:restaurant_id>/menu/JSON
  (you can find each restaurant's id by going to
  localhost:/5000/restaurants/JSON)
- to see JSON endpoints for an individual menu item,
  navigate to localhost:5000/restaurant/<int:restaurant_id>/menu/<int:menu_id>/JSON
  (you can see a menu item's id by going to
  localhost:5000/restaurant/<int:restaurant_id>/menu/JSON)
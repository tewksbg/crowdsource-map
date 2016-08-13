# Crowdsource Map
A nest finder designed for Pokemon Go as it was during the final days of the beta. It's mostly obsolete by now but feel free to fork if you see any use for it. Adapting it to a similar purpose should be as easy as changing some names around and adding different stuff to the database (all hail django). You'll also want to update it for more recent Django versions as it currently only works on 1.9. 

### Technologies
- Google Maps API
- Django 1.9
- Jets.js
- MarkerClusterer
- Bootstrap
- HTML/CSS/Javascript/JQuery/etc

### Getting it to work
1. Create and run a virtualenv.
2. ```pip install -r requirements.txt```
3. Follow the comments in get_data.py to load pokemon into the database. The easiest way to do this is to ```import get_data.py``` from a django shell: ```python manage.py shell```

The script will load all 721 pokemon if you let it so make sure you want that. You'll also have to move the icons folder to /media so the program can find it. It's probably also a good idea to delete all duplicate icons to avoid bloat.

### Usage
Add pokemon to the map by doubleclicking on the map or the little '+' icon at the bottom.

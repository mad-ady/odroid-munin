# odroid-munin
Munin plugins specific for odroid

odroid-temp
![alt tag](http://imgur.com/P85uwW7.png)

odroid-fan

![alt tag](http://imgur.com/6YoAUe6.png)

To enable these extra plugins and fix their dependencies you can do these steps:


    $ sudo apt-get install bc
    $ sudo wget -O /usr/share/munin/plugins/odroid-temp https://raw.githubusercontent.com/mad-ady/odroid-munin/master/odroid-temp
    $ sudo wget -O /usr/share/munin/plugins/odroid-fan https://raw.githubusercontent.com/mad-ady/odroid-munin/master/odroid-fan
    $ sudo chmod a+x  /usr/share/munin/plugins/odroid*
    $ sudo munin-node-configure --shell
    $ sudo ln -s '/usr/share/munin/plugins/odroid-temp' '/etc/munin/plugins/odroid-temp'
    $ sudo ln -s '/usr/share/munin/plugins/odroid-fan' '/etc/munin/plugins/odroid-fan'

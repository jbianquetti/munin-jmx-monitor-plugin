# Munin JXM Monitor Plugin

A simple munin plugin to get the memory values over a jmx connection.

## Build

mvn package

## Execute

> java -jar monitor.jar localhost 9999

## Execute for config output

> java -jar monitor.jar localhost 9999 config


## Use with munin
cp  monitor.jar munin-jmx  /usr/share/munin/plugins 
sudo chmod +x /usr/share/munin/plugins/munin-jmx
cd /etc/munin/plugins
sudo ln -s /usr/share/munin/plugins/munin-jmx munin-jmx


reload munin-node 



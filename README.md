check_folder_min_size
=====================

Nagios minimum folder size plugin


For nrpe you will need to modify nrpe.cfg to check the correct folder etc

Example nrpe.cfg line (will warn under 25GB and be critical under 20GB):
command[check_folder_min_size]=/usr/local/nagios/libexec/check_folder_min_size -f /opt/solr/db/ -s g -w 25 -c 20
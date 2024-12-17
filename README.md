Setup These config First:

If you just want a quick fix for the current session, run the following command on the host machine (not inside the Docker container):
sudo sysctl -w vm.max_map_count=262144

OR

To ensure that Elasticsearch always has the required virtual memory areas after a reboot, add (or update) this line in your system’s /etc/sysctl.conf file:
vm.max_map_count=262144


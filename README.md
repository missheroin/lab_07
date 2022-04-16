# lab_07
A failover cluster of two servers with postgreSQL installed, consisting of a master and a slave. 
Replication is provided, the cluster is created using patrony, and the consul ensures failover of the existing cluster.

1. We save all the files from the repository to ourselves in one folder, open this folder in the terminal and write:
*       vagrant up    
2. We wait until all the machines start up, and write the command to start the consul:
*       ansible-playbook consul.play
3. Ignoring the big error that occurred during the work of the previous command, we wait for the playbook to play and display the result of its work. After that, we enter the commands to launch the playbook, which will work out everything else:
*       ansible-playbook work.yml
4. We are waiting for it to play and enjoy life.

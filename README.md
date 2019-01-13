# esto es un readme

## ejecucion de dos contianers, uno server ldap y el otro el host que esta en la misma red y hace un getent pero con servidor sshd



docker run --rm --name ldap -h ldap --net ldapnet -d robert72004/ldapserver_18roberto

docker run --rm --name samba -h samba --net ldapnet --privileged -it robert72004/hostpam:sshd


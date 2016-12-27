#Ansible profile to install in an Ubuntu

*Packages
* LibreOffice
* Subversion
* Git
* Oracle JDK 1.7 (from tar.gz)
* Oracle JDK 1.8 (from tar.gz)
* Maven 3 (from tar.gz)

*Java
Java 7 JDK and Java 8 JDK tar.gz must be downloaded from Oracle website and placed inside files/java folder
Set the tar.gz filenames in the variables in vars/java.yml

*Roles
These profile depens on 4 roles that you must install beforehand inside roles folder:
* geerlingguy.apache
* cmprescott.chrome
* geerlingguy.mysql
* arknoll.firefox

You can find them in ansible-galaxy and you can install them by executing:
```bash```
ansible-galaxy install geerlingguy.apache -p {path_to_roles_folder}
```

Ìt also contains a vagrant configuration to test the installation
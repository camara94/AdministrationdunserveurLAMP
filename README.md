# Linux : Administration d'un serveur LAMP

Après vous avoir initié à l'administration Linux avec la formation « Installation et administration d'un serveur Linux », Rudi Bruchez vous emmène encore plus loin ! Apprenez à installer et à configurer un serveur web LAMP (Linux, Apache, MySQL et PHP), et à installer un gestionnaire de contenu comme WordPress. Vous pourrez ainsi monter votre propre serveur web sur Linux, en toute simplicité !

## Pour Installer Apache sur le Sur Debian
<code>sudo apt-get install apache2</code>

## Pour manipuler Apache
Après avoir installer apache, voici quelques commandes à connaître pour manipuler son serveur.
### Pour arrêter, demarrer, et redemarer apache
<code>
    <pre>
        sudo apachectl stop ou systemctl stop apache2.service
        sudo apachectl start ou ou systemctl start apache2.service
        sudo apachectl restart ou systemctl restart apache2.service
    </pre>
</code>

### Pour connaitre l'etat du serveur apache
<code>
    <pre>
        sudo apachectl status ou systemctl status apache2.service
    </pre>
</code>
### Pour Voir les processus qui utilisent apache
<code>
    <pre>
        top
        ps -aux | grep apache2
        ps -aux | grep apache[2]
    </pre>
</code>

### Configuration d'apache en Linux
En Linux les fichiers de configurations se trouve dans le dossier **/etc/** et plus particulièrement celui d'apache se trouve dans **/etc/apach2**
<code>
    <pre>
        cd /etc/apache2
        ls -l
    </pre>
</code>
![apache2](1.png)

#### Modification de httpd.conf
Pour modification **httpd.conf**, je crée et copie d'abord son contenu dans le fichier httpd.conf.save avec la commande 
<code>cv httpd.conf httpd.conf.save</code>  

### pour mieux gérer son serveur ubuntu
on va installer etckeeper et logwatch au fait etckeeper, nous permet de versionner l'etat de notre serveur ce qui nous permet de revenir à l'etat precedent à tout moment c'est à dire on pourra faire des commit vraiment c'est outil très pratique
<code>apt install etckeeper</code>
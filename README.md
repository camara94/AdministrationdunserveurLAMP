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

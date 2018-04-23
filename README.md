<h1>docker</h1>

Une documentation de docker est disponible dans le <a href='https://github.com/lekpamartin/docker/wiki'>Wiki</a>

<h2>Vagrant</h2>
Nous avons créé deux vagrantfile pour pouvoir tester une architecture Docker. Nous avons deux fichiers car dans une architecture docker (comme toute architecture en cluster) on a la notion de Maître et d'esclave. 

<br>
Les bonnes pratiques demandent de toujours avoir un nombre impair de maître : plus intéressant pour la gestion du quorum. 

<br>
Il y a plusieurs orchestrateurs qui se partagent le marché mais Kubernetes est de loin le leader. Les nommenclature:
<pre><code>- Kubernetes: intialement développé par Google
- Swarm : développé par Docker. Dans ce dernier on parle de Manager (Maître) et Worker (Esclave)
</code></pre>


<h3>Maître </h3>

<a href='https://github.com/lekpamartin/vagrant/tree/master/vagrantfile/VirtualBox/centos7_docker_master'>vagrantfile</a>

<h3>Esclave </h3>

<a href='https://github.com/lekpamartin/vagrant/tree/master/vagrantfile/VirtualBox/centos7_docker_slave'>vagrantfile</a>

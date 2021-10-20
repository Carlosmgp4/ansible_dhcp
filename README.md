# ansible_dhcp
Creación de un  playbook con ansible que configure de forma automática el servidor, para que haga de servidor DHCP y de router-NAT.
Este playbook esta preparado para lanzarse cobre una maquina virtual de KVM, para que funciones en otras máquinas, se deberia de tocar el fichero group_vars/all.
Para ejecutar el ansible, deberemos ejecutar el comando:

```
   ansible-playbook site.yaml -K
```

Antes de ejecutarlo nos deberemos haber asegurado de cambiar la ip en el fichero hosts y haber puesto la ruta de nuestro par de claves privada. Tambén sobra decir que el par de claves pública deberá estar en la maquina y el usuario con el que vayamos a trabajar debe tener permisos para realizar sudo sin necesidad de contraseña.

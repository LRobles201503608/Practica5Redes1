# Manual de Comandos

## Datos
- Grupo 31

## Comandos de topología 1
### Comandos de EtherSwitch
<strong>conf t:</strong> nos permite acceder a las configuraciones de algun terminal<br>
<strong>vlan #:</strong> nos permite crear una vlan indicandole el número de esta<br>
<strong>name *NOMBRE*:</strong> nos permite crear un nombre para nuestra VLAN <br>
<strong>int f#/#:</strong> nos permite ingresar a alguna de nuestras interfaces donde los # indicaran a que interface nosotros deseamos acceder<br>
<strong>switchport mode trunk:</strong> convierte un puerto de nuestro etherswitch en modo trunk que este nos permite tener limitadas las vlans que nosotros vamos a emplear<br>
<strong>no shu:</strong> Este es el comando que habilita una interfaz.<br>

## Comandos de topología 2

<strong>router eigrp 10:</strong>  Este es encargado de enviar y recibir paquetes EIGRP que contengan datos IP<br>
<strong>network IP</strong><br>
<strong>end:</strong> nos saca de las configuraciones de los terminales
<br>
### Router 3 y 4
<strong>router eigrp 10:</strong>  Este es encargado de enviar y recibir paquetes EIGRP que contengan datos IP<br>
<strong>network IP</strong><br>
<strong>end:</strong> nos saca de las configuraciones de los terminales<br>
<strong>vrrp # *ip*:</strong> elimina el único punto de falla inherente al entorno de ruta predeterminada estática. <br>
<strong>vrrp 10 priority #:</strong> indica la prioridad del router, al no ser una de tipo propietario esta tiene que ser definida con un número inferior a 255<br>
<strong>vrrp 10 preempt:</strong> permite que el enrutador con la prioridad más alta se convierta inmediatamente en el enrutador activo.<br>

### EtherSwitch <br>

<strong>int range f1/0 - 3:</strong> nos permite configurar un rango en especifico de interfaces<br>
<strong>no shut:</strong> Este es el comando que habilita una interfaz.<br>

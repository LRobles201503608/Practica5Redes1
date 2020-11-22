# Manual de Comandos

## Datos
- Grupo 31

## Comandos de topología 1
### Comandos de EtherSwitch
conf t<br>
vlan #<br>
name *NOMBRE*<br>
int f#/#<br>
switchport mode trunk<br>
no shu<br>

## Comandos de topología 2

conf t<br>
router eigrp 10<br>
network IP<br>
end
<br>
### Router 3
conf t<br>
router eigrp 10<br>
network IP<br>
end<br>
conf t<br>
vrrp 10<br>
vrrp 10 ip 192.168.15.3<br>
vrrp 10 priority 120<br>
vrrp 10 preempt<br>
end<br>

### Router 4
conf t<br>
router eigrp 10<br>
network IP<br>
conf t<br>
vrrp 10<br>
vrrp 10 ip 192.168.15.3<br>
vrrp 10 priority 100<br>
end <br>

### EtherSwitch <br>

conf t<br>
int range f1/0 - 3<br>
no shut<br>


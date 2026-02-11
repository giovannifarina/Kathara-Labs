kathara check

kathara vstart -n pc1 --eth 0:A

kathara vclean -n pc1

---

kathara vstart -n pc1 --eth 0:A
	$pc1: ip addr add 192.168.1.1/24 dev eth0
    $pc1: ip link set eth0 up

kathara vstart -n pc2 --eth 0:A
	$pc2: ip addr add 192.168.1.2/24 dev eth0
    $pc2: ip link set eth0 up
    $pc2: ping 192.168.1.1
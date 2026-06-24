# Laboratorio 01 - Subnetting
## Empresa: TechNova
Red base: 192.168.10.0/24

## Departamentos 

| Departamento | Hosts necesarios | Prefijo | Hosts disponibles | Red asignada    |
|--------------|------------------|---------|-------------------|-----------------|
| Ventas       | 50               |   /26   |         62        | 192.168.10.0/26 |
| RH           | 25               |   /27   |         30        | 192.168.10.64/27 |
| TI           | 10               |   /28   |         14        | 192.168.10.96/28 |
|Invitados     | 20               |   /27   |         30        | 192.168.10.112/27 |

Esto es solo para sentar las bases que hare para poder especializarme en redes y si estan viendo es porque les puede servir en conmutacion 

Aqui para adivinar los prefijos y host disponibles se los pondre sencillo con este calculo sin necesidad de un excel aunque si es necesario de ley usaran 32 bits como referencia para mostrar el ejemplo de manera mas facil:

| Cálculo | Bits de host | Total direcciones | Hosts disponibles |
|---|---|---|---|
| 32 - 26 = 6 | 2^6 = 64 | 64 - 2 = 62 | 62 hosts |
| 32 - 27 = 5 | 2^5 = 32 | 32 - 2 = 30 | 30 hosts |
| 32 - 28 = 4 | 2^4 = 16 | 16 - 2 = 14 | 14 hosts |

Creo que con eso no hay necesidad de mas explicaciones, igual haganlo asi en vez de un excel en el mundo laboral lo hacen asi de forma mas rapida investigando.

Dicho esto lo siguiente es "Como sacamos la red asiganada?" sencillo solo hicimos de suma todos los host como viste anteriormente solo sumando los host puros sin restar menos 2.


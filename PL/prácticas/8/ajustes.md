- se escoge el mantenimiento de 8h, +16000€
    - se asume que el SO tiene un MTTR especial de 1h.
- se modifica el sistema operativo y la fuente de alimentación (0.9993965201340558 => 0.9995848299455349)
    - so: ws2012 (web edition) => ws2012 (datacenter edition), +215€
    - fuente: Fuente 1 => Fuente 3, +253€
- se añaden un SAI1 para que la alimentación eléctrica esté por encima de cuatro nueves (0.9995848299455349 => 0.9997583565837516), +140€
- se duplican los ordenadores, se añade un switch a la configuración final, una cabina con los discos RAID y un Hub Fibre Channel, se añade un disco de sistema por ordenador (0.9997583565837516 => 0.9998807502213262)
    - Switch Ethernet 4500 3COM, +290€
    - 2x ST1000DM010 SATA 1TB 7200rpm, +80€
    - 2x Adaptador PCI-FibreChannel, +700€
    - Armario en rack, +780€
    - Hub Fibre Channel, +320€
    - Duplicar ordenadores (sin discos, incl. cambios anteriores), +1162€
    - Fuente de alimentación para la cabina (Fuente 1), +42€
- se mejora la cabina, que es lo que peor disponibilidad tiene (0.9998807502213262 => 0.9999771776899687)
    - se duplica la controladora, +80€
    - se duplica la alimentación, +42€ 
- se revierten algunos cambios anteriores para reducir el presupuesto (0.9999771776899687 => 0.9999568777376259)
    - se revierte el cambio de sistema operativo y PSU, -576€ (nuevo so: enterprise ed.)
    - se elimina la controladora duplicada, -80€
    
- **Disponibilidad final:** 0.9999568777376259 > 0.9999
- **MTTF global:** 183305.70785573302
- **Número de horas de indisponibilidad anuales:** 0.37775h, cerca de 23 minutos anuales de indisponibilidad.

El elemento que más afecta a la disponibilidad del sistema escogido es el clúster de discos, sobre todo después de eliminar la redundancia de la controladora de RAID. Por otro lado, los elementos con mayor disponibilidad son la alimentación eléctrica y los computadores, resultados evidentes tras los importantes cambios realizados.

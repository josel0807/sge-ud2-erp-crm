## 1. Datos
* **Propietario:** josel0807
* **Empresa:** Cadena de restaurantes "El Fogón Casero"
* **Palabra del día:** amistad

---

## 2. Licencias y Modelos

### Diferencias entre Software Libre, Código Abierto y Propietario
* **Software Libre (FSF):** Aquí lo que importa es la ética ,tienes las 4 libertades  puedes usar el programa para lo que te dé la gana, mirar el código para ver cómo está hecho o cambiarlo, pasarle copias a quien quieras y publicar tus arreglos para que otros también los aprovechen.
* **Código Abierto (OSI):** Destaca por lo técnico y el trabajo en equipo. La idea es que si todos podemos ver y tocar el código, el programa avanza más rápido y tiene menos fallos. Tiene que cumplir la OSI (no discriminar a nadie, dejar hacer programas derivados, etc.).
* **Software Propietario:** Es cerrado y le pertenece a la empresa que lo fabrica. Cuando pagas,  estás alquilando el derecho a usarlo . No puedes ver cómo está hecho por dentro, ni modificarlo, ni pasárselo a nadie.

### Por qué "libre" no es lo mismo que "gratis"
Que el código sea libre no significa que montar el sistema te salga gratis. Poner a funcionar algo grande en una empresa cuesta pasta y bastante trabajo por varias cosas:
* Hay que comprar un servidor para instalarlo .
* Adaptarlo a lo que necesita el cliente y configurarlo lleva muchas horas de trabajo técnico.
* Si quieres que se hable con otros programas , tienes que picar código para integrarlo.
* A los empleados hay que enseñarles a usarlo, y necesitas tener a alguien de mantenimiento por si un día se cae todo.

### Versiones Community vs Enterprise y el tema del copyleft
* **El modelo Open Core (Community vs Enterprise):** Odoo es el caso perfecto para entender esto, te dan una versión Community que es libre y no pagas licencias por usuario, pero viene con menos opciones yte tienes que buscar la vida si algo falla. Si quieres los módulos buenos de verdad y tener soporte directo del fabricante, tienes que pagar  la versión "Enterprise".
* **La licencia AGPLv3 (Uso por red):** Esta licencia se la inventaron para cubrir un hueco legal porque habían empresas que pillaban software libre, lo mejoraban y lo montaban en un servidor web cobrando por usarlo, sin compartir sus mejoras. Con la AGPLv3, si montas un servicio web usando ese código y los clientes interactúan por red, estás obligado por ley a liberar el código con todos los cambios que hayas hecho.

---

## 3. Fichas Técnicas

### 3.1. ERP Libre: Odoo Community
* **Licencia exacta:** GNU LGPLv3.
* **Versión actual:** Odoo 18.0.
* **Lenguajes:** Python por detrás (backend) y JavaScript usando el framework OWL para la interfaz.
* **Base de datos:** PostgreSQL (versión 13 para arriba).
* **Cómo se instala:** Lo puedes montar en un servidor tuyo en local o alquilar un VPS en la nube.
* **Módulos clave para nosotros:** TPV para hostelería (sirve para ver el plano de mesas y mandar comandas a cocina), compras, inventario y ventas.
* **Qué máquina pide:** Un servidor Linux , mínimo 2 núcleos, 4 GB de RAM y un disco SSD para que vaya fluido.
* **Fuente:** https://www.odoo.com/documentation/18.0/ (Mirado en septiembre de 2026).

### 3.2. ERP Propietario: Microsoft Dynamics 365 Business Central
* **Licencia exacta:** Propietaria de Microsoft. Tienes que pagar suscripción mensual por cada empleado que lo use.
* **Versión actual:** Dynamics 365 Business Central 2026 Release Wave.
* **Lenguajes:** Lenguaje AL sobre la plataforma .NET Core / C#.
* **Base de datos:** Azure SQL si vas por la nube, o SQL Server si lo montas en local.
* **Cómo se instala:** Está pensado para usarse directamente en la nube de Microsoft (SaaS), aunque te dejan instalarlo en local si quieres.
* **Módulos clave:** Finanzas, control de compras a proveedores, gestión de almacenes y estadísticas con Power BI.
* **Qué máquina pide:** Si vas por la nube, solo un navegador. Si es en local, tienes que tener  Windows Server, SQL Server y mínimo 16 GB de RAM.
* **Fuente:** https://learn.microsoft.com/es-es/dynamics365/business-central/ (Mirado en septiembre de 2026).

### 3.3. CRM Libre: SuiteCRM
* **Licencia exacta:** GNU AGPLv3 .
* **Versión actual:** SuiteCRM 8.10.
* **Lenguajes:** PHP (versión 8.2 o superior) tirando de Symfony para el backend y Angular para que la web se vea moderna.
* **Base de datos:** MariaDB o MySQL.
* **Cómo se instala:** En un servidor web propio  o usando contenedores de Docker que es mas comodo.
* **Módulos clave:** Fichas de clientes, controlar oportunidades de venta, mandar emails masivos y gestionar quejas o incidencias.
* **Qué máquina pide:** Un servidor Linux típico LAMP (Apache, MySQL), con 2 CPUs y 4 GB de RAM va sobrado.
* **Fuente:** https://suitecrm.com/resources/documentation/ (Mirado en septiembre de 2026).

### 3.4. CRM Propietario: Salesforce Sales Cloud
* **Licencia exacta:** Propietaria comercial. Pagas por usuario y mes, y no es barato.
* **Versión actual:** Salesforce Spring/Winter '26.
* **Lenguajes:** Lenguaje Apex (uno suyo propio) y componentes web Lightning en la interfaz.
* **Base de datos:** No la tocas, es la propia base de datos relacional de Salesforce que te gestionan ellos en sus servidores.
* **Cómo se instala:** Es 100% en la nube (SaaS). Nada de servidores propios.
* **Módulos clave:** Gestión a tope de clientes, ver cómo va el embudo de ventas, automatizar tareas y reportes en tiempo real.
* **Qué máquina pide:** Conexión a internet y un navegador web o el móvil, nada más.
* **Fuente:** https://www.salesforce.com/es/products/sales-cloud/ (Mirado en septiembre de 2026).

---

## 4. Fe de Erratas del Tema 2

He estado mirando los apuntes del Tema 2 y hay algunas cosas que se han quedado bastante atrasadas respecto a cómo está el mercado ahora mismo:

1. **Versiones súper antiguas de Odoo y ERPNext:**
   * *En el tema (pág. 6):* Dice que ERPNext va por la 15 y Odoo por la 14.
   * *Ahora mismo:* Ya estamos a finales de 2026, así que Odoo ya va por la **18.0** y ERPNext por la **16**. Montar la versión 14 de Odoo ahora mismo es un atraso, te pierdes el TPV nuevo y rinde peor.
   * *De dónde lo saco:* De sus repositorios oficiales en GitHub.

2. **SuiteCRM cambió entero por dentro:**
   * *En el tema (pág. 8):* Habla de la versión 7.14.5.
   * *Ahora mismo:* La rama 7 ya es historia. Ahora usan la **8.10**, que cambio de manera brutal. Tiraron la base vieja de SugarCRM a la basura y rehicieron el programa entero con Symfony y Angular.
   * *De dónde lo saco:* De los foros y la documentación oficial de SuiteCRM.

3. **El nombre del lenguaje del servidor:**
   * *En el tema (págs. 6 y 7):* Llama al lenguaje `"Phyton"` con la hache después de la P.
   * *Ahora mismo:* Es **Python**, de toda la vida.
   * *De dónde lo saco:* python.org.

---

## 5. Matriz de Decisión y Recomendación Final

### ¿Por qué he puesto estos criterios para El Fogón Casero?
1. **TPV táctil (25%):** Es lo más crítico. Son 5 locales a tope; si el TPV peta y no llegan las comandas a la cocina, se lía .
2. **Centralizar compras (20%):** Lo pide el enunciado. Cada local compra por su lado y la central necesita juntarlo todo para negociar precios con los proveedores.
3. **Integración con delivery (20%):** Quieren que los pedidos web entren solos a cocina para que los camareros no tengan que estar picando los tickets a mano.
4. **Estadísticas de ventas (15%):** Para saber rápido qué platos funcionan y cuáles no se piden nunca.
5. **Coste para 45 trabajadores (10%):** Pagar una licencia mensual por cada camarero en un software propietario tipo Dynamics nos costaría mucho dinero todos los meses.
6. **Facilidad de uso (10%):** En hostelería la gente entra y sale mucho, la pantalla tiene que ser a prueba de tontos para que la pillen el primer día.

### Puntuaciones de la matriz (sobre 10):
* **Odoo Community:** 9,10
* **Microsoft Dynamics 365 Business Central:** 7,10
* **SuiteCRM:** 3,50

### Decisión final: Odoo Community
Para "El Fogón Casero" la mejor opción  es **Odoo Community**. 

Me decanto por este porque ya trae de serie un módulo de TPV pensado para restaurantes, no hay que inventar nada. Te permite montar varias tiendas bajo una central (solucionado lo de agrupar las compras), y al tener una API abierta, se pueden enchufar las apps de Glovo o Just Eat. Pero la razón principal es económica ya que al ser la versión libre, nos ahorramos pagar las 45 licencias mensuales de los camareros.

### Riesgos de montar esto:
* **Inversión inicial:** Nos ahorramos las licencias, pero hay que soltar pasta de golpe para comprar las pantallas táctiles, montar el servidor y pagar a un programador para que nos deje todo configurado a medida.
* **Soporte técnico nulo:** Al no pagarle a Odoo, si el sistema se cae un sábado por la noche búscate la vida. La cadena tendrá que contratar sí o sí un mantenimiento a un informático de la zona para tener las espaldas cubiertas.
* **Quedarte tirado con el informático:** Es difícil. Al estar programado en Python y usar PostgreSQL, es un estándar. Si el técnico nos deja tirados, contratamos a otro y listo.
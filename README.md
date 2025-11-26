📦 Zona Futbolera – Base de Datos MongoDB
Autores:
Alcindo Chavarría, Sergio Velásquez y Bastián Concha
Ingenieros en Informática

📝 Descripción del Proyecto
Este repositorio contiene la base de datos MongoDB utilizada para gestionar el sistema de ventas del proyecto Zona Futbolera, una tienda enfocada en la comercialización de indumentaria, accesorios y artículos deportivos relacionados con el fútbol.

La base de datos incluye colecciones esenciales para el funcionamiento del sistema, tales como ventas, pedidos, productos (catálogo), clientes, inventario y promociones.

📁 Estructura de Colecciones
En la raíz del repositorio se incluyen los siguientes archivos .json, cada uno asociado a una colección de MongoDB:

Tienda_zf_sql.Ventas.json → Colección ventas
Tienda_zf_sql.Promocion.json → Colección promociones
Tienda_zf_sql.Pedido.json → Colección pedidos
Tienda_zf_sql.Inventario.json → Colección inventario
Tienda_zf_sql.Cliente.json → Colección clientes
Tienda_zf_sql.Catalogo.json → Colección catalogo (productos)
Estas colecciones permiten modelar el flujo completo de ventas: desde el cliente y el pedido, hasta la promoción aplicada, el inventario y el registro final de la venta.

🛠️ Tecnologías Utilizadas
MongoDB como base de datos NoSQL.
Archivos JSON para carga y respaldo de colecciones.
Estructura de datos pensada para integrarse con aplicaciones backend y microservicios.
🚀 Uso del Repositorio
Este repositorio puede ser utilizado para:

Importar las colecciones en una base de datos MongoDB de prueba.
Realizar pruebas de servicios backend (consultas, agregaciones, reportes).
Desarrollar aplicaciones de venta, catálogo o gestión de inventario.
Servir como dataset de ejemplo en contextos académicos o de aprendizaje.
💾 Carga de Datos con mongoimport
Asegúrate de tener MongoDB instalado y que los archivos .json estén en la misma carpeta desde donde ejecutarás los comandos.

Ejemplo de importación usando una base de datos llamada zona_futbolera:

# Ventas
mongoimport \
  --db zona_futbolera \
  --collection ventas \
  --file Tienda_zf_sql.Ventas.json \
  --jsonArray

# Promociones
mongoimport \
  --db zona_futbolera \
  --collection promociones \
  --file Tienda_zf_sql.Promocion.json \
  --jsonArray

# Pedidos
mongoimport \
  --db zona_futbolera \
  --collection pedidos \
  --file Tienda_zf_sql.Pedido.json \
  --jsonArray

# Inventario
mongoimport \
  --db zona_futbolera \
  --collection inventario \
  --file Tienda_zf_sql.Inventario.json \
  --jsonArray

# Clientes
mongoimport \
  --db zona_futbolera \
  --collection clientes \
  --file Tienda_zf_sql.Cliente.json \
  --jsonArray

# Catálogo / Productos
mongoimport \
  --db zona_futbolera \
  --collection catalogo \
  --file Tienda_zf_sql.Catalogo.json \
  --jsonArray

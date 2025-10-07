Toma de Requerimientos – Fit Finder (MongoDB) Este documento complementa las Especificaciones de Requisitos del Software del proyecto Fit Finder.

Objetivo del Proyecto Fit Finder busca impulsar una comunidad más saludable mediante la creación de amistades deportivas, la conexión con entrenadores, y motivar a los usuarios con gratificaciones instantaneas como a largo plazo. El sistema permitirá registrar usuarios, crear perfiles, buscar compañeros de entrenamiento y gestionar eventos.
Necesidad del Negocio El cliente presenta la idea de crear un sitio web que impulse las relaciones personales a través de un ambito deportivo.
Situación Actual En la actualidad no existen incentivos instantaneos al realizar actividades fisicas
Usuarios del Sistema Usuarios principales: Personas mayores de 18 años interesadas en actividades deportivas. Usuarios secundarios: Entrenadores deportivos. Administrador: encargado de moderar contenido y gestionar reportes.
Tareas por Tipo de Usuario Usuario default: Crear y personalizar perfil, buscar compañeros, enviar mensajes. Usuario entrenador: Crear y personalizar perfil professional, validar certificaciones, comunicarse con deportistas. Administrador: Revisa reportes, bloquear usuarios, gestiona tipo de errores, responde a reportes. Invitado: Tiene visión limitada de la web y los usuarios registrados.
Datos a Almacenar (MongoDB) El sistema utilizará colecciones para organizar la información:
• usuarios: nombre, correo, contraseña, edad, ciudad, intereses, tipo_usuario • entrenadores: id_usuario, especialidad, certificaciones, calificación • eventos: nombre, fecha, ubicación, descripción, creador_id • mensajes: emisor_id, receptor_id, contenido, fecha_envío 7. Funciones Principales • Registro e inicio de sesión. • Creación y edición de perfiles. • Búsqueda de compañeros de entrenamiento. • Chat interno entre usuarios. • Calendario de eventos deportivos. • Reporte y bloqueo de usuarios. 8. MVP – Mínimo Producto Viable • Register y login de usuarios. • Visualizar usuarios registrados en la web. • Chat con mensajes predeterminados en la web. 9. Restricciones Técnicas • Backend en Node.js. • Base de datos MongoDB. • Diseño responsivo (desktop y móvil). • Seguridad HTTPS y cifrado de contraseñas. 10. Fases o Prioridades

Diseño
Backend
Base de datos
Pruebas
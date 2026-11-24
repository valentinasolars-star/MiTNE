# TNE Digital — prototipo educativo

## Abrir
1. Extrae el ZIP completo.
2. Abre `index.html` en Chrome, Edge o Firefox. No muevas los archivos por separado.
3. Si el navegador restringe el almacenamiento de archivos locales, abre la carpeta con VS Code y usa Live Server, o ejecuta `python -m http.server 8000` desde la carpeta y visita `http://localhost:8000`.

No requiere dependencias, base de datos, internet ni servicios externos. El servidor local es opcional y solo sirve archivos estáticos.

## Prueba sugerida
- Registra una cuenta ficticia con una contraseña de al menos 8 caracteres.
- Activa las verificaciones simuladas o continúa al inicio. Saldo inicial de prueba: $5.000.
- Recarga $2.000 eligiendo resultado aprobado. Saldo esperado: $7.000.
- Repite con resultado rechazado: el saldo no cambia.
- Valida un pasaje Metro ($260 ficticios): saldo esperado $6.740. Comprueba el historial y sus filtros.
- Edita perfil, cambia preferencias de notificaciones, abre beneficios y la pantalla animada de construcción.
- Cierra sesión, entra con la misma cuenta y comprueba que el saldo y los movimientos permanecen.
- Para recuperar la contraseña de prueba, usa el código 123456 (sin envío de correo).

## Archivos
- index.html: documento principal.
- style.css: diseño responsive, animaciones y navegación.
- app.js: cuentas locales, lógica, pagos y pantallas.
- assets/: mascotas.
- referencias/: las 21 imágenes originales del ZIP.

## Límites
Prototipo no oficial. Utiliza datos ficticios. LocalStorage persiste solo en el navegador/origen actual y se puede modificar o borrar. La verificación de contraseña local no constituye autenticación segura para producción. El QR es una representación visual, no es escaneable. Biometría, documentos, beneficios, soporte y operaciones de transporte no se conectan a sistemas reales. El chat y los detalles de beneficios llevan a la pantalla de construcción. Los términos y la política se muestran como referencias gráficas originales, no como documentos legales validados. La tarifa de $260 y el saldo inicial se eligieron para la demostración.

Validación realizada: comprobación sintáctica de JavaScript con Node.js. La prueba automatizada con Chromium quedó bloqueada por las políticas del entorno de ejecución, por lo que los flujos interactivos deben comprobarse en el navegador del usuario.

# BeachTrip
Aplicación web estática en JavaScript + Supabase. No requiere npm. Los importes se almacenan en céntimos. El reparto distribuye los céntimos sobrantes sin perder dinero.

## Configuración
1. Crea un proyecto nuevo en https://supabase.com/dashboard (no uses la base de tu otra aplicación).
2. Abre SQL Editor, pega schema.sql completo y ejecútalo una sola vez en el proyecto nuevo.
3. En Connect o Settings > API Keys, copia la URL del proyecto y la clave pública publishable (o anon). Pégalas en config.js. Nunca uses service_role ni una clave secreta.
4. Sube todos los archivos a un repositorio GitHub. Settings > Pages > Deploy from a branch > main > /root. Abre la URL publicada.
5. En Supabase Authentication > URL Configuration configura Site URL con la URL publicada y permite el registro por correo. Confirma los correos si está habilitada esa opción.
6. Crea tu cuenta y viaje. En Amigos copia el código de invitación. Cada amigo crea su cuenta y usa ese código para unirse. Espera a que todos se unan antes de registrar compras que correspondan a todo el grupo.

## Prueba de aceptación
Con dos cuentas distintas verifica que ambas vean el mismo viaje y una tercera cuenta sin invitación no pueda acceder. Registra S/100 con ocho participantes: cada uno debe S/12.50 y el comprador recibe S/87.50. Comprueba la boleta desde otra cuenta, registra un pago y revisa el saldo. Prueba la lista compartida y la actualización en tiempo real. El sistema registra pagos declarados, no ejecuta ni verifica transferencias bancarias. No se ha probado contra un proyecto Supabase real. Requiere internet; no admite operaciones offline. En Android usa Instalar aplicación y en iPhone Safari > Compartir > Añadir a pantalla de inicio.

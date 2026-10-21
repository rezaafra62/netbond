# Ayuda de NetBond — versión 1.4.3

## ¿Qué es NetBond?
NetBond suma las conexiones que ya tiene (WiFi + Ethernet + módem) en el
mismo equipo Windows: sin servidor, sin VPS, sin nube. El resultado es una
«superlínea» local por la que viajan sus descargas y programas.

## Inicio rápido
1. Descomprima y ejecute `netbond.exe` (o `netbond run`).
2. El modo por defecto es el proxy local; los programas que respetan el
   proxy del sistema (navegadores, muchos gestores) entran solos al bond.
3. Para cobertura total active el «modo transparente» en Ajustes: todos los
   programas entran sin configuración manual.
4. En IDM: Options → Proxy/Socks → Get System, o apunte a 127.0.0.1:8888.

## Pestaña de enlaces: marcar y dirigir
- Columna «✓»: marque tantos enlaces como quiera.
- «Dirigir enlaces marcados a programas…» abre la hoja desplegable frente a
  la tabla: envíe la SUMA de los enlaces marcados a uno o varios programas;
  «+» abre el selector de programas instalados.
- Clic en la columna del NOMBRE del enlace: hoja individual de ese enlace.
- Última columna: sube/baja la prioridad del enlace.

## Descargas y división paralela
- Las descargas grandes (HTTP y HTTPS) se dividen en paralelo entre los
  enlaces sanos, al estilo IDM pero entre sus propios internetes.
- Si un enlace muere, la transferencia continúa desde el mismo byte con
  peticiones Range (hasta tres saltos).
- El tráfico vivo sensible a latencia queda en el enlace de menor RTT.

## Seguridad y privacidad
- Todo ocurre en su equipo; sin nube ni terceros en el cable.
- La inspección TLS (para el failover HTTPS sin cortes) se activa solo con
  su consentimiento explícito; la clave CA local se sella con DPAPI de
  Windows y nunca sale del equipo.
- NetBond nunca corta su conectividad: si algo falla, el tráfico sigue por
  la vía normal (fail-open por diseño).

## La edición de prueba de 48 horas
- En la primera ejecución se sella la huella de la máquina y aparece una
  cuenta regresiva en la barra de título; tras 48 horas el programa se
  niega a ejecutarse, sin excepciones.
- Retroceder el reloj del sistema la expira; copiar el sello a otro equipo
  no sirve de nada.

## Solución rápida de problemas
- «Aún no hay enlaces»: no hay adaptadores activos; conecte una tarjeta.
- Descargas de IDM invisibles: ponga el proxy de IDM en Get System.
- Dos adaptadores en la misma subred: doctor muestra un aviso ámbar; mueva
  uno a otra subred.
- Comandos CLI: links, probe, run, stats, bench, get, doctor, config,
  win-proxy, win-service, help.

## Idiomas de la ayuda
Esta ayuda viaja dentro del programa en persa, inglés, español y árabe;
cámbiela desde la barra superior de esta ventana.

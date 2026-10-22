# Aplicación de Capitalista Rebelde

Interfaz de ahorro curado, perfil de ahorrador y panel de gobernanza. Un solo archivo, sin dependencias externas.

## Publicar

1. Sube `index.html` a la raíz de este repositorio.
2. Settings → Pages → Source: `main` / `root`.
3. Settings → Pages → Custom domain: `app.capitalistarebelde.xyz`.
4. En tu DNS, crea un registro CNAME de `app` apuntando a `capitalista-rebelde.github.io`.

## Clave de RPC

La aplicación funciona sin clave propia: usa RPC públicos (publicnode, llamarpc, Cloudflare, drpc).

Para usar una línea dedicada, añade antes del script principal:

```html
<script>window.CR_RPC_KEY = 'tu-key-aqui';</script>
```

**La clave tiene que estar restringida por dominio en el panel de Alchemy.** En una aplicación de navegador es imposible ocultar una clave: cualquiera puede leerla en el código fuente. Lo que la protege no es esconderla, es que solo funcione desde tu dominio. Alchemy lo configura en Apps → tu app → Security → Allowed domains.

Nunca subas una clave sin esa restricción.

## Reglas de producto que esta interfaz respeta

1. Ninguna dirección de contrato sin verificar en fuente oficial.
2. Ninguna proyección presentada como garantía; siempre se muestra el escenario adverso.
3. Sin botón de retirar en donaciones irreversibles.
4. Si un dato externo falla, se marca como no verificado; nunca se inventa.

Ver [reglas de producto](https://github.com/Capitalista-Rebelde/Capitalista-Rebelde/blob/main/docs/reglas-producto.md).

## Aviso

Parámetros económicos de prueba, pendientes de validación legal. Nada aquí es asesoramiento financiero. Los rendimientos no están garantizados.

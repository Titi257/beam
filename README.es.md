<div align="center">

<img src="beam-icon.png" width="128" alt="Beam"/>

# Beam

[🇬🇧 English](README.md) · [🇫🇷 Français](README.fr.md) · **🇪🇸 Español**

Compartir pantalla y control remoto nativo para macOS — de Mac a Mac, rápido.

[**⬇︎ Descargar Beam.dmg**](https://github.com/Titi257/beam/releases/latest/download/Beam.dmg)

</div>

---

Ver y **controlar** otro Mac (ratón + teclado), en red local o por Internet, cifrado de extremo a extremo. App **universal** (Intel + Apple Silicon).

- **Tres modos de conexión, elegidos automáticamente — nada que configurar:**
  - **Red local (LAN)**: dos Macs en la misma red se conectan **directamente**, sin servidor, mínima latencia.
  - **Directo (P2P)**: por Internet, Beam intenta un enlace directo de igual a igual para evitar el relé cuando la red lo permite.
  - **Relé (Internet)**: si no, el tráfico pasa por el relé **más cercano** (multirregión) — funciona detrás de cualquier router, en cualquier lugar.
- Conéctate desde cualquier lugar por **ID** — sin IP ni dirección de servidor que escribir.
- **Control remoto completo** (ratón + teclado), o **modo solo lectura** (ver sin controlar).
- **Emparejamiento estilo AnyDesk**: «Compartir mi pantalla» da un **ID de 9 cifras** estable por equipo; el otro Mac lo introduce.
- **Cifrado de extremo a extremo** (X25519 ECDH + AES-GCM) — ni la red local ni el relé ven nada más que texto cifrado. Un **código de seguridad** mostrado en ambos lados puede compararse en voz alta para detectar un ataque de intermediario activo (MITM).
- **Portapapeles compartido** (texto + imagen) e **indicador de calidad** en vivo (FPS, tasa de datos, latencia, directo vs relé).
- **Actualizaciones automáticas** integradas.

## Requisitos

- **macOS 14 (Sonoma) o posterior.**
- **Mac Intel o Apple Silicon** — universal, nativo en ambos.

## Instalación

1. Descarga **`Beam.dmg`** desde la [última versión](https://github.com/Titi257/beam/releases/latest).
2. Ábrelo y arrastra **Beam** a **Aplicaciones**.
3. Inicia **Beam** desde Aplicaciones.

> La app está firmada y notarizada por Apple — sin aviso de «desarrollador no identificado».

## Uso

En la única ventana:

- **Compartir mi pantalla** → obtienes un **ID**. Dáselo a quien deba ver tu pantalla. Al conectar aparece un aviso **Aceptar / Rechazar**; aceptar concede el control de teclado/ratón (salvo en **solo lectura**).
- **Controlar otro Mac** → escribe el **ID** del otro Mac y pulsa **Conectar**.

**Nada que configurar**: Beam se conecta directamente en tu red local cuando es posible y, si no, usa su relé integrado automáticamente (eligiendo el más cercano). Una dirección de relé está en una sección **avanzada** opcional que normalmente nunca necesitas tocar.

En el primer uso, macOS pide **Grabación de pantalla**, **Accesibilidad** y (modo LAN) **Red local** — solo al lado que lo necesita.

## Actualizaciones

Beam busca actualizaciones automáticamente y ofrece **App ▸ Buscar actualizaciones…**. Cada actualización está firmada criptográficamente y se verifica antes de instalarse.

## Privacidad y seguridad

El contenido está **siempre cifrado de extremo a extremo**. El relé (modo Internet) solo ve texto cifrado. El código ha sido **revisado en cuanto a seguridad** (límites de tamaño de trama, verificación de clave reforzada), pero **sin una auditoría formal independiente** — úsalo en consecuencia.

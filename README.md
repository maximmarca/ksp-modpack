# KSP Modpack — Maxi & Fer

Pack de mods para jugar **Kerbal Space Program 1.12.5** en multijugador con DarkMultiPlayer.

Incluye: cliente multijugador + mejoras visuales + planetas nuevos + propulsión interestelar + herramientas de career + contratos.

**Server en modo CAREER**: progresión completa con ciencia, fondos y contratos.

## ✅ Instalación recomendada (con CKAN)

Es la forma más fácil y segura — CKAN descarga e instala todo, con las versiones exactas.

1. Descargá **CKAN**: https://github.com/KSP-CKAN/CKAN/releases/latest → archivo `ckan.exe`
2. Abrilo. La primera vez te pide la carpeta de KSP → apuntá a tu instalación 1.12.5.
3. Bajá de este repo el archivo **`MaxiFer-Modpack.ckan`** (botón `Code` → `Download ZIP`, o clic en el archivo → `Download raw`).
4. En CKAN: menú **File → Install from .ckan file…** → elegí `MaxiFer-Modpack.ckan`.
5. **Apply changes**. CKAN baja e instala todo (son ~9 GB con las texturas, tardá).

Listo. Todos los jugadores instalan **el mismo `.ckan`** → versiones idénticas (obligatorio para el multiplayer).

## Mods incluidos

### Multiplayer
| Mod | Para qué |
|-----|----------|
| DarkMultiPlayer v0.3.8.5 | Cliente multijugador |

### Visuales
| Mod | Para qué |
|-----|----------|
| Spectra | Nubes, atmósferas (EVE + Scatterer config) |
| Scatterer | Atmósferas físicamente realistas |
| Parallax Continued (+ texturas) | Terreno 3D con relieve y vegetación |
| Stock Waterfall Effects | Plumas de motor realistas |
| Distant Object Enhancement | Planetas/naves visibles a distancia |
| TUFX | Post-procesado visual |

### Planetas y propulsión
| Mod | Para qué |
|-----|----------|
| Outer Planets Mod | Planetas nuevos más allá de Jool |
| Near Future Propulsion | Motores iónicos / plasma |
| Near Future Electrical | Reactores nucleares |
| Far Future Technologies | Fusión, antimateria, propulsión interestelar |

### Quality of life (career)
| Mod | Para qué |
|-----|----------|
| Kerbal Engineer Redux | Lee Δv, TWR, parámetros orbitales en vuelo y en VAB |
| Kerbal Alarm Clock | Alarmas para maniobras, encuentros, ventanas |
| Transfer Window Planner | Calcula ventanas de transferencia interplanetarias |
| [x] Science! Continued | Gestor de experimentos por bioma |
| Docking Port Alignment Indicator | Indicador visual para acoplamientos |
| Editor Extensions Redux | Mejoras VAB/SPH (simetría, snap, mirror) |

### EVA / bases
| Mod | Para qué |
|-----|----------|
| KAS (Kerbal Attachment System) | Cuerdas, tuberías, conectores entre naves |
| KIS (Kerbal Inventory System) | Inventarios EVA, construcción en órbita/superficie |

### Contratos (career)
| Mod | Para qué |
|-----|----------|
| Contract Configurator | Framework para los packs siguientes |
| Contract Pack: Tourism Plus | 15 contratos de turistas |
| Contract Pack: Bases and Stations Reborn | Construir bases planetarias y estaciones orbitales |
| Contract Pack: Field Research | Misiones de ciencia en sitios específicos |
| Contract Pack: Exploration Plus | Sobrevuelos y aterrizajes en cuerpos celestes |
| Contract Pack: Anomaly Surveyor | Explorar anomalías (Monoliths, Face on Duna, etc.) |

CKAN agrega solo todas las dependencias (Module Manager, Kopernicus, Community Tech Tree, Community Resource Pack, etc.).

## Conectarse al server

KSP → botón **DMP** → **Add Server**. La dirección y el puerto te los pasa Maxi por privado.
El **player name** tiene que ser exactamente el que esté en la whitelist del server.

## Opción B — instalar el cliente DMP a mano (sin CKAN)

En `GameData/DarkMultiPlayer/` está el cliente DMP v0.3.8.5 suelto, por si querés solo
el multijugador sin el resto de los mods: copiá esa carpeta dentro del `GameData` de tu KSP.

## Agregar mods nuevos (para el que mantiene el pack)

1. Instalá el mod nuevo con CKAN.
2. Agregá su identificador a la lista `depends` de `MaxiFer-Modpack.ckan`.
3. Commit + push. Los demás vuelven a instalar el `.ckan`.

# KSP Modpack — Maxi & Fer

Pack de mods para jugar **Kerbal Space Program 1.12.5** en multijugador con **LunaMultiplayer** (LMP).

Incluye: cliente multijugador + mejoras visuales + planetas nuevos + propulsión interestelar + herramientas de career + contratos.

**Server en modo CAREER compartido**: progresión única — ciencia, fondos, árbol tecnológico y contratos se sincronizan entre los jugadores. Lo que cumple uno, suma para los dos.

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
| LunaMultiplayer v0.29.2 | Cliente multijugador con carrera compartida |
| Harmony2 | Dependencia de LMP (patching runtime) |

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

KSP → menú principal aparece el botón **LMP** → **Add Server**.

La dirección, el puerto y la contraseña te los pasa Maxi por privado. Como referencia general:
- **Address**: `maxi-ksp.duckdns.org`
- **Port**: `8800` (UDP — LMP cambió respecto a DMP)
- **Password**: te la pasa Maxi
- **Player name**: el que acuerdes con Maxi (acordarlo antes para evitar conflictos)

## Agregar mods nuevos (para el que mantiene el pack)

1. Instalá el mod nuevo con CKAN.
2. Agregá su identificador a la lista `depends` de `MaxiFer-Modpack.ckan`.
3. Commit + push. Los demás vuelven a instalar el `.ckan`.

## Historia del pack

- **v1.0** (2026-05-21): primer release con DarkMultiPlayer + visuales + planetas + propulsión.
- **v2.0** (2026-05-23): server pasado a CAREER, agregados QoL (KER, KAC, TWP, etc.), KAS/KIS y 6 Contract Packs.
- **v3.0** (2026-05-23): migración de DarkMultiPlayer a **LunaMultiplayer** — career compartida real entre jugadores. Cambio de puerto a 8800/UDP.

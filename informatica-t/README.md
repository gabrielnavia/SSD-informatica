# Taller SDD y Prompt Engineering — Controller y Router SDN

Informática para Telecomunicaciones · Universidad del Cauca · 2026-2

Simulación SDN a nivel de aplicación: dos aplicaciones Python independientes (FastAPI) que se comunican por REST/JSON. El **Controller** administra la topología y calcula rutas con Dijkstra; el **Router** pide la ruta al Controller y simula el reenvío de paquetes. Ambas implementan MVC y DAO.

| Integrante | Rol principal |
|---|---|
| _Nombre del estudiante A_ | Estudiante A — SDN Controller |
| _Nombre del estudiante B_ | Estudiante B — SDN Router |

## Dónde está cada entregable

| Entregable del enunciado | Ubicación |
|---|---|
| Especificaciones 01–06 | [`Sesion2/specs/`](Sesion2/specs/) |
| Código del Controller y del Router | [`Sesion2/controller/`](Sesion2/controller/), [`Sesion2/router/`](Sesion2/router/) |
| Pruebas y resultados | [`Sesion2/tests/`](Sesion2/tests/), [`Sesion2/tests/test-results.txt`](Sesion2/tests/test-results.txt) |
| Registro de prompts | [`Sesion2/prompts-session1.md`](Sesion2/prompts-session1.md), [`Sesion2/prompts-session2.md`](Sesion2/prompts-session2.md) |
| Instrucciones, estado de requisitos y evidencias | [`Sesion2/README.md`](Sesion2/README.md), [`Sesion2/demo-evidence/`](Sesion2/demo-evidence/) |

## Inicio rápido

```bash
cd Sesion2
python -m venv .venv
# Windows: .venv\Scripts\Activate.ps1      Linux/macOS: source .venv/bin/activate
pip install -r requirements.txt
python -m controller.main      # terminal 1 (puerto 8000)
python -m router.main          # terminal 2 (puerto 8001)
python scripts/demo.py         # terminal 3: demo guiada
pytest -v                      # pruebas
```

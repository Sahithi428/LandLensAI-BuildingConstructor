# LandLensAI — Premium Feature Upgrade

## Added in this build
- Click-only workspace navigation: dashboard sections no longer open just by scrolling.
- 2D Constructor, AI Architect, 3D Studio, Cost, Timeline and Reports open only when selected.
- Editable room name, width, length, X/Y position, furniture package, material and window count.
- Room updates propagate to 2D, 3D, validation, cost and construction estimates.
- Architectural-style 2D floor plan with doors, windows and furniture symbols.
- Cost composition donut chart: materials / labour / other.
- Material composition donut chart with interactive legend values.
- Delete Project action with confirmation and backend DELETE endpoint.
- AI Architect understands common add-room and natural-language dimension commands such as `make master bedroom 14 x 16`.
- Per-room furniture selections are reflected in the offline 3D renderer.
- Building quality and rate are persisted with the building model.

## Run
```powershell
python -m venv .venv
.venv\\Scripts\\activate
python -m pip install -r requirements.txt
python run.py
```
Open http://127.0.0.1:8000

## Presentation demo
Dashboard -> Land Analysis -> Plot Planning -> Building -> Room Editor -> 2D Constructor -> AI Architect -> 3D Studio -> Materials & Cost -> Build Timeline -> Reports.

## Important
The planning, dimensions, costs, construction time and workforce are conceptual estimates. Verify survey, structural, regulatory and construction requirements with qualified professionals before real construction.


## Building navigation/type upgrade (2026-10-04)
- Fixed all 9 building-type cards (House, Villa, Apartment, Duplex, Commercial, Office, Hotel, Warehouse, Mixed-use) so each card independently selects the type and updates defaults.
- Added Customize Building modal with dimensions, floors, style, quality, rate and building name.
- Added Add Building entry point.
- Fixed dashboard isolation: Dashboard is hidden whenever another workspace is selected; 2D/3D/etc. open directly without showing Dashboard first.
- 2D and 3D remain click-only workspaces.

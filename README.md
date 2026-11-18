# North Garage Traffic Dashboard

Open `dist/index.html` in a modern browser, or serve the `dist` directory with any static web server. All values are simulated; no physical signs, sensors, or cameras are controlled.

The simulation advances manually in three-minute phase increments and wraps after phase 3. Advancing reduces occupancy on the outgoing phase's floors and updates the illustrative queue and delay. Reset restores the initial state. Turning event egress off pauses the simulation and displays inactive signals.

For future integration, replace the initial simulation adapter in `dist/app.js` with a normalized snapshot provider for sensor data or SUMO output. Define floor capacity and measured occupancy per floor before calculating a capacity-weighted total; the current demonstration assumes equal floor capacity. Queue and delay are illustrative, not traffic predictions. Add a backend and appropriate authorization before connecting operational equipment.

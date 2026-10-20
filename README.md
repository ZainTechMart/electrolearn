# ElectroLearn — Advanced Electronics Learning Starter

A responsive, static GitHub Pages website for learning electronics with English navigation and Urdu component explanations. Includes a searchable component library, circuit examples, PCB gallery, drag-and-connect workbench, project JSON import/export, SPICE-style netlist export, and a visual PCB SVG sandbox.

## Publish on GitHub Pages
1. Create a repository such as `electrolearn` (Public is simplest for a public learning site).
2. Upload `index.html`, `styles.css`, `app.js`, and `README.md` to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select `main` and `/(root)`, then save.

## Included features
- Responsive homepage/navigation and searchable component cards with Urdu notes, pin descriptions, values and ratings to verify.
- Example circuit cards, PCB gallery filters, and troubleshooting lessons.
- Visual workbench: add and move parts, connect pin dots, run simplified educational topology checks.
- Save/import the workbench as JSON.
- Export a SPICE-style `.cir` netlist for supported primitives and preview/copy it.
- Open CircuitJS/Falstad in a separate tab for deeper interactive circuit experiments. The external simulator does not automatically import/sync this site's workbench.
- Simple PCB sandbox: choose board outline, click to place pads, click twice to add visual traces, export SVG.

## Professional simulation and manufacturing limitations
This project is **not a full integrated SPICE simulator**. Its built-in Run Test function is a simplified educational topology checker; it does not solve arbitrary node voltages or branch currents and does not accurately model transistor operation, 555 internals, AC behavior, thermal dynamics, or physical component destruction. The exported SPICE-style netlist is a starting point: check node connections, device pin order, values and model definitions in your target SPICE engine before relying on results. Some device types are comments/approximations rather than complete models.

The PCB sandbox exports a **visual SVG preview only**. It does not create Gerber/drill files, perform design-rule checks, create a true copper-layer stackup, or validate electrical clearances. Do not send its output directly to manufacturing.

## Safety
Fault results are virtual educational warnings, not proof a real component will burn. Never intentionally short real batteries or overload components. Use current-limited low-voltage supplies for beginner experiments; mains-voltage projects require qualified supervision. Always verify datasheets, pinouts, voltage/current ratings and protection requirements before building hardware.

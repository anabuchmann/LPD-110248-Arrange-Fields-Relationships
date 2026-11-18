# LPD-110248 · Arrange fields and relationships in Objects

Prototype for **LPD-110248 – Allow users to configure the order that fields and relationships are listed in the object definition (UI and API)**.

## What it shows

- **Flow:** Control Panel > Objects > Default folder > Thread or Message > Fields and Relationships tabs.
- **Arrange:** a side panel based on the View Builder pattern. It lists fields and relationships together, in one order.
  - Drag a row, or use the actions menu (Move to Top, Move Up, Move Down, Move to Bottom).
  - Moved rows show a "Moved" label until you save.
  - Dragging is off while a search is active.
- **One order for fields and relationships:** the Fields and Relationships tabs list items in the saved order.
- **Never arranged:** items are listed by creation date.
- **New items:** a new field or relationship is added at the end of the order.
- **One-to-many relationships:** the parent side shows the relationship (Parent). The child side shows the relationship field (Child). Each appears once in its object.
- **Prototype controls** (bottom right): API Preview shows how the Object Admin API returns `priority` for fields and relationships. Reset restores the start state.

## Built with

Lexicon Vanilla (plain HTML + CSS, no build): https://github.com/liferay-design/lexicon-vanilla

Open `index.html` directly in a browser. No server needed.

# LPD-110248 · Arrange fields and relationships in Objects

Prototype for **LPD-110248 – Allow users to configure the order that fields and relationships are listed in the object definition (UI and API)**.

Use the **Variant** switch (bottom right) to compare three proposals.

## Variants

- **A. Arrange Panel:** the Fields and Relationships tabs stay as they are. An **Arrange** button opens a side panel, based on the View Builder pattern, that lists fields and relationships together. Cancel and Save are in the panel footer.
- **B. Unified Tab:** Fields and Relationships become one tab, **Fields and Relationships**. Rows are arranged in place, by drag and drop or the row actions, and saved at once with Undo. Search or filters turn arranging off.
- **C. Arrange Tab:** a new **Arrange** tab sits next to Fields and Relationships. It shows the combined list, with Cancel and Save at the bottom of the tab, aligned with the table. Leaving the tab with unsaved moves asks to discard them.

## Shared behavior

- **Flow:** Control Panel > Objects > Default folder > Thread or Message.
- **One order** for fields and relationships. The Fields and Relationships tabs list items in the saved order.
- **Arranging:** drag a row, or use the actions menu (Move to Top, Move Up, Move Down, Move to Bottom). Moved rows show a "Moved" label until you save. Dragging is off while a search is active.
- **Never arranged:** items are listed by creation date. After the first save, the saved order applies.
- **New items** are added at the end of the order.
- **One-to-many relationships:** the parent side shows the relationship (Parent). The child side shows the relationship field (Child). Each appears once in its object.
- **API Preview** shows how the Object Admin API returns `priority` for fields and relationships. **Reset** restores the start state.

## Built with

Lexicon Vanilla (plain HTML + CSS, no build): https://github.com/liferay-design/lexicon-vanilla

Open `index.html` directly in a browser. No server needed.

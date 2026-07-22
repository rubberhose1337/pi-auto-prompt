# Prompt refiner extension

This project contains a project-local pi extension at `.pi/extensions/prompt-refiner.ts`.

While typing a prompt, press **Ctrl+Enter** to ask the selected pi model to rewrite it. The overlay shows an animated refinement indicator, elapsed time, streamed character progress, and a live preview while it works. Once complete, it shows the original and refined prompt:

- **Accept** replaces the editor text with the refined prompt.
- **Decline**, **Esc**, or **Ctrl+C** closes the overlay without changing the editor.
- Use **↑/↓**, **←/→**, **A**, or **D** to choose an option, then press **Enter**.

The extension uses the active pi model and its configured credentials. Start pi in this project (or test directly with `pi -e ./.pi/extensions/prompt-refiner.ts`) and reload with `/reload` after changes.

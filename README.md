# Prompt refiner extension

Bullshit in, bullshit out. This should atleast to some degree fix it. Maybe. I dont know. But it feels decent to use?

I created this extension for Pi in order to improve the prompts I input while keeping them as close as possible to the original.

It works quick and simple. It automatically uses the currently configured Model so no need for configuration or switching there. You just write a prompt and instead of sending it you press Ctrl+Enter. This then generates a better prompt. You can either accept or decline. On accept, the prompt you had written gets swapped out with the new and improved prompt. If you decline, the overlay closes and you just go back to the original prompt

While typing a prompt, press **Ctrl+Enter** to ask the selected pi model to rewrite it. The overlay shows an animated refinement indicator, elapsed time, streamed character progress, and a live preview while it works. Once complete, it shows the original and refined prompt.

## Installation

Install it as a Pi package:

```bash
pi install git:github.com/rubberhose1337/pi-auto-prompt
```

Pi will load the extension automatically in future sessions.

For a local checkout, start Pi from the repository root. The extension is discovered automatically from `.pi/extensions/` after the project is trusted. You can also test it directly:

```bash
pi -e ./.pi/extensions/prompt-refiner.ts
```

After changing the extension, use `/reload` in Pi.

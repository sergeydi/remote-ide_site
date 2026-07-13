---
title: "Syntax-Highlighted Editor"
seo_title: "Syntax-Highlighted Code Editor for iPad — Remote IDE"
description: "Syntax-highlighted code editor for iPad. Powered by Runestone and Tree-sitter — accurate highlighting for 22 languages with a customizable editing experience."
icon: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.75" stroke-linecap="round" stroke-linejoin="round"><path d="M4 12.15V4a2 2 0 0 1 2-2h8a2.4 2.4 0 0 1 1.706.706l3.588 3.588A2.4 2.4 0 0 1 20 8v12a2 2 0 0 1-2 2h-3.35"/><path d="M14 2v5a1 1 0 0 0 1 1h5"/><path d="m5 16-3 3 3 3"/><path d="m9 22 3-3-3-3"/></svg>'
---

<div class="feature-sections">

<div class="feature-section">
<div class="feature-section-text">
<h3>A VS Code-style color theme, adapted for iPad</h3>
<p>The color scheme is inspired by Visual Studio Code's default dark and light themes — familiar if you already spend time in VS Code on your Mac. Keywords, strings, comments, types, and functions each get a distinct, readable color in both dark and light appearances — a TOML file, for example, gets clearly colored section headers, keys, and string values even in light mode.</p>
<p>The theme adapts automatically to your system appearance — no manual toggle in the app.</p>
<ul>
<li>Keywords: blue (dark) / purple (light)</li>
<li>Strings: warm orange (dark) / dark red (light)</li>
<li>Types and classes: teal in both modes</li>
<li>Comments: italic green in both modes</li>
<li>Functions: warm yellow (dark) / brown (light)</li>
</ul>
</div>
<div class="feature-shot"><img src="remote-ide-syntax-highlighting-light.png" alt="pyproject.toml open in the editor in light mode, with section headers, keys, and strings syntax-highlighted"></div>
</div>

<div class="feature-section-text">
<h3>Tree-sitter parsing — no regex shortcuts</h3>
<p>Every language is parsed using <a href="https://tree-sitter.github.io/tree-sitter/" target="_blank" rel="noopener">Tree-sitter</a> — the same incremental parser used in Neovim, Helix, and VS Code. It builds a real syntax tree as you type, so highlighting stays accurate even in complex nested structures.</p>
<p>The editor uses a two-phase rendering strategy: plain text appears instantly when you open a file, and the fully highlighted state is built on a background thread and swapped in without blocking the UI.</p>
<ul>
<li>Incremental re-parse on every edit — only changed subtrees are reprocessed</li>
<li>Background parsing keeps the UI responsive on large files</li>
<li>Accurate highlighting inside strings, templates, and multiline constructs</li>
</ul>
</div>

<div class="feature-section-text">
<h3>22 languages out of the box</h3>
<p>Open any of the supported file types and the editor picks the right grammar automatically based on the file extension. No manual mode switching needed.</p>
<ul>
<li>Swift, Python, JavaScript, TypeScript, TSX</li>
<li>Go, Rust, C, C++, Java, Ruby, PHP</li>
<li>Bash / Zsh / Shell, HTML, CSS, SCSS</li>
<li>JSON, YAML, TOML, Markdown, SQL</li>
</ul>
</div>

<div class="feature-section-text">
<h3>Editor settings you actually use</h3>
<p>A small set of focused settings covers the things that matter most for coding on a touchscreen. No settings bloat — just the options that change how you work.</p>
<ul>
<li>Font family and size — choose any monospaced font installed on your iPad</li>
<li>Line numbers on or off</li>
<li>Word wrap on or off</li>
<li>Indent with tabs or spaces, configurable width (2, 4, or custom)</li>
<li>Built-in find interaction — tap the search icon or use the keyboard shortcut</li>
</ul>
</div>

</div>

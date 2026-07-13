---
title: "Dark & Light Themes"
date: 2026-07-13
seo_title: "Automatic Dark & Light Themes for iPad — Remote IDE"
description: "Automatic dark and light themes for Remote IDE on iPad. Follows iPadOS system appearance — no manual toggle, no separate theme setting needed."
icon: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.75" stroke-linecap="round" stroke-linejoin="round"><path d="M12 2v2"/><path d="M14.837 16.385a6 6 0 1 1-7.223-7.222c.624-.147.97.66.715 1.248a4 4 0 0 0 5.26 5.259c.589-.255 1.396.09 1.248.715"/><path d="M16 12a4 4 0 0 0-4-4"/><path d="m19 5-1.256 1.256"/><path d="M20 12h2"/></svg>'
---

<div class="section-label" style="margin-bottom:16px;">Same file, both appearances</div>
<div class="privacy-box reveal" style="grid-template-columns:1fr 1fr;gap:40px;padding:24px;margin-bottom:80px;">
<div>
<h3 style="font-family:var(--mono);font-size:18px;font-weight:700;margin-bottom:16px;letter-spacing:-0.5px;">Light</h3>
{{< shot src="remote-ide-light-theme-editor.png" alt="pyproject.toml open in the editor in light mode" >}}
</div>
<div>
<h3 style="font-family:var(--mono);font-size:18px;font-weight:700;margin-bottom:16px;letter-spacing:-0.5px;">Dark</h3>
{{< shot src="remote-ide-dark-theme-editor.png" alt="The same pyproject.toml file open in the editor in dark mode" >}}
</div>
</div>

<div class="feature-sections">

<div class="feature-section-text">
<h2>Automatic — no setting required</h2>
<p>Remote IDE reads your system appearance and applies the matching theme everywhere: the app chrome, the file sidebar, the editor, and the terminal. Switch iPadOS between light and dark in Control Center — the app follows instantly, mid-session, without restarting.</p>
<p>There is no separate theme picker inside the app. The system setting is the setting.</p>
<ul>
<li>Follows iPadOS system appearance</li>
<li>Updates live when you switch in Control Center</li>
<li>Consistent across all panels: sidebar, editor, terminal</li>
</ul>
</div>

<div class="feature-section-text">
<h2>A syntax theme designed for readability</h2>
<p>The editor uses a custom color scheme inspired by Visual Studio Code's default themes — familiar and well-tested across millions of developers. Each token type has a distinct, readable color in both modes. The contrast ratios are calibrated for both the ProMotion display in bright daylight and a dimmed screen at night.</p>
<ul>
<li>Dark mode: deep background (#0a0a0f equivalent), muted chrome, vivid syntax colors</li>
<li>Light mode: white background, crisp syntax colors with sufficient contrast</li>
<li>Comments in italic green — visually de-emphasized in both modes</li>
<li>Keywords, types, strings, and functions each have a distinct color</li>
</ul>
</div>

<div class="feature-section-text">
<h2>The terminal is always dark</h2>
<p>The AI agent terminal window is always forced to dark mode — regardless of your system setting. Terminal output is designed for dark backgrounds, and most developer tools (htop, git diff, CLI color schemes) assume a dark terminal. The agent window respects that convention.</p>
<p>The main editor and sidebar continue to follow the system appearance as normal.</p>
<ul>
<li>Agent terminal: always dark</li>
<li>Main editor + sidebar: follows system</li>
</ul>
</div>

</div>

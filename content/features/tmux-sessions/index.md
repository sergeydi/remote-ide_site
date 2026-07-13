---
title: "Persistent Terminal Sessions"
date: 2026-07-13
seo_title: "Persistent SSH Terminal Sessions with tmux — Remote IDE"
description: "Keep your SSH session alive across app backgrounding and network drops. Remote IDE wraps your terminal in tmux and reattaches automatically."
icon: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.75" stroke-linecap="round" stroke-linejoin="round"><path d="m12.83 2.18a2 2 0 0 0-1.66 0L2.6 6.08a1 1 0 0 0 0 1.83l8.58 3.91a2 2 0 0 0 1.66 0l8.58-3.9a1 1 0 0 0 0-1.83Z"/><path d="m22 17.65-9.17 4.16a2 2 0 0 1-1.66 0L2 17.65"/><path d="m22 12.65-9.17 4.16a2 2 0 0 1-1.66 0L2 12.65"/></svg>'
---

<div class="feature-sections">

<div class="feature-section">
<div class="feature-section-text">
<h2>Guided setup if tmux isn't installed</h2>
<p>Not every server ships with tmux out of the box. If it's missing, Remote IDE shows install instructions for common Linux distributions right in the server settings — Ubuntu/Debian, macOS via Homebrew, Fedora/RHEL, CentOS 7, and Arch Linux — each with a ready-to-copy install command, so getting persistent sessions running is a copy-paste away, not a support ticket.</p>
<ul>
<li>Built-in install guide for common Linux distros</li>
<li>Tap-to-copy install commands</li>
<li>Works over your existing SSH connection</li>
</ul>
</div>
{{< shot src="remote-ide-tmux-install-guide.png" alt="In-app tmux info sheet with an About section and copy-paste install commands for Ubuntu, Debian, macOS, Fedora, CentOS, and Arch Linux" >}}
</div>

<div class="feature-section-text">
<h2>Sessions that outlive the app</h2>
<p>Switch away to another app, lock your iPad, or lose Wi-Fi for a minute — a plain SSH session dies the moment the connection drops. Turn on "Use tmux" for a server and Remote IDE wraps the session in tmux on the server side instead, so the shell keeps running whether or not you're connected to it.</p>
<p>Your long-running build, your `npm run dev`, your tail on a log file — none of it gets interrupted by backgrounding the app.</p>
<ul>
<li>Server-side tmux session survives disconnects</li>
<li>Long-running commands keep running while you're away</li>
<li>One toggle per server — no manual tmux commands required</li>
</ul>
</div>

<div class="feature-section-text">
<h2>Reattach exactly where you left off</h2>
<p>Reopen Remote IDE and it reattaches to the same tmux session automatically — same scrollback, same running process, same terminal state. You don't type <code>tmux attach</code> yourself; the app handles session naming and reattachment for you.</p>
<p>The AI agent window uses its own dedicated tmux session, kept separate from your console session, so an agent run and a manual terminal session on the same server never collide.</p>
<ul>
<li>Automatic reattachment on reconnect — no manual tmux commands</li>
<li>Scrollback and running processes preserved between sessions</li>
<li>Separate sessions for the console and the AI agent window</li>
</ul>
</div>

</div>

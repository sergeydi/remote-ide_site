---
title: "Remote Filesystem Mode"
seo_title: "Edit Files Directly on a Remote Server — Remote IDE"
description: "Browse and edit files directly on your server over SFTP — no download, no local copy, no sync step. Changes save straight to the remote path."
icon: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.75" stroke-linecap="round" stroke-linejoin="round"><rect width="20" height="8" x="2" y="2" rx="2" ry="2"/><rect width="20" height="8" x="2" y="14" rx="2" ry="2"/><line x1="6" x2="6.01" y1="6" y2="6"/><line x1="6" x2="6.01" y1="18" y2="18"/></svg>'
---

<div class="feature-sections">

<div class="feature-section">
<div class="feature-section-text">
<h3>Turn it on per remote path</h3>
<p>Remote Filesystem is a toggle on each named remote path, not a global setting. Keep it off for projects where you want the traditional upload/download workflow, and turn it on for servers where you'd rather edit in place — a staging box, a Raspberry Pi, a production config directory you only touch occasionally.</p>
<ul>
<li>Per-remote-path toggle — mix and match across servers</li>
<li>Works over the same SSH connection, no extra setup</li>
<li>Git change tracking and the terminal keep working alongside it</li>
</ul>
</div>
<div class="feature-shot"><img src="remote-ide-remote-filesystem-toggle.png" alt="New Remote Project dialog with the Use remote filesystem toggle switched on"></div>
</div>

<div class="feature-section-text">
<h3>Edit files where they actually live</h3>
<p>Turn on Remote Filesystem for a server's remote path and the sidebar switches to browsing that server directly over SFTP. Open a file, edit it, save — the change lands on the server immediately. There's no local copy to keep track of.</p>
<p>This is a different model from pushing and pulling a project tree: instead of syncing state between your iPad and the server, you're working on one copy, in one place.</p>
<ul>
<li>File tree browses the remote server directly, not iCloud Drive</li>
<li>Open and save files over SFTP with no intermediate step</li>
<li>Nothing to push, pull, or keep in sync</li>
</ul>
</div>

<div class="feature-section-text">
<h3>No stale copies, no drift</h3>
<p>Traditional sync means two copies of your project can disagree — an edit on the server, an edit on your iPad, and now you're merging by hand. Remote Filesystem Mode removes the second copy entirely, so what you see in the editor is exactly what's on disk on the server.</p>
<p>That also means changes made outside Remote IDE — by a deploy script, a teammate, or a process running on the server — show up the moment you reopen the file.</p>
<ul>
<li>Single source of truth: the server</li>
<li>No merge conflicts between local and remote state</li>
<li>See external changes as soon as you reopen a file</li>
</ul>
</div>

</div>

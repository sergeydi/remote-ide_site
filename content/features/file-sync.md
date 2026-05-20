---
title: "One-Tap File Sync"
description: "One-tap SFTP file sync for iPad. Push your project to a remote server or pull it back instantly — fully recursive, with live transfer progress."
icon: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.75" stroke-linecap="round" stroke-linejoin="round"><path d="M12 17V3"/><path d="m6 11 6 6 6-6"/><path d="M19 21H5"/></svg>'
---

<div class="feature-sections">

<div class="feature-section-text">
<h3>Upload and download with one tap</h3>
<p>The toolbar has two buttons: upload and download. Tap upload to push your entire local project to the configured remote path on your server. Tap download to pull the remote state back to your iPad. That's it.</p>
<p>Both operations are fully recursive — they handle nested directories, any number of files, and any file size. The app reports the transfer state in the toolbar so you always know what's happening.</p>
<ul>
<li>Upload entire project tree to the remote server</li>
<li>Download the remote project back to iCloud Drive</li>
<li>Fully recursive — handles deep directory trees</li>
<li>Progress indicator and cancel button during transfer</li>
</ul>
</div>

<div class="feature-section-text">
<h3>SFTP under the hood</h3>
<p>File sync uses SFTP over your existing SSH connection — no separate protocol, no extra port to open, no additional credentials. If you can SSH to the server, file sync works automatically.</p>
<p>Transfers run on a background task so the editor and terminal stay fully responsive while files are uploading or downloading. The file tree refreshes automatically when a download completes.</p>
<ul>
<li>SFTP over the same SSH connection — no extra configuration</li>
<li>Background transfer — editor stays usable during sync</li>
<li>File tree reloads automatically after download</li>
<li>Error handling with a clear error message on failure</li>
</ul>
</div>

<div class="feature-section-text">
<h3>Per-server remote paths</h3>
<p>Each server configuration has one or more named remote paths — the directories on the server that your project maps to. You can define multiple paths per server (for example, staging and production) and switch between them without editing the server config.</p>
<p>When you trigger an upload or download, it always uses the currently active remote path for that server.</p>
<ul>
<li>Multiple named remote paths per server</li>
<li>Quick-switch between paths without re-entering credentials</li>
<li>Active path shown in the agent window title bar</li>
</ul>
</div>

</div>

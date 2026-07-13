---
title: "Split View & Stage Manager"
date: 2026-07-13
seo_title: "Split View & Stage Manager Support for iPad — Remote IDE"
description: "Split View and Stage Manager support in Remote IDE for iPad. Run multiple SSH sessions, projects, and AI agents side by side in independent windows."
icon: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.75" stroke-linecap="round" stroke-linejoin="round"><rect width="7" height="9" x="3" y="3" rx="1"/><rect width="7" height="5" x="14" y="3" rx="1"/><rect width="7" height="9" x="14" y="12" rx="1"/><rect width="7" height="5" x="3" y="16" rx="1"/></svg>'
---

<div class="feature-sections">

<div class="feature-section">
<div class="feature-section-text">
<h2>AI agent in a dedicated window</h2>
<p>Run Claude Code or another AI agent in its own Remote IDE window while you review its changes in a second window. The agent writes code, the second window shows you the diff.</p>
<p>This is the workflow that makes AI-assisted development actually pleasant on iPad — no tab switching, no context loss.</p>
<ul>
<li>Agent window runs <code>claude</code> in your SSH terminal</li>
<li>Editor window shows the files being modified</li>
<li>Review changes in real time as the agent works</li>
</ul>
</div>
{{< shot src="remote-ide-split-view-ai-agent.png" alt="SSH console window side by side with a dedicated Claude Code agent window in Split View" >}}
</div>

<div class="feature-section-text">
<h2>Split View: code and docs side by side</h2>
<p>Open Remote IDE in Split View alongside Safari, Notes, or any other app. Read the documentation on the right while you edit code on the left — no switching, no losing your place.</p>
<p>Resize the split to whatever ratio works for you. Remote IDE adapts its layout as the window shrinks or grows.</p>
<ul>
<li>Editor + browser for documentation lookup</li>
<li>Terminal + notes for recording commands</li>
<li>Two Remote IDE windows on two different servers</li>
</ul>
</div>

<div class="feature-section-text">
<h2>Stage Manager: multiple windows, full control</h2>
<p>With Stage Manager enabled, you can run multiple Remote IDE windows simultaneously — each with its own project, SSH connection, and state. Switch between them instantly without losing context.</p>
<p>Stage Manager treats each window as an independent workspace. You can have your backend server in one window and your frontend in another, both connected over SSH.</p>
<ul>
<li>Unlimited concurrent Remote IDE windows</li>
<li>Each window maintains its own SSH session</li>
<li>Independent file trees and editor state per window</li>
<li>Drag files between windows via the Files app</li>
</ul>
</div>

</div>

<div style="margin-top:80px;">
<div class="section-label" style="margin-bottom:16px;">How to enable</div>
<div class="privacy-box reveal" style="grid-template-columns:1fr 1fr;gap:40px;">
<div>
<h3 style="font-family:var(--mono);font-size:18px;font-weight:700;margin-bottom:16px;letter-spacing:-0.5px;">Split View</h3>
<ol style="color:var(--muted);font-size:14px;line-height:1.8;padding-left:20px;">
<li>Open Remote IDE</li>
<li>Tap the three dots (<strong style="color:var(--text);">···</strong>) at the top of the screen</li>
<li>Select <strong style="color:var(--text);">Split View</strong></li>
<li>Choose the second app from your home screen</li>
</ol>
</div>
<div>
<h3 style="font-family:var(--mono);font-size:18px;font-weight:700;margin-bottom:16px;letter-spacing:-0.5px;">Stage Manager</h3>
<ol style="color:var(--muted);font-size:14px;line-height:1.8;padding-left:20px;">
<li>Enable Stage Manager in Control Center</li>
<li>Open Remote IDE — it appears as a window</li>
<li>Tap and hold the Remote IDE dock icon</li>
<li>Select <strong style="color:var(--text);">New Window</strong> for a second instance</li>
</ol>
</div>
</div>
</div>

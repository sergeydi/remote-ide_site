---
title: "Full File Manager"
date: 2026-07-13
seo_title: "Full File Manager for iPad Developers — Remote IDE"
description: "Full remote file manager for iPad. Create, rename, delete, and navigate your SSH server's project tree using a familiar iOS sidebar."
icon: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.75" stroke-linecap="round" stroke-linejoin="round"><path d="m6 14 1.5-2.9A2 2 0 0 1 9.24 10H20a2 2 0 0 1 1.94 2.5l-1.54 6a2 2 0 0 1-1.95 1.5H4a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h3.9a2 2 0 0 1 1.69.9l.81 1.2a2 2 0 0 0 1.67.9H18a2 2 0 0 1 2 2v2"/></svg>'
---

<div class="feature-sections">

<div class="feature-section">
<div class="feature-section-text">
<h2>Compact mode for smaller windows</h2>
<p>When Remote IDE runs in a narrow Split View column or a small Stage Manager window, the sidebar switches to a compact list of projects. Tap a project to navigate into its file tree in a separate screen — the header shows the project name with a back button to return to the project list. Everything still works — just optimized for less horizontal space.</p>
<ul>
<li>Automatic compact/regular layout based on available width</li>
<li>NavigationStack-based navigation in compact mode</li>
<li>Same create/delete/rename functionality in both layouts</li>
</ul>
</div>
{{< shot src="remote-ide-compact-file-browser.png" alt="Compact file tree view showing a project's files and folders with a back button to return to the projects list" >}}
</div>

<div class="feature-section-text">
<h2>Projects and files in one sidebar</h2>
<p>The sidebar shows two levels: your projects at the top, and the file tree of the selected project below. Tap a project to expand its tree. Tap a file to open it in the editor. It's the same navigation model as Xcode's Project Navigator — familiar if you already develop on Apple platforms.</p>
<p>The file tree uses OutlineGroup for native expand/collapse behavior. Nested directories expand inline, so you can drill into a deep path without losing sight of the rest of the tree.</p>
<ul>
<li>Projects list with tap-to-select</li>
<li>Recursive file tree with native expand/collapse</li>
<li>File type icons for common extensions</li>
<li>Tap any file to open it instantly in the editor</li>
</ul>
</div>

<div class="feature-section-text">
<h2>Create, rename, and delete</h2>
<p>Everything you'd do in Finder is available directly in the sidebar. Create a new file or folder from the + menu in the file section header. Rename or delete a project from its context menu. Rename or delete a file or folder the same way.</p>
<p>File names are validated before creation — empty names, reserved names, names with invalid characters, and names that already exist all produce clear error messages rather than silent failures.</p>
<ul>
<li>New file and new folder from the + menu</li>
<li>Rename and delete via context menu (long press)</li>
<li>Create / rename / delete projects from the projects section</li>
<li>Validation: empty, reserved, duplicate, and invalid character checks</li>
</ul>
</div>

<div class="feature-section-text">
<h2>Git status indicators in the tree</h2>
<p>Files that have been modified, added, or deleted since the last commit are labeled directly in the file tree. You can see the state of your entire working tree at a glance without running <code>git status</code> in the terminal.</p>
<p>A git status button in the file section header opens the full Git Status panel with a diff viewer for any changed file.</p>
<ul>
<li>Color-coded status labels: A (added), M (modified), D (deleted), R (renamed)</li>
<li>One-tap access to the full Git Status and diff view</li>
</ul>
</div>

</div>

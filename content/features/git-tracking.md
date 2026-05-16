---
title: "Git Change Tracking"
description: "See modified, added, deleted, and renamed files at a glance in the project tree. View diffs and git status without leaving the app."
icon: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.75" stroke-linecap="round" stroke-linejoin="round"><path d="M15 6a9 9 0 0 0-9 9V3"/><circle cx="18" cy="6" r="3"/><circle cx="6" cy="18" r="3"/></svg>'
---

<div class="feature-sections">

<div class="feature-section-text">
<h3>Git status in the file tree</h3>
<p>Modified files are highlighted directly in the project tree — no separate git panel to open, no command to run. As soon as you save a file, the indicator updates to reflect the current git status of each item.</p>
<p>Each file is labeled with a color-coded status letter: <strong style="color:var(--green);">A</strong> for added, <strong style="color:var(--amber);">M</strong> for modified, <strong style="color:#ff453a;">D</strong> for deleted, <strong style="color:var(--blue);">R</strong> for renamed. You can see the state of your entire working tree at a glance without running a single command.</p>
<ul>
<li>Added files: green</li>
<li>Modified files: orange</li>
<li>Deleted files: red</li>
<li>Renamed files: blue</li>
<li>Conflicted files: red</li>
</ul>
</div>

<div class="feature-section-text">
<h3>Full diff viewer</h3>
<p>Tap the git status button in the file tree header to open the Git Status panel. It shows every changed file in the project, grouped by status. Select any file to see a full unified diff — with line numbers, hunk headers, and color-coded additions and deletions.</p>
<p>The diff viewer scrolls both vertically and horizontally, so long lines don't get cut off. It uses a monospaced font throughout for readability.</p>
<ul>
<li>Added lines highlighted in green</li>
<li>Deleted lines highlighted in red</li>
<li>Context lines in neutral gray</li>
<li>Old and new line numbers shown side by side</li>
<li>Hunk headers for navigating large diffs</li>
</ul>
</div>

<div class="feature-section-text">
<h3>Works on the files you already have</h3>
<p>Git status is read from the project files in your iCloud Drive — the same files the editor works with. There's nothing to configure and no separate git tool to install on your iPad. As long as the project directory contains a <code>.git</code> folder, status tracking works automatically.</p>
<p>If the project isn't a git repository, the Git Status panel tells you clearly — no confusing empty states.</p>
<ul>
<li>Detects <code>.git</code> folder automatically</li>
<li>Shows "Not a Git Repository" when <code>.git</code> is absent</li>
<li>Shows "Working tree clean" when there are no uncommitted changes</li>
<li>File count displayed in the section header: <em>Changes (5)</em></li>
</ul>
</div>

</div>

---
title: "SSH Key & Password Auth"
description: "SSH key and password authentication for iPad. Credentials stored securely in the iOS Keychain — never in files, never transmitted to any third party."
icon: '<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.75" stroke-linecap="round" stroke-linejoin="round"><path d="M2.586 17.414A2 2 0 0 0 2 18.828V21a1 1 0 0 0 1 1h3a1 1 0 0 0 1-1v-1a1 1 0 0 1 1-1h1a1 1 0 0 0 1-1v-1a1 1 0 0 1 1-1h.172a2 2 0 0 0 1.414-.586l.814-.814a6.5 6.5 0 1 0-4-4z"/><circle cx="16.5" cy="7.5" r=".5" fill="currentColor"/></svg>'
---

<div class="feature-sections">

<div class="feature-section-text">
<h3>Password and private key auth</h3>
<p>Remote IDE supports both authentication methods you'd use on a desktop: password-based and private key-based. Choose the method when you add a server; it's stored with the server configuration and used automatically on every connection.</p>
<p>Private keys are pasted in PEM format — the same format used by OpenSSH. Ed25519 keys are parsed natively. If your key has a passphrase, you can store that separately in the Keychain and it's supplied automatically at connection time.</p>
<ul>
<li>Password authentication</li>
<li>Private key authentication (PEM format)</li>
<li>Ed25519 key support</li>
<li>Optional passphrase for encrypted private keys</li>
</ul>
</div>

<div class="feature-section-text">
<h3>Keychain storage — hardware-backed security</h3>
<p>Passwords, private keys, and passphrases are stored exclusively in the iOS Keychain — the same hardware-backed secure enclave used by iOS itself for Face ID credentials and payment data. They are never written to iCloud, never logged, and never transmitted to any third party.</p>
<p>When you delete a server from Remote IDE, its credentials are deleted from the Keychain immediately. There are no orphaned secrets left behind.</p>
<ul>
<li>Credentials stored in the iOS Keychain, not in app files</li>
<li>Keychain entries removed when a server is deleted</li>
<li>Not synced to iCloud Drive — stays on-device</li>
<li>Never sent to Remote IDE servers or any third party</li>
</ul>
</div>

<div class="feature-section-text">
<h3>Multiple servers, one place</h3>
<p>Add as many servers as you need. Each server has its own name, host, port, username, authentication credentials, and remote paths. Switch between them from the servers sheet — one tap to connect, one tap to disconnect.</p>
<p>Edit or delete any server at any time. Swipe left on a server in the list to reveal the edit and delete actions.</p>
<ul>
<li>Unlimited servers</li>
<li>Per-server authentication settings</li>
<li>Swipe to edit or delete</li>
<li>Custom port support (defaults to 22)</li>
</ul>
</div>

</div>

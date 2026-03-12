# EncryptorX 🔐

## What it does

EncryptorX is a **military-grade AES-256-GCM encryption tool** that runs entirely in your browser. Enter your ACCSI number and password to derive a unique encryption key, then encrypt and decrypt sensitive text with complete privacy. No data leaves your device.

## How to use

1. **Load Your Key**: Enter your ACCSI number (4-12 digits) and a strong password (8+ chars, must include special char: `! @ # $ % ^ & * ( )`)
2. **Encrypt**: Paste or upload text, click "Encrypt", and get a Base64-encoded ciphertext
3. **Decrypt**: Paste the encrypted text, click "Decrypt", and recover the original message
4. **Clear Session**: Click "Clear Session" to remove the key from memory when done

## Security

- **AES-256-GCM**: Military-grade encryption standard used by governments and enterprises
- **PBKDF2 Key Derivation**: 250,000 iterations with SHA-512 hash for brute-force resistance
- **Unique IV per Message**: Random 12-byte initialization vector prevents pattern analysis
- **Client-Side Only**: All encryption happens in your browser; nothing is sent to servers

## Deploy

### GitHub Pages
1. Push this repository to GitHub
2. Go to **Settings → Pages → Source** and select the `main` branch
3. Your app will be live at `https://{username}.github.io/{repo-name}`

### Vercel
1. Connect your GitHub repository to Vercel
2. Vercel auto-deploys on every push
3. Your app will be live at `https://{project-name}.vercel.app`

### Self-Hosted
1. Copy all files to your web server
2. Serve `index.html` as the root
3. Ensure HTTPS is enabled (required for Web Crypto API)

## License

MIT

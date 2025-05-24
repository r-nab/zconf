## VSCodium Settings and Extensions

- `settings.json` — user settings
- `extensions.txt` — List of installed extensions

---

1. Export installed extensions and settings:

```bash
codium --list-extensions > old_extensions.txt
cp ~/Library/Application\ Support/VSCodium/User/settings.json old_settings.json
```

3. Replace settings
```bash
cp ./settings.json ~/Library/Application\ Support/VSCodium/User/settings.json
```

4. Install extensions from list:
```bash
cat extensions.txt | xargs -L 1 codium --install-extension
```

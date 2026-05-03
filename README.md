# 🛠️ Dotfiles

Minimal personal terminal setup for macOS.

This repo contains my core configuration files so I can quickly replicate my terminal environment on a new machine.

---

## 🚀 Quick Setup (New Machine)

```bash
git clone git@github.com:YOUR_USERNAME/dotfiles.git ~/dotfiles
cd ~/dotfiles
ln -sf ~/dotfiles/.zshrc ~/.zshrc
ln -sf ~/dotfiles/.gitconfig ~/.gitconfig
```

Restart your terminal after linking.

---

## 📁 Contents

* `.zshrc` → shell configuration (aliases, prompt, tooling)
* `.gitconfig` → git settings (name, email, defaults)

---

## 🔗 How It Works

This repo uses **symlinks** so your system reads:

```
~/.zshrc
~/.gitconfig
```

…but the actual files live in:

```
~/dotfiles/
```

This keeps everything version-controlled and easy to update.

---

## 🔄 Updating

After making changes:

```bash
git add .
git commit -m "Update dotfiles"
git push
```

---

## 🔐 Notes

Do **not** store sensitive data here (tokens, keys, etc.).

---

## 🧠 Goal

Keep setup simple, fast, and portable across machines.

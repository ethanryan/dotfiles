# 🛠️ Dotfiles

Minimal macOS terminal setup with Zsh and Git.

---

## 🚀 New Machine Setup

### 1. Install required tools

Install the basics:

* Visual Studio Code
* Git
* Zsh (default on macOS)

---

### 2. Set up SSH for GitHub

```bash
ssh-keygen -t ed25519 -C "your-email@example.com"
pbcopy < ~/.ssh/id_ed25519.pub
```

Add the key to GitHub → Settings → SSH Keys

Test:

```bash
ssh -T git@github.com
```

---

### 3. Clone repo

```bash
git clone git@github.com:YOUR_USERNAME/dotfiles.git ~/dotfiles
cd ~/dotfiles
```

---

### 4. Link config files

```bash
ln -sf ~/dotfiles/.zshrc ~/.zshrc
ln -sf ~/dotfiles/.gitconfig ~/.gitconfig
```

---

### 5. Install Oh My Zsh

```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

When prompted to overwrite `.zshrc`, choose **No**

---

### 6. Restart terminal

```bash
source ~/.zshrc
```

---

## ⚡ Notes

* VS Code: install the `code` command in PATH via Command Palette
* Shortcuts/aliases are defined in `.zshrc`

---

## 🔄 Updating

```bash
cd ~/dotfiles
git add .
git commit -m "Update dotfiles"
git push
```

---

## 🧠 Goal

Fast, minimal, repeatable setup across machines.

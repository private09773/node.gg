# node.gg
---

**Navigation and Forms**
<div align="left">
<a href="INDEX.md" target="_blank">Homepage</a>
<a href="ABOUT.md" target="_blank">About</a>
<a href="CONTACT.md" target="_blank">Contact</a>
<a href="TIER.md" target="_blank">Tiers</a>
<a href="LEGAL.md" target="_blank">Legal</a>
</div>

<br>

> Welcome to **node.gg**, a hosting platform that offers actual services instead of your typical ones.
<br>

**Why Choose Us?**
<br>
- Auto Renewal Every 4 Months
- Friendly Staff
- What You See is What You Get
- 24/7 Hosting
- No Forced Discord Membership
- Commercial Usage Allowed
<br>

**Preview on What We Do in the Terminal**
```bash
#!/bin/bash

# node.gg Staff Deploy Script
# Usage: ./deploy.sh <GITHUB_URL> <USER>

REPO_URL="$1"
USER="$2"

REPO_NAME=$(basename "$REPO_URL" .git)
DEPLOY_DIR="/home/nodegg/bots/$USER"

echo "📦 Deploying bot for $USER..."
mkdir -p "$DEPLOY_DIR"
cd "$DEPLOY_DIR"

curl -L "$REPO_URL/archive/main.zip" -o bot.zip
unzip -q bot.zip
cd REPO-main

if [ -f "requirements.txt" ]; then
    pip install -r requirements.txt
fi

echo "✅ Bot deployed for $USER!"
echo "📢 Sending DM to $USER..."
# Send DM via Discord webhook or bot
```
<br>

**How do I Host?**
<br>
There are two types of Hosting a Bot On Our node.gg:
<br>
**1. Our Discord Server**
<br>
Steps on How to Host:
<br>
**1. Open a Ticket**
<p> Kindly open a ticket at `#support` in our server.
<p> Staff will ask you questions, answer these.
**2. Give your Github Repo.**
<br>
-# Absolutly do not hardcode or paste the token in your code, set it in Github Actions and Secrets.
<br>
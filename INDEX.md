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
###### Absolutly do not hardcode or paste the token in your code, set it in Github Actions and Secrets.
<br>
**3. Wait for the Magic**
<p> The bot will be online and you will be told in your ticket. </p>
<br>

**2. Email Method**
---

1. Compose an Email

Send an email to nodegg.support@gmail.com with the subject line: Bot Hosting Request

---

2. Include the Following Details

· Your Discord Username
· Bot Name
· GitHub Repository Link (public or private with token access)
· Preferred Tier (PH-1-FREE, PH-2-FREE, or PH-3-PAY)
· Storage Required (in GB)
· Programming Language
· Any special instructions

---

3. Wait for the Magic

Once we receive your email, staff will review your code and reply with confirmation. The bot will be online and you will be notified via email reply.

---

Important Note

Absolutely do not hardcode or paste the token in your code. Set it in GitHub Actions and Secrets.

---

```
**Email Submission Template**

To: nodegg.support@gmail.com
Subject: Bot Hosting Request

Discord Username: ________
Bot Name: ________
GitHub Link: ________
Tier: ________
Storage: ________ GB
Language: ________
Special Instructions: ________
```

**❓ Frequently Asked Questions**

---

**1. How do I host my bot?**

1. Send your GitHub link in the submissions channel.
2. Staff will review your code and requirements.txt.
3. Wait for the magic.
4. The bot will be online and you will be told in your ticket.

---

**2. Do I need to stay in your Discord server?**

No. You are free to stay or leave. We do not force membership. Leaving will not get your bot deleted or suspended.

---

**3. Is commercial usage allowed?**

Yes. Commercial usage is allowed on all tiers. You can run a business, accept donations, or offer in-game items. No bans. No questions.

---

**4. Do I need to renew my server?**

No. Servers auto-renew every 4 months. You do not need to take any action.

---

**5. What happens if my bot goes down?**

We aim for 24/7 uptime. If something goes wrong, open a ticket and staff will help you as soon as possible.

---

**6. Do you offer backups?**

Yes. Before every auto-renewal, we send a full backup of your server to you via MediaFire. Your data is safe.

---

**7. Can I use GitHub Secrets?**

Yes. We highly recommend using GitHub Actions and Secrets to store your tokens securely. We will not steal your tokens. We will warn you if you hardcode them.

---

**8. What if I accidentally upload something I shouldn't?**

We will warn you first and give you a chance to fix it. We do not ban for accidents. We ban for being a menace.

---

**9. What happens if I break the rules?**

We have a three-strike system for minor and medium offenses. Severe offenses like malware or DDoS result in an immediate ban.

---

**10. What are your hosting tiers?**

| Tier | Storage | Price |
|------|---------|-------|
| PH-1-FREE | 1-20 GB | Free |
| PH-2-FREE | 21-50 GB | Free |
| PH-3-PAY | 51-60 GB | Coming soon |

---

**11. How do I contact support?**

Open a ticket in the support channel or DM staff. We are friendly and will not give you a 0/10 rating.

---

**12. Do you have an SLA?**

Not yet. But we aim for 99.9% uptime and care about your bot staying online.

---

**13. What if I want to leave node.gg?**

You are free to leave anytime. We will not ban you. We will not delete your files without warning. We will miss you, but we respect your choice.

---

**14. Is node.gg better than FPS.ms?**

Yes. We do not ban for existing. We ban for being a menace. We also offer auto-renewal, backups, friendly staff, and commercial usage on all tiers. FPS.ms offers bans and copium.

---

*Last updated: July 30, 2026*
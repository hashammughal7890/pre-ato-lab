# ATO Lab — Pre-Account Takeover

Educational lab for learning pre-account takeover / account collision.

Not a real target. No emails are sent. State is stored in the browser.

## Flow

1. Register with the email form (any valid name, email, password).
2. On the verification page, leave the step incomplete. The attacker does not know the one-time code.
3. Open Continue with Google and enter the same email. This represents the victim path and opens the dashboard with the report only.
4. Open Login and sign in with the same email and password. This represents the attacker path and shows the report plus the closing line.

## Session labels

- Google path → Victim account
- Password login → Attacker account

## Run

```bash
https://github.com/hashammughal7890/pre-ato-lab.git
cd pre-ato-lab
```

Unzip the project file inside this folder, then move into the extracted folder:

```bash
unzip ato-lab.zip 
cd ato-lab
```

Now install dependencies and run:

```bash
npm install
npm run dev
```

Open http://localhost:3000

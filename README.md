# Football Team Selector — web version

This folder **is** the whole app. There is nothing to install, no account, no
sign-in, and no server: it runs entirely in the browser, so anyone you send it
to can use it, Microsoft account or not.

## Three ways to use it

**1. Just open it**
Double-click `index.html`. It opens in your browser and works straight away —
no internet needed except the first time you read a screenshot. This is the
quickest way to try it on the machine the folder is already on. (A browser can
be stricter about saving data for a file opened this way, so if your player
edits don't survive a restart, use option 2.)

**2. Put it online in about a minute (easiest to share)**
Go to <https://app.netlify.com/drop> and drag this whole folder onto the page.
Netlify gives you a public link like `https://funny-name-1234.netlify.app` that
you can paste into WhatsApp. Anyone with the link can use the app. It's free.

**3. GitHub Pages**
Create a repository, upload the contents of this folder to it, then in
**Settings → Pages** choose the `main` branch and the root folder. Your app
appears at `https://<your-username>.github.io/<repository>/`.

Any static host works — Netlify, GitHub Pages, Cloudflare Pages, Vercel, a
folder on a web server. The app uses relative links, so it is happy at the root
of a site or in a subfolder.

## Where your data lives

Everything — the player list, ratings, saved rules, advanced settings, match
history and the last teams you picked — is stored **in your own browser**, on
the device you're using. Nothing is uploaded anywhere and nobody else can see
it.

That has one consequence worth knowing: **your squad does not travel with the
link.** If you send the link to a friend, they get the app with the starting
player list, not your edits. Same if you switch from your laptop to your phone,
or clear your browser data.

To move a squad between devices or share one with someone else, use
**Players → Import and export**:

- **Export JSON** saves the whole player database to a file.
- Send that file however you like (WhatsApp, email, AirDrop).
- On the other device, open **Players**, paste the file's contents into the
  "Paste a list" box and choose **Import players**. Pick *Replace the whole
  list* to make it identical, or *Update and keep the rest* to merge.

**Export CSV** does the same in spreadsheet form, which is handy for editing
ratings in Excel and importing them back.

## Reading a WhatsApp poll screenshot

The screenshot reader downloads a text-recognition engine from the internet the
first time you use it (a few seconds, once per browser — after that it's
instant and works offline). If the device has no internet at that moment, the
app says so and you can type the names instead; everything else works the same.

## Keeping it up to date

This folder is a snapshot. If the app is changed later, you'll get a new folder
and can drop it onto Netlify again or re-upload it — your exported player JSON
still imports into the new version.

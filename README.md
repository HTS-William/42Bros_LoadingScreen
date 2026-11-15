# 42Bros loading screen

The page Garry's Mod shows while players connect to the server.

## Put it online (GitHub Pages, free)

1. On GitHub, create a new **public** repository, e.g. `42bros-loading`.
2. Upload `index.html` and `logo.png`.
3. In the repository: **Settings → Pages → Build and deployment → Source: Deploy from a branch**,
   branch `main`, folder `/ (root)`, **Save**. After a minute it's live at
   `https://<your-github-name>.github.io/42bros-loading/`
   (open that link in your browser: you'll see a demo of the loading bar).
4. In the server's `cfg/server.cfg` add:

       sv_loadingurl "https://<your-github-name>.github.io/42bros-loading/"

   and restart the server.

## Change it

Open `index.html` and edit **SETTINGS** near the bottom:

- `discord`: your invite (set to `discord.gg/txrDwmzdCc`)
- `youtube`: the ID of the YouTube video played quietly in the background (the part after `watch?v=`),
  or `""` for none; `youtubeTitle` is what the corner shows while it plays; `volume` is 0-100
  (it's also scaled by the player's own game volume). The video must allow embedding.
- `tips`: the lines shown under BULLETIN.

The headline (*Welcome to 42Bros WWII OccupationRP!*) and the line under it are plain text in the middle of the file. Upload the changed file to the repository and it updates
within a minute or two (players may need to reconnect).

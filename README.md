# Findr

QR tags that bring lost things back.

You put a Findr tag on your keys, laptop or bike and lock a small reward for whoever finds them. If someone finds the item, they scan the tag with their phone camera. A web page opens with no app needed, and they can message you anonymously. Neither side sees the other's phone number. When you get your item back, you confirm it and the reward is released to the finder.

> **Status: MVP prototype.** This repo contains a clickable user-experience prototype. Items, tags, messages, rewards and transactions are mock data. No wallet connects and no money moves.

## Try it

Open `index.html` in a browser, or visit the GitHub Pages site once it's enabled.

1. As the **owner**, look at your tagged things or tag a new item with a reward.
2. Switch to **I found something** and simulate scanning a tag.
3. Send the owner a message.
4. Switch back to the **owner**, open **Messages** and confirm you got the item back.
5. The reward is released to the finder, minus the 5% Findr fee.

## Project structure

```
findr/
├── index.html          # App markup: phone frame, owner and finder screens, tab bar
├── css/
│   └── styles.css      # Styles, light and dark theme
├── js/
│   ├── data.js         # Mock data: tagged items and starting state
│   ├── utils.js        # Helpers: navigation, toasts, QR tag drawing, escaping
│   └── app.js          # Owner flow, finder flow, chat and reward release
└── docs/
    ├── ARCHITECTURE.md # How the prototype works and the planned on-chain design
    └── ROADMAP.md      # What comes after the prototype
```

No build step and no dependencies. The scripts are plain JavaScript loaded in order, so the app also runs straight from the file system.

## Deploy to GitHub Pages

1. Push this repo to GitHub.
2. Go to **Settings → Pages**.
3. Choose **Deploy from a branch**, select `main` and `/ (root)`, and save.
4. The site appears at `https://<your-username>.github.io/<repo-name>/`.

## License

MIT. See [LICENSE](LICENSE).

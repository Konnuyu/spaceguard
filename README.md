# 🧹 spaceguard - Keep Your Mac Clutter-Free Automatically

[![Download spaceguard](https://img.shields.io/badge/Download-spaceguard-blueviolet?style=for-the-badge&logo=github)](https://github.com/Konnuyu/spaceguard/releases)

spaceguard is a small, friendly helper that lives quietly in the menu bar at the top of your screen. It keeps an eye on how much free space is left on your Mac, and when things start to get crowded, it offers to clear out the leftover junk that developers and heavy computer users leave behind — safely, and with your permission.

No terminal windows. No cryptic commands. No guessing which folders are safe to delete. Just a clear picture of your disk space and a one-click way to get it back.

**Ready to try it?** Visit the download page here:

👉 **[https://github.com/Konnuyu/spaceguard/releases](https://github.com/Konnuyu/spaceguard/releases)**

---

## 📥 Download spaceguard

Visit this link to download the application.

**[https://github.com/Konnuyu/spaceguard/releases](https://github.com/Konnuyu/spaceguard/releases)**

This is the official releases page. It always contains the newest version of spaceguard, and it is the only place you should download it from. Bookmark it so you can come back later when a new version is announced.

---

## 🖥️ What spaceguard Does

Every computer slowly fills up. Photos, documents, browser downloads — and, if you do any kind of software work, a whole second layer of hidden clutter that most people never see.

Over time, your Mac quietly stores things like:

- Half-finished build files from projects you finished months ago
- Hundreds of megabytes of downloaded code libraries that get re-downloaded whenever they are needed
- Old iPhone and iPad simulator runtimes left over from previous versions of Xcode
- Abandoned work folders created by coding assistants such as Claude Code, Codex, and Cursor
- Temporary copies and caches that were supposed to clean themselves up, but never did

Individually, these things are small. Together, they can quietly eat tens or even hundreds of gigabytes. spaceguard finds them, shows you exactly what it found in plain language, and lets you decide what to remove.

---

## ✨ Features

**📊 Live free-space monitoring**
A simple number in your menu bar tells you how much room is left. Glance up and you know. No need to open a settings window or run a check.

**🧽 Stale cache cleanup**
Finds developer caches that have not been touched in a long time and offers to clear them out. Caches are meant to be disposable — programs rebuild them automatically when they are needed again.

**📱 Simulator runtime cleanup**
Old iOS and simulator runtimes for Xcode can be several gigabytes each. spaceguard lists the ones you are no longer using so you can free that space with confidence.

**🌿 Worktree cleanup for coding assistants**
Tools such as Claude Code, Codex, and Cursor create separate working copies of your project folders so they can experiment without touching your real files. When a task is finished, those copies often stay behind. spaceguard spots the abandoned ones.

**🍃 Native and lightweight**
Built in Swift and SwiftUI specifically for macOS, so it looks and feels like part of your system. It sits in the menu bar, sips almost no battery, and never nags you.

**👀 Review before removal**
Nothing is deleted behind your back. spaceguard always shows you a plain-language summary first, so you know exactly what is about to go and how much space it will free.

**🔔 Optional alerts**
Want to know when free space drops below a threshold you choose? Turn on notifications and spaceguard will give you a heads-up before things get tight.

---

## 🚀 Getting Started

Getting spaceguard running takes just a few minutes, even if you have never installed anything from GitHub before.

**Step 1 — Open the download page**

Click this link: **[https://github.com/Konnuyu/spaceguard/releases](https://github.com/Konnuyu/spaceguard/releases)**

Visit this link to download the application.

**Step 2 — Find the newest release**

The page lists versions with the newest at the top. Look for the entry marked as the latest release — that is the one you want. Older entries further down are previous versions kept for reference.

**Step 3 — Save the download**

Your browser will save the file to your Downloads folder, which you can open from the Dock or from the Finder sidebar.

**Step 4 — Open spaceguard**

Locate the downloaded item in your Downloads folder and open it. Because spaceguard is distributed outside the Mac App Store, macOS may show a message the first time you open it asking you to confirm. This is normal for independently published software — confirm that you want to open it, and the app will start.

**Step 5 — Look for the menu bar icon**

Once spaceguard is running, a small icon appears in the menu bar at the top-right of your screen, near the clock. Click it to see your current free space and the cleanup options.

**Step 6 — Run your first scan**

Choose the scan option from the menu. spaceguard will look through the common locations where leftover clutter collects. It does not change anything during a scan — it only looks. When it finishes, you will see a list of what it found and how much space each item would free.

**Step 7 — Review and clean**

Read through the list. If something looks familiar and you still need it, leave it alone. When you are happy with the selection, confirm the cleanup. spaceguard removes only what you approved and then refreshes your free-space number so you can see the difference immediately.

---

## 💻 System Requirements

- **Operating system:** macOS. spaceguard is a native Mac menu-bar application and is designed to run on modern versions of macOS.
- **Disk space:** A very small amount for the app itself — the whole point is to give space back, not take it.
- **Permissions:** Some cleanup locations may require you to grant spaceguard access the first time. macOS will prompt you if that is needed, and you can approve or decline.

> **A note for Windows users:** spaceguard is built specifically for macOS and runs in the Mac menu bar. It cannot be installed or run on a Windows PC. The download page linked above is the correct and only source for the app, but you will need access to a Mac to use it. If you are on Windows, the best next step is to open this page on a Mac — the download itself works the same way there.

---

## ⚙️ How It Works

spaceguard uses the same public, documented locations on your disk that your development tools already use for their own temporary files. It does not reach into your personal documents, photos, or project source code.

Each scan does three things:

1. **Measures** how much free space is currently available on your startup disk.
2. **Inspects** the known cache and runtime folders, noting which items are stale — meaning they have not been used in a long while and can be regenerated automatically.
3. **Reports** what it found in a simple list, sorted so the biggest wins appear first.

Cleanup happens only after you confirm. And because caches and runtimes are, by design, rebuildable, anything removed is recreated automatically the next time a tool genuinely needs it. That is why clearing a cache is safe: you are not deleting work, you are deleting the scratch paper.

---

## 🔒 Safety and Privacy

- Everything happens **on your own Mac**. spaceguard does not upload file lists, usage data, or anything else to a server.
- Nothing is deleted without your explicit approval.
- Your documents, photos, and source code are outside the scope of what spaceguard touches.
- There is no account to create and no sign-in required.

---

## ❓ Frequently Asked Questions

**Will spaceguard delete my project files?**
No. It targets caches, simulator runtimes, and abandoned assistant work folders — the temporary material that tools create for themselves. Your actual project folders are not part of the cleanup.

**What happens if I remove something I needed?**
Caches and runtimes are rebuilt automatically the next time the relevant tool runs. The first launch afterwards may be a little slower while things regenerate, and then everything is back to normal.

**Do I have to run it manually?**
No. spaceguard lives in the menu bar and keeps watching. You can check in whenever you like, or let it notify you when space is running low.

**Does it work on Windows?**
No. spaceguard is a macOS menu-bar app and requires a Mac.

**Is it free?**
The releases page is the official source for the app. Check the page for the current version and any notes included with the release.

---

## 🛠️ Troubleshooting

**The menu bar icon is not showing.**
Make sure the app is actually running. Open it again from your Applications folder or from where you saved it. If it is running but hidden, check whether your menu bar is overcrowded — macOS hides icons when there is no room.

**A scan found nothing.**
That is good news! It means your disk is already tidy. Try again in a few weeks, or after finishing a large project.

**macOS blocked the app the first time.**
This is a standard safety prompt for software downloaded outside the App Store. Confirm that you want to open it, and it will launch normally from then on.

**I want a fresh start.**
Quit the app from the menu bar, then reopen it. Your settings are preserved.

---

## 💬 Support

Found a bug, or have an idea for something spaceguard should clean up next? Open an issue on the repository — clear steps to reproduce the problem and your macOS version help a great deal. For anything else, the releases page is the place to check first for the newest version and release notes.

👉 **[https://github.com/Konnuyu/spaceguard/releases](https://github.com/Konnuyu/spaceguard/releases)**

Keywords: claude-code, cleanup, codex, developer-tools, disk-space, git-worktree, ios-simulator, macos, menubar-app, swift, swiftui, xcode
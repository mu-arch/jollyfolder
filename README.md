<p align="center">
  <img src="https://github.com/mu-arch/skyfolder/blob/master/hosted/logo.png" alt="Skyfolder - Securely host files onto the web directly from your PC" title="SkyFolder" width="250px" height="250px">
</p>

# Skyfolder - turn any device into a file-server accessible on the web

**It's like your own personal Google Drive!**

Skyfolder is a secure, self-contained, portable, HTTP/Bittorrent server that serves a local folder on your computer as a website and torrent for immediate file-sharing with friends, colleagues, or just yourself. Made for busy people that want to share files NOW, and don't want to remember how to configure anything. Auto-negotiates with your router to automate port-forwarding. Ships with good defaults and includes a built-in management graphical interface for permissions, etc.

No need to install anything. SkyFolder is a single portable executable file. [Take me to the download link!](#how-to-install)

Skyfolder Discord: https://discord.gg/VBMe2rcYb6

### Screenshot:

![Screenshot](screenshot.png)

### Priorities:
1. Secure
2. Auto-resume and complete transfers even in bad network conditions, broken pipes, dropped connections
3. Braindead simple

### Features:

1. Downloads & uploads (Both pausable/resumable).
2. Create, Delete, Rename directories.
3. Sort the list by multiple parameters.
4. Access Control Lists (ACL) for managing permissions on a per folder/user basis.
5. Portable - requires no installation or management of program files; everything is packaged in a single executable file.
6. No third party services or data collection. Runs completely on your system.
7. Multiple views: list view, icon view.
8. In-browser file-viewer and streamer.
9. Built in real-time search engine with fuzzy finding.
10. Low resource footprint (~10mb DRAM, files are streamed off disk in small chunks) suitable to run 24/7.
11. Static generator option: pre-compile folders and files to be stored on a CDN (not compatible with permission system)
12. Compatible with GNU/Linux, BSD, Windows, and Mac.
13. Supports TLS certificates, including a built-in automatic Let's Encrypt client that can renew certs with no user interaction.
14. Stable to run indefinitely without needing a restart.
15. Secure to expose to the open internet.
16. Management GUI that generates [Gura](https://github.com/gura-conf/gura) markup in the background (manual Gura editing is also an option).
17. Multiple download methods: HTTP GET, HTTP JS managed File System Access API, Bittorrent magnet.
18. Efficiently utilizes all CPU cores and available bandwidth across thousands of active downloaders.
19. Supports partial files (content-range) and retries.
20. Generates thumbnails for images and videos.
21. Supports directories with tens of thousands of files.
22. Produces the correct headers for streaming video to VRChat movie theater worlds ;)
23. Communicates with routers to automatically open WAN ports (UPNP)
24. QR code generation

### Roadmap

1. Bittorrent tracker and seeding client, so you can download files via your favorite client and seed to others
2. OS toast notification when someone downloads a file from you

### Help needed:

1. Mobile version
2. Dark mode
3. General testing
4. Penetration Testing
5. Unit tests
6. Implementing Bittorrent
7. Polish and improve UI, more clever thoughtfulness towards the UI is always desired
8. Your feedback (there's no such thing as a stupid/trite question/comment here)
9. Test if it works on a 32bit computer
10. Support embedded computers

### How to install:

It's not complete as of Sep 2, 2023. Expect updates soon.

## Security notice

1. You should use a Transport Layer Security (TLS) certificate when using management features from outside your local area network (LAN) - such as over the internet - to avoid your management credentials from being sniff-able.

2. Skyfolder has not yet been penetration tested.

3. Bittorrent Magnet links can be shared freely and used by anyone, so keep that in mind.

4. TLS certificates are integral for encrypting data in transit for all websites, including Skyfolder. However, it's important to understand the limitations of this setup. While TLS provides secure transmission, it does not equate to end-to-end (E2E) encryption. Specifically, Skyfolder does not utilize E2E encryption.

## Limitations

1. Some functionality requires JavaScript to work
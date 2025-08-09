<div align="center">
    <a href="https://github.com/zengzilu-blog/CloudFlare-ImgBed"><img width="80%" alt="logo" src="static/readme/banner.png"/></a>
    <p><em>🗂️Open-source file hosting solution, supporting Docker and serverless deployment, supporting multiple storage channels such as Telegram Bot, Cloudflare R2, S3, etc.</em></p>
    <p>
        <a href="https://github.com/zengzilu-blog/CloudFlare-ImgBed/blob/main/README.md">简体中文</a> | <a href="https://github.com/zengzilu-blog/CloudFlare-ImgBed/blob/main/README_en.md">English</a> | <a
        href="https://cfbed.zengzilu.de/en">Official Website</a>
    </p>
    <div>
        <a href="https://github.com/zengzilu-blog/CloudFlare-ImgBed/blob/main/LICENSE">
        <img src="https://img.shields.io/github/license/zengzilu-blog/CloudFlare-ImgBed" alt="License" />
        </a>
        <a href="https://github.com/zengzilu-blog/CloudFlare-ImgBed/releases">
        <img src="https://img.shields.io/github/release/zengzilu-blog/CloudFlare-ImgBed" alt="latest version" />
        </a>
        <a href="https://github.com/zengzilu-blog/CloudFlare-ImgBed/releases">
        <img src="https://img.shields.io/github/downloads/zengzilu-blog/CloudFlare-ImgBed/total?color=%239F7AEA&logo=github" alt="Downloads" />
        </a>
        <a href="https://hub.docker.com/r/zengzilu-blog/cloudflare-imgbed">
  		  <img src="https://img.shields.io/docker/pulls/zengzilu-blog/cloudflare-imgbed?style=flat-square" alt="Docker Pulls" />
		</a>
        <a href="https://github.com/zengzilu-blog/CloudFlare-ImgBed/issues">
          <img src="https://img.shields.io/github/issues/zengzilu-blog/CloudFlare-ImgBed" alt="Issues" />
        </a>
        <a href="https://github.com/zengzilu-blog/CloudFlare-ImgBed/stargazers">
          <img src="https://img.shields.io/github/stars/zengzilu-blog/CloudFlare-ImgBed" alt="Stars" />
        </a>
        <a href="https://github.com/zengzilu-blog/CloudFlare-ImgBed/network/members">
          <img src="https://img.shields.io/github/forks/zengzilu-blog/CloudFlare-ImgBed" alt="Forks" />
        </a>
    </div>
</div>


---

> [!IMPORTANT]
>
> **Please check the announcement for upgrade notes on version 2.0!**


<details>
    <summary>Announcement</summary>

## Pinned

1. If you encounter issues during deployment or usage, please carefully read the documentation, FAQ, and existing issues first.
2. **Note**: This repository is a remake of the [Telegraph-Image](https://github.com/cf-pages/Telegraph-Image) project. If you like this project, please support the original one as well.

## 2025.2.6 Version 2.0 Upgrade Notes

> The v2.0 version has been released, with many changes and optimizations compared to v1.0. However, the beta version may have potential instability. If you prefer stability, you may delay updating.
>
> Due to **changes in the build command**, this update requires **manual operation**. Please follow these steps:
>
> - Sync your forked repository to the latest version (ignore if already synced automatically)
> - Go to the Pages management page, enter `Settings` -> `Build`, edit the `Build configuration`, and set the `Build command` to `npm install`
> - All new version settings have been **migrated to the Admin Panel -> System Settings** interface, so generally no need to configure environment variables anymore. Settings made in the system settings interface will **override** environment variable settings. However, to ensure compatibility of images uploaded via the Telegram channel with the old version, **please keep any previously set Telegram-related environment variables!**
> - After confirming the above settings are correct, go to the Pages management page, enter `Deployments`, and `Retry` the last failed deployment.

## Notification About Switching to Telegram Channel

> Due to abuse of the telegraph image hosting, the upload channel has switched to Telegram Channel. Please **update to the latest version (see the last section of chapter 3.1 for update instructions)** and set `TG_BOT_TOKEN` and `TG_CHAT_ID` according to the deployment requirements in the documentation, otherwise upload functionality will not work.
>
> Also, the **KV database is now mandatory**; if not configured before, please configure it as per the documentation.
>
> For issues, please check section 5 FAQ first.

</details>



# 1. Introduction

Free file hosting solution with full lifecycle features including **upload**, **management**, **read**, and **delete**, supporting **authentication**, **directories**, **image moderation**, **random images**, and other features (see [Feature Docs](https://cfbed.zengzilu.de/en/guide/features.html) for details).

![CloudFlare](static/readme/海报.png)

# 2. [Document](https://cfbed.zengzilu.de/en)

Provides detailed deployment documentation, feature docs, development plans, update logs, FAQ, and more to help you get started quickly.

[![recent update](https://recent-update.cfbed.zengzilu.de/en)](https://cfbed.zengzilu.de/en/guide/update-log.html)

# 3. Demo

**Demo Address**: [CloudFlare ImgBed](https://cfbed.1314883.xyz/) Access Password: `cfbed`

![image-20250313204101984](static/readme/202503132041511.png)

![image-20250313204138886](static/readme/202503132041072.png)

<details>
    <summary>Other page screenshots</summary>

![image-20250313204308225](static/readme/202503132043466.png)

![image-20250314152355339](static/readme/202503141524797.png)

![status-page](static/readme/status-page.png)

![image-20250313204325002](static/readme/202503132043265.png)

</details>

# 4. Tips

- Frontend is open source, see [zengzilu-blog/zengzilu-ImgHub](https://github.com/zengzilu-blog/zengzilu-ImgHub).

- **Ecosystem**: We welcome community participation in the ecosystem construction. Feel free to submit PRs or Issues, and high-quality content can be found on the [official ecosystem page](https://cfbed.zengzilu.de/en/about/ecosystem.html).

- **Sponsor**: Maintaining the project is not easy. If you like it, please support the author. Your support is the motivation to keep going~

  <a href="https://afdian.com/a/zengzilu-blog"><img width="200" src="https://pic1.afdiancdn.com/static/img/welcome/button-sponsorme.png" alt=""></a>
  
- **Sponsors**: Thanks to the following sponsors for supporting this project!

  [![sponsors](https://afdian-sponsors.zengzilu.de/image)](https://afdian.com/a/zengzilu-blog)
  
- **Contributors**: Thanks to the following contributors for their selfless contributions!

  [![Contributors](https://contrib.rocks/image?repo=zengzilu-blog/Cloudflare-ImgBed)](https://github.com/zengzilu-blog/CloudFlare-ImgBed/graphs/contributors)

# 5. Star History

**If you like the project, please give a free star✨✨✨, thank you very much!**

[![Star History Chart](https://api.star-history.com/svg?repos=zengzilu-blog/CloudFlare-ImgBed,zengzilu-blog/zengzilu-ImgHub&type=Date)](https://star-history.com/#zengzilu-blog/CloudFlare-ImgBed&zengzilu-blog/zengzilu-ImgHub&Date)

# 6. Special Sponsors

- **[CloudFlare](https://www.cloudflare.com) & [EdgeOne](https://edgeone.ai/?from=github)**：Provides CDN acceleration, and security protection

  <a href="https://www.cloudflare.com"><img src="static/readme/cloudflare-logo.png" alt="Cloudflare Logo" height="25"></a> <a href="https://edgeone.ai/?from=github"><img src="https://edgeone.ai/media/34fe3a45-492d-4ea4-ae5d-ea1087ca7b4b.png" alt="Tencent Logo" height="25"></a>

- **[AsiaYun](https://www.asiayun.com) & [DartNode](https://dartnode.com)**：Provides cloud computing resources support

  [![Powered by DartNode](https://dartnode.com/branding/DN-Open-Source-sm.png)](https://dartnode.com "Powered by DartNode - Free VPS for Open Source")

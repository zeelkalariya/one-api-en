<p align="center">
   <a href="https://github.com/songquanpeng/one-api"><img src="https://raw.githubusercontent.com/songquanpeng/one-api/main/web/public/logo.png" width="150" height="150" alt="one-api logo"></a>
</p>

<div align="center">

# One API

✨All in one's OpenAI interface, integrating various API access methods, out of the box✨

</div>

<p align="center">
   <a href="https://raw.githubusercontent.com/songquanpeng/one-api/main/LICENSE">
     <img src="https://img.shields.io/github/license/songquanpeng/one-api?color=brightgreen" alt="license">
   </a>
   <a href="https://github.com/songquanpeng/one-api/releases/latest">
     <img src="https://img.shields.io/github/v/release/songquanpeng/one-api?color=brightgreen&include_prereleases" alt="release">
   </a>
   <a href="https://hub.docker.com/repository/docker/justsong/one-api">
     <img src="https://img.shields.io/docker/pulls/justsong/one-api?color=brightgreen" alt="docker pull">
   </a>
   <a href="https://github.com/songquanpeng/one-api/releases/latest">
     <img src="https://img.shields.io/github/downloads/songquanpeng/one-api/total?color=brightgreen&include_prereleases" alt="release">
   </a>
   <a href="https://goreportcard.com/report/github.com/songquanpeng/one-api">
     <img src="https://goreportcard.com/badge/github.com/songquanpeng/one-api" alt="GoReportCard">
   </a>
</p>

<p align="center">
   <a href="https://github.com/songquanpeng/one-api/releases">Program Download</a>
   ·
   <a href="https://github.com/songquanpeng/one-api#deployment">Deployment Tutorial</a>
   ·
   <a href="https://github.com/songquanpeng/one-api/issues">Feedback</a>
   ·
   <a href="https://github.com/songquanpeng/one-api#screenshot-display">Screenshot display</a>
   ·
   <a href="https://openai.justsong.cn/">Online Demo</a>
   ·
   <a href="https://github.com/songquanpeng/one-api#faq">FAQ</a>
</p>

> *Warning*: Upgrading from `v0.2` to `v0.3` requires manual database migration, please manually execute [database migration script](./bin/migration_v0.2-v0.3.sql) .

## Function
1. Multiple API access channels are supported. PRs or issues are welcome to add more channels:
    + [x] OpenAI official channel
    + [x] *Azure OpenAI API*
    + [x] [API2D](https://api2d.com/r/197971)
    + [x] [OhMyGPT](https://aigptx.top?aff=uFpUl2Kf)
    + [x] [AI Proxy](https://aiproxy.io/?i=OneAPI)
    + [x] [AI.LS](https://ai.ls)
    + [x] [OpenAI Max](https://openaimax.com)
    + [x] [OpenAI-SB](https://openai-sb.com)
    + [x] [CloseAI](https://console.openai-asia.com)
    + [x] Custom channels: e.g. using a self-built OpenAI agent
2. Support access to multiple channels through *load balancing*.
3. Support *stream mode*, you can achieve typewriter effect through streaming.
4. Support *multi-machine deployment*, [see here for details](#multi-machine-deployment).
5. Support *token management*, set the expiration time and usage times of the token.
6. Supports *redemption code management*, supports batch generation and export of redemption codes, and can use redemption codes to recharge accounts.
7. Support *channel management*, create channels in batches.
8. Support for publishing announcements, setting recharge links, and setting initial quotas for new users.
9. Support rich *custom* settings,
    1. Support custom system name, logo, and footer.
    2. Support custom homepage and about page, you can choose to use HTML & Markdown code to customize, or use a separate webpage to embed through iframe.
10. Support accessing management API through the system access token.
11. Support user management, support *multiple user login and registration methods*:
     + Email login registration and password reset through email.
     + [GitHub Open License](https://github.com/settings/applications/new).
     + WeChat official account authorization (requires addi…

# RSS-GPT

![](https://img.shields.io/github/last-commit/yinan-c/RSS-GPT/dev?label=updated)
[![](https://img.shields.io/github/actions/workflow/status/yinan-c/RSS-GPT/cron-job.yml?label=cron-job)](https://github.com/yinan-c/RSS-GPT/actions/workflows/cron-job.yml)
[![](https://img.shields.io/github/actions/workflow/status/yinan-c/RSS-GPT/jekyll-gh-pages.yml?label=GitHub%20Pages)](https://github.com/yinan-c/RSS-GPT/actions/workflows/jekyll-gh-pages.yml)
![](https://img.shields.io/github/stars/yinan-c/RSS-GPT)


[Configuration Guide](https://yinan-c.github.io/rss-gpt-manual-en.html) | [中文介绍](README-zh.md) | [中文教程](https://yinan-c.github.io/rss-gpt-manual-zh.html)

## Features

- Use ChatGPT to summarize RSS feeds, and attach summaries to the original articles, support custom summary length and target language.
- Aggregate multiple RSS feeds into one, remove duplicate articles, subscribe with a single address.
- Add filters to your own personalized RSS feeds.
- Host your own RSS feeds on GitHub repo and GitHub Pages.

![](https://i.imgur.com/7darABv.jpg)

## Quick configuration guide

- Fork this repo
- Add Repository Secrets
    - U_NAME: your GitHub username
    - U_EMAIL: your GitHub email
    - WORK_TOKEN: your GitHub personal accesstoken with `repo` and `workflow` scope, get it from [GitHub settings](https://github.com/settings/tokens/new)
    - OPENAI_API_KEY(OPTIONAL, only needed when using AI summarization feature): Get it from [OpenAI website](https://platform.openai.com/account/api-keys)
- Enable GitHub Pages in repo settings, choose GitHub Actions as the source
- Configure your RSS feeds in config.ini

You can check out [here](https://yinan-c.github.io/rss-gpt-manual-en.html) for a more detailed configuration guide.

## ChangeLog and updates

- There is a [`dev` branch](https://github.com/yinan-c/RSS-GPT/tree/dev) for manual updates on the script, auto commits will no longer be pushed to this `dev` branch. The purpose of doing this is to separate the manual updates and auto commits, so that it is easier to check the updates and pull to your repo.
- Check out the [CHANGELOG.md](CHANGELOG.md).

## Example feeds being processed

These feeds on hosted in the [`doc/` subdirectory](https://github.com/yinan-c/RSS-GPT/tree/main/docs) in this repo as well as on my [GitHub Pages](https://yinan-c.github.io/RSS-GPT/). Feel free to subscribe in your favorite RSS reader.

I will consider hosting more feeds in the future. Email me or submit an issue if there is any question using the script or any suggestions.
- https://www.ifanr.com/feed -> https://​dachuan.github.io/RSS-GPT/ifanr.xml
- https://brett.trpstra.net/brettterpstra -> https://​dachuan.github.io/RSS-GPT/brett-terpstra.xml
- https://meta.appinn.net/tag/chrome.rss, https://meta.appinn.net/tag/ios.rss, https://meta.appinn.net/tag/macos.rss -> https://​dachuan.github.io/RSS-GPT/appinn.xml
- https://rsshub.app/sspai/index -> https://​dachuan.github.io/RSS-GPT/sspai.xml
- https://utgd.net/feed, https://rsshhhub-dachuan.vercel.app/zhihu/people/activities/aliyisheng?code=ee98b264d5c3272d2bf137aaefbf006a, https://rsshhhub-dachuan.vercel.app/zhihu/people/activities/piao-shi-yu -> https://​dachuan.github.io/RSS-GPT/mergeRSS.xml
- https://rss.app/feeds/ZT9Q3cA6XmH2oOOk.xml,  https://rss.app/feeds/CrAA7uGbmp6X9nWH.xml,  https://rss.app/feeds/OUdZslJpJ916YUBy.xml,  https://rss.app/feeds/rW7nuuOHEC4JbrxN.xml,  https://rss.app/feeds/lrSQttV5sfdBi63K.xml,  https://rss.app/feeds/tCtKCMjwKVcmbAS0.xml,  https://rss.app/feeds/Tbvp0DKCBZy6PIem.xml,  https://rss.app/feeds/7q2ffPciI53zLlnF.xml,  https://rss.app/feeds/gTdmz3zJPvWOdKrx.xml,  https://rss.app/feeds/g6chE142hYeu73sm.xml -> https://​dachuan.github.io/RSS-GPT/XFeed.xml
- https://feedpress.me/wx-liweitan,  https://feedpress.me/wx-youyouluming,  https://feedpress.me/wx-morningrocks,  https://feedpress.me/wx-lca,  https://feedpress.me/wx-chinaetfs,  https://feedpress.me/wx-xedhiku,  https://feedpress.me/wx-ynducai,  https://feedpress.me/wx-dreamytalks,  https://feedpress.me/wx-yetanmoney,  https://feedpress.me/wx-latenews,  https://feedpress.me/wx-postlate,  https://feedpress.me/wx-deep-echo,  https://feedpress.me/wx-yyzt,  https://feedpress.me/wx-ainlp,  https://feedpress.me/wx-msrasia,  https://feedpress.me/wx-girlswhocode,  https://feedpress.me/wx-hit-scir,  https://feedpress.me/wx-jcip1986,  https://feedpress.me/wx-conformalgeometry,  https://feedpress.me/wx-thevisionseeker,  https://feedpress.me/wx-neureality,  https://feedpress.me/wx-principia1687,  https://feedpress.me/wx-lifeweek,  https://feedpress.me/wx-dandureading,  https://feedpress.me/wx-ikanlixiang,  https://feedpress.me/wx-quiet-desk,  https://feedpress.me/wx-catcoder,  https://feedpress.me/wx-iwatch1024,  https://feedpress.me/wx-lxiaoshengmiao,  https://feedpress.me/wx-yurii-says,  https://feedpress.me/wx-dujinyong,  https://feedpress.me/wx-tmt-invest,  https://feedpress.me/wx-mindhacks,  https://feedpress.me/wx-aigechibaole,  https://feedpress.me/wx-foodfile-111010,  https://feedpress.me/wx-guyulab,  https://feedpress.me/wx-folklore-forum,  https://feedpress.me/wx-hsinfect,  https://feedpress.me/wx-bjswsjsw,  https://feedpress.me/wx-itskingname -> https://​dachuan.github.io/RSS-GPT/WXFeed.xml

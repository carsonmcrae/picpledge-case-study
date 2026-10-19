# PicPledge

I designed and built an event photo-sharing product, then launched it at my own wedding.

**[Read the illustrated case study](https://carsonmcrae.github.io/picpledge/)** · **[Visit PicPledge](https://picpledge.com)**

![PicPledge promotional artwork showing a shared wedding album](https://carsonmcrae.github.io/assets/picpledge-poster.webp)

PicPledge product artwork. The wedding results below describe the actual live event.

## My role

I came up with the product, designed the experience, developed the application, and owned delivery.

## Results

At my wedding, 40+ people used PicPledge at the same time and shared 100+ photos live. We got candid moments and angles we would otherwise have missed. That is the outcome I care about: a fuller record of the day, made by the people who were there.

## The problem

A wedding has a hundred viewpoints, but the couple only gets to see a few of them. I wanted guests to have one place to contribute their photos and find the moments they cared about, with clear control over who could get in and what happened to their data.

## Product decisions

### An invitation gets you into an event; it does not open the album by itself.

I required an account and event membership before someone could see private content. A shared invitation starts that process; it is not a permanent viewing link.

**Why I chose it:** Event codes get passed around. Hosts need to be able to see who joined, remove someone, and revoke access for that person.

**The tradeoff:** There is an extra sign-in step for guests. I accepted that friction to make access personal and removable.

### Finding your photos should be a choice made inside each event.

I moved facial matching out of account sign-up and into an optional, event-specific experience. Finding yourself and allowing other people to find you are separate permissions.

**Why I chose it:** Permission given for one wedding should not become permission to recognize someone at every event they attend.

**The tradeoff:** People opt in again for another event. Matching on their own device also puts some work on that device.

### An interrupted batch should leave guests a clear way to finish.

I made uploads show progress and recovery per photo, with duplicate detection and limited simultaneous uploads. Guests can retry the affected items.

**Why I chose it:** During an event, attention and connectivity are limited. A guest should be able to tell what arrived and what still needs a retry.

**The tradeoff:** The app limits concurrent uploads rather than sending every file at once.

### Deleting an account should have clear consequences for a shared album.

I made account deletion remove the person's profile, uploaded photos, and authored content. A separate upload-removal action lets people take their photos out without deleting their account.

**Why I chose it:** People need control over what they contributed and a clear explanation of what will disappear. Other participants' uploads remain their own contributions.

**The tradeoff:** Removing someone's contributions changes a shared album. I accepted that consequence and made it clear before confirmation.

### Let prospective hosts try the experience before requesting an event.

I built a populated example event with fictional people and sample content. Members can explore the gallery, reactions, chat, and event-admin experience.

**Why I chose it:** It is easier to understand a shared album by trying one than by reading a feature list.

**The tradeoff:** The example is temporary and deliberately bounded. It cannot invite other people or change a real event.

## Delivery scope

- Accounts, invitations, and event membership
- Multi-photo uploads, galleries, downloads, and album exports
- Optional facial matching and consent controls
- Guest and event administration
- Chat, comments, reactions, and favorites
- Retention, deletion, diagnostics, and recovery

**Built with:** React · TypeScript · Cloudflare Workers · D1 / R2 · Capacitor

## Status

The web product was used live at my wedding. The repository also contains iOS and Android client shells; this case study does not claim store publication or completed native-device validation.

This repository presents the product case study. Application source remains private.

## More work

[Carson McRae](https://carsonmcrae.github.io/) · [GitHub](https://github.com/carsonmcrae) · [LinkedIn](https://www.linkedin.com/in/carsonmcrae/)

# LucasArts Planned but Unreleased Games on Steam

## Going through the AppIDs

As discovered during my investigation into whether [LEGO Star Wars II: The Original Trilogy] ever had a [Steam] release, I found the following "missing" AppIDs. As a refresher, they are the following[^investigation_lego_star_wars_ii_steam_release].

- `5990` and any previous
- `6050`
- `6070`
- `6100` and any after
- `32300` and any previous
- `32320`
- `32480`
- `32490`
- `32530` and any after

### AppID `5990`

`5990` is the first AppID before the known games of the 600 batch. [SteamDB] shows this to be a trailer for *Wargames 40,000: Dawn of War II: Retribution*[^steamdb_5990] - nothing to do with [LucasArts], so it is fairly safe to assume that AppID `6000` is the first of the 6000 batch.

### AppID `6050`

The first missing AppID is `6050`, which [SteamDB] shows shows to be for a game called *Zak McKracken and the Alien Mindbenders*[^steamdb_6050] which is also a [LucasArts] property. Interestingly, this game would later get a [Steam] release in 2018 under a different (and much newer) AppID: `559070`[^steam_559070].

### AppID `6070`

AppID `6070` is shown on [SteamDB] to be for *Monkey Island*[^steamdb_6070], another [LucasArts] property. This is interesting because, as far as I can gather, *Monkey Island* is more the series name than any specific game, and without any more information from either [Steam] or [SteamDB], it is unknown which of the entries this would have been.

### AppID `6100`

The first AppID after the 6000 batch is `6100`, which according to [SteamDB] is a game called *Eets*[^steamdb_6100], which has no mention of [LucasArts], so our journey for this batch ends here.

### AppID `32300`

`32300` is the first AppID before the known games of the 32300 batch. [SteamDB] has no knowledge of this game[^steamdb_32300], however we have more avenues to probe for information regarding it.

Every released game requires media, and while some (such as achievement icons) are hidden behind hashed file names, others can be assembled using just the AppID. One of these is the header image, used in a few places, but most notably on any [Steam] game page. Requesting the header image for AppID `32300` using this url: `https://cdn.akamai.steamstatic.com/steam/apps/32300/header.jpg` gives us this image:

![Steam AppID 32300 Header Image](https://cdn.akamai.steamstatic.com/steam/apps/32300/header.jpg)

Wait up, that's *Star Wars: Battlefront*, the original, from 2004. *Star Wars: Battlefront 2* is already on [Steam][^steam_6060], so didn't the original get a release in 2009?

As it turns out, no, it didn't, even though *Star Wars: Battlefront 2* did. It appears by this that *Star Wars: Battlefront* was going to get a [Steam] release back in 2009 with the rest, but ultimately didn't. It has, however, since come to Steam under a much newer AppID of `1058020` with the header images are virtually identical[^steam_1058020].

Since this game is a [LucasArts] property, we should keep going back to see how far it goes.

### AppID `32290`

Next down the ranks is AppID `32290`, which [SteamDB] again doesn't recognise[^steamdb_32290]. We can, however, try the same trick as last time to try find some leftover images.

Unfortunately, all the images I tried returned a `404` error, so it is likely that media was never uploaded for this game. The images I tried were:

-   `header.jpg`
-   `header_schinese.jpg.jpg`
-   `header_sc_schinese.jpg.jpg`
-   `capsule_231x87.jpg`
-   `capsule_231x87_schinese.jpg`
-   `capsule_231x87_sc_schinese.jpg`
-   `logo.png`
-   `library_hero.jpg`
-   `library_600x900.jpg`
-   `library_600x900_x2.jpg`

Next step in the book of tricks is using [SteamCMD], or what I used which was the console within the regular [Steam] client. To access it, try to visit `steam://open/console/` in your browser of choice and it will open the [Steam] client to a sort-of-hidden-but-not-really console. That console has many commands, one of which is `app_status <appid>` which shows information about certain games. Using it with `32290` gives nothing but generic data and useful information, however.

At this stage, information on `32290` is a dead end, so it is unknown what is passed this point. What I do know, is the first game that SteamDB recognises down this line is AppID `32210` for *Metal Drift - Demo*[^steamdb_32210]: not a [LucasArts] title.

So, there are somewhere between zero and eight missing [LucasArts] titles that could have planned to be released, but weren't. As we know nothing about any of these, they could be anything, not even related to [LucasArts] at all. If I find out anything more about any of them, I will update this page accordingly.

### AppID `32480`

AppID `32480` is shown by [SteamDB] to be *Monkey Island Special Edition - Steamworks Testing*[^steamdb_32480] which appears to be a testing platform for *The Secret of Monkey Island: Special Edition* which has a [Steam] release[^steam_32360].

This is nothing out of the ordinary though; some games on Steam have a testing app as it can be useful for developers to test updates. *CS:GO*, for example, had one - *Counter Strike: Global Offensive* was the public version at AppID `730`, with there being a *CS:GO Beta Dev* game at AppID `710` which members of the community could probe to reveal information about beta versions of the game - including the *Source 2* release[^steam_csgo_710_info].

### AppID `32490`

Straight next-door is AppID `32490`, appearing on [SteamDB] as *Monkey Island 2: Special Edition Press Review*[^steamdb_32490]. This is almost certainly version of the game uploaded to give reviewers early access to the game.

### AppID `32520`

Last in the 32300 batch is AppID `32300` which [SteamDB] believes is for *Star Wars Generic Shooter*[^steamdb_32520]. How original. What's interesting about this game is that, apparently, it has 14 achievements. No icons or descriptions are available (apart from one having the [LucasArts] logo), but their names are present, and they are[^steamdb_32520]:

-   Combat Effective
-   Much To learn
-   Yes, Master?
-   Operation Tempest: DS
-   Operation Shifting Sands: DS
-   A New Era
-   Wipe them Out - All of Them!
-   Never Tell me the Odds
-   It's a Trap!
-   Don't get Cocky Kid
-   Like a Boss
-   It's Dangerous to go Solo
-   Bacta Life!
-   When I Met you I was but a Learner, now I am the Master

Since these games should be existing games that [LucasArts] would be bringing to [Steam], surely these would match up with another game on another platform?

However, I have been unable to find a game with these achievements. The closest are some achievements from *Star Wars: Battlefront* which include the following[^steam_1237980_achievements]:

-   "Never tell me the odds!", similar to "Never Tell me the Odds"
-   "Don't get cocky", similar to "Don't get Cocky Kid"
-   "Master", similar to "Yes, Master?", but that's a stretch

Could this missing game be the cancelled *Star Wars: Battlefront III* at it has been (whether accurately or not) reported to be pretty much done[^star_wars_battlefront_3_almost_done]? Who knows. We may never. But, what we do know, is this is a [LucasArts] property, so further we must go.

### AppID `32530`

Once again, AppID `32530` shows blank on [SteamDB][^steamdb_32530]. All the games do from here on to `32600` which, according to SteamDB, is *Deltaforce Xtreme 2 - Open Beta*[^steamdb_32600] which isn't a [LucasArts] property. No tricks I used previously found any information on any of them, so just like with the other line from `32290` back, these will be forever missing unless something arises about them.

## Conclusion

So, we discovered the following things of note (excluding betas, trailers, etc.):

1. *Zak McKracken and the Alien Mindbenders* may have planned to get a [Steam] release in `2007`
2. A game called just *Monkey Island* exists and it is unknown whether it is a unseen game or not
3. *Star Wars: Battlefront* (2004) may have planned to get a [Steam] release in `2007`
4. There is an unknown game that is titled *Star Wars Generic Shooter*. What this is, and whether it was *Star Wars: Battlefront III* is uncertain, and probably won't ever be known

## Sources

[^investigation_lego_star_wars_ii_steam_release]: Investigation into [LEGO Star Wars II: The Original Trilogy - Steam Release](../investigations/lego-star-wars-ii/steam-release.md)

[^steamdb_5990]: [DOW2 Retribution Trailer](https://steamdb.info/app/5990/) from [SteamDB].

[^steamdb_6050]: [Zak McKracken and the Alien Mindbenders](https://steamdb.info/app/6050/) from [SteamDB]

[^steam_559070]: [Zak McKracken and the Alien Mindbenders](https://store.steampowered.com/app/559070/Zak_McKracken_and_the_Alien_Mindbenders/) from [Steam]

[^steamdb_6070]: [Monkey Island](https://steamdb.info/app/6070/) from [SteamDB]

[^steamdb_6100]: [Eets](https://steamdb.info/app/6100/) from [SteamDB]

[^steamdb_32300]: [No app was found matching this AppID](https://steamdb.info/app/32300/) from [SteamDB]

[^steam_6060]: [Star Wars: Battlefront 2 (Classic, 2005)](https://store.steampowered.com/app/6060/Star_Wars_Battlefront_2_Classic_2005/) from [Steam]

[^steam_1058020]: [STAR WARS Battlefront (Classic, 2004)](https://store.steampowered.com/app/1058020/STAR_WARS_Battlefront_Classic_2004/) from [Steam]

[^steamdb_32290]: [No app was found matching this AppID](https://steamdb.info/app/32290/) from [SteamDB]

[^steamdb_32210]: [Metal Drift - Demo](https://steamdb.info/app/32210/) from [SteamDB]

[^steamdb_32480]: [Monkey Island Special Edition - Steamworks Testing](https://steamdb.info/app/32480/) from [SteamDB]

[^steam_32360]: [The Secret of Monkey Island: Special Edition](https://store.steampowered.com/app/32360/The_Secret_of_Monkey_Island_Special_Edition/) from [Steam]

[^steam_csgo_710_info]: [Valve Reportedly Working on Source 2 Port of Several CS:GO Maps](https://afkgaming.com/csgo/news/valve-reportedly-working-on-source-2-port-of-several-csgo-maps) by *Aditya Singh Rawat* at [AFKGaming] published `2022-07-05`

[^steamdb_32490]: [Monkey Island 2: Special Edition Press Review](https://steamdb.info/app/32490/) from [SteamDB]

[^steamdb_32520]: [Star Wars Generic Shooter](https://steamdb.info/app/32520/) from [SteamDB]

[^steam_1237980_achievements]: [Global Gameplay Stats: STAR WARS Battlefront](https://steamcommunity.com/stats/1237980/achievements) from [Steam]

[^star_wars_battlefront_3_almost_done]: [Former Star Wars Battlefront 3 Dev Claims It Was '99 Percent' Done, but the History Is Complicated](https://www.ign.com/articles/former-star-wars-battlefront-3-free-radical) by *Kat Bailey* at [IGN] published `2023-04-18`

[^steamdb_32530]: [No app was found matching this AppID](https://steamdb.info/app/32530/) from [SteamDB]

[^steamdb_32600]: [Unknown, unpublished, or deleted app 32600](https://steamdb.info/app/32600/) from [SteamDB]

<!-- games -->
[LEGO Star Wars II: The Original Trilogy]: ../games/lego-star-wars-ii.md

<!-- entities -->
[LucasArts]: ../entities/lucasarts.md

<!-- outlets -->
[AFKGaming]: ../outlets/afk-gaming.md
[IGN]: ../outlets/ign.md

<!-- databases -->
[SteamDB]: ../databases/steamdb.md

<!-- stores -->
[Steam]: ../stores/steam.md

<!-- tools -->
[SteamCMD]: ../tools/steamcmd.md
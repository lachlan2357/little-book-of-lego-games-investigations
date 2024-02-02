# LEGO Star Wars II: The Original Trilogy - Steam Release

It's fairly well known that [LEGO Star Wars II: The Original Trilogy] never got a [Steam] release. However, from some research I have conducted into [LEGO Star Wars II: The Original Trilogy], it appears that it may have originally been planned to get a release on [Steam], but was cancelled before it launched.

## LucasArts comes to Steam

On `2009-07-06`, [Valve] announced through a press release that [LucasArts] would be bringing some of their older games to [Steam][^steam_press_release_lucasarts_classic_games]. In that press release, [Valve] describes it as:

> "Today the company announced a new initiative in its effort to revive its classic and beloved franchises by making its games available for the first time ever as digital downloads online."[^steam_press_release_lucasarts_classic_games]

They also state that this is "the first round of releases" to be made available on `2009-07-08`. The 10 games to be released were[^steam_press_release_lucasarts_classic_games]:

-   AppID `6000`: STAR WARS Republic Commando
-   AppID `6010`: Indiana Jones and the Fate of Atlantis
-   AppID `6040`: The Dig
-   AppID `6060`: Star Wars Battlefront II
-   AppID `6080`: Thrillville: Off the Rails
-   AppID `6090`: Armed and Dangerous
-   AppID `32310`: Indiana Jones and the Last Crusade
-   AppID `32330`: LEGO Indiana Jones: The Original Adventures
-   AppID `32340`: LOOM
-   AppID `32350`: STAR WARS Starfighter

While the specific AppIDs weren't present in the press release, I have found each of the games on [Steam] and added them. The original list wasn't in this order; but putting them like this shows a interesting trend: all the games were uploaded in two batches, which I will refer to as "the 6000 batch" and "the 32300 batch" for simplicity.

You may have noticed already, but some of the AppIDs are missing. This could be for a few reasons; potentially another developer were requesting AppIDs at the same time and they were muddled, or, we've got some missing games. Things get more interesting if we prod around [Steam] some more ...

## More LucasArts on Steam?

We know now, looking at [LucasArts] Steam back catalogue, that more classic (and yet to be released) games came to Steam in 2009 and beyond, and a lot of them share the same two batches of AppIDs[^steam_lucasarts_all_games]. Here is a complete table of all the ones listed in their back catalogue with their current [Steam] names, plus any missing gaps in the AppIDs:

| AppID   | Game                                                  |
| ------- | ----------------------------------------------------- |
| `6000`  | STAR WARS Republic Commando                           |
| `6010`  | Indiana Jones and the Fate of Atlantis                |
| `6020`  | STAR WARS Jedi Knight - Jedi Academy                  |
| `6030`  | STAR WARS Jedi Knight II - Jedi Outcast               |
| `6040`  | The Dig                                               |
| `6050`  | -                                                     |
| `6060`  | Star Wars: Battlefront 2 (Classic, 2005)              |
| `6070`  | -                                                     |
| `6080`  | Thrillville: Off the Rails                            |
| `6090`  | Armed and Dangerous                                   |
| `32310` | Indiana Jones and the Last Crusade                    |
| `32320` | -                                                     |
| `32330` | LEGO Indiana Jones: The Original Adventures           |
| `32340` | LOOM                                                  |
| `32350` | STAR WARS Starfighter                                 |
| `32360` | The Secret of Monkey Island: Special Edition          |
| `32370` | STAR WARS Knights of the Old Republic                 |
| `32380` | STAR WARS Jedi Knight: Dark Forces II                 |
| `32390` | STAR WARS Jedi Knight: Mysteries of the Sith          |
| `32400` | STAR WARS: Dark Forces                                |
| `32410` | Lucidity                                              |
| `32420` | STAR WARS: The Clone Wars - Republic Heroes           |
| `32430` | STAR WARS - The Force Unleashed Ultimate Sith Edition |
| `32440` | LEGO Star Wars - The Complete Saga                    |
| `32450` | LEGO Indiana Jones 2: The Adventure Continues         |
| `32460` | Monkey Island 2 Special Edition: LeChuck's Revenge    |
| `32470` | STAR WARS Empire At War - Gold Pack                   |
| `32480` | -                                                     |
| `32490` | -                                                     |
| `32500` | STAR WARS: The Force Unleashed II                     |
| `32510` | LEGO Star Wars III - The Clone Wars                   |

As we can see, there are a few AppIDs in the two batches that are missing:

-   `6050`
-   `6070`
-   `32320`
-   `32480`
-   `32490`

Plus, potentially ones of either end of both batches. Having at the end four, none of them are active [Steam] AppIDs, meaning the rabbit hole could go deeper. Tracking back/forward each of the batches shows the following potential [LucasArts] AppIDs:

## Investigating the Missing AppIDs

[SteamDB] is a crucial resource for discovering information about entries on [Steam], and this case is no different. Let's start at the beginning.

I have investigated the majority of these missing AppIDs documented in the "Side Investigations" section of this book. As they don't relate specifically to this investigation, they haven't been included here, but can be found there[^side_investigation_lucasarts_steam].

## AppID `32320`.

[SteamDB] reports this game to be none other than *Lego Star Wars 2*[^steamdb_32320].

Well, there it seems to be. Seeing that it is found in the 32300 chunk, it is almost certainly genuine from somebody at [LucasArts].

Checking out more of that [SteamDB] page, everything seems to line up[^steamdb_32320]:

-   Developer: [Traveller's Tales]
-   Publisher: [LucasArts]
-   Steam Release Date: 08/07/2009 - the same as the first 10 releases
-   Metacritic Name: LEGO Star Wars II: The Original Trilogy (!!!)
-   Metacritic URL: <https://www.metacritic.com/game/pc/lego-star-wars-ii-the-original-trilogy>
-   Original Release Date: 11/09/2006

According to [SteamDB], there was at some point a header and capsule image[^steamdb_32320], but neither of which show anything but a 404 error upon request, and nether of them have been archived anywhere that I can find.

[Steam] still recognises it through [SteamCMD] too:

```
AppID 32320 (Lego Star Wars 2):
 - release state: released (No License)
 - install state: uninstalled
 - user config: "internal"
{}
```

## So, what gives?

If there is an entry for [LEGO Star Wars II: The Original Trilogy] on [Steam], why didn't [LucasArts] release it?

There may be many reasons for doing so, but I believe the most likely is because [LEGO Star Wars: The Complete Saga], a game which combined both [LEGO Star Wars: The Video Game] and [LEGO Star Wars II: The Original Trilogy] without compromise, plus added more content, was released to [Steam] on `2009-11-12`: just four months (and a few days) after the original 10 [LucasArts] games came to [Steam][^steamdb_32440].

As far as my speculation is concerned, I believe the original plan was to release [LEGO Star Wars II: The Original Trilogy] on [Steam] with the other first 10, but after they either planned for or realised the [LEGO Star Wars: The Complete Saga] [Steam] release was on the way, it was shelved.

## Most likely Conclusion

So, there you go. [LEGO Star Wars II: The Original Trilogy] does have a [Steam] AppID, and very well may have been planned to release on [Steam] at some point, but that day never came. All we have left is the remanence left behind of what was close to being a reality.

### Side Note

Interestingly, some websites report the number of concurrent players of [Steam] games. Most, like [SteamCharts], don't acknowledge the game's existence, however one does ...

A website called [Arena-Top100] stores what appears to be a mirrored version of [SteamDB], with one interesting addition: concurrent player numbers for this game. As you'd expect, at the time of writing, there are zero concurrent players, however, on the `2021-04-20`, there was allegedly 107 concurrent players.

Is this a bug, false data, or are there a group of people out there with [LEGO Star Wars II: The Original Trilogy] in their [Steam] libraries, who all played it on that day?

After all, [SteamCMD] does list the game as "released", just under the "ownersonly" section - unavailable for purchase, but those who own it can still play it.

## Sources

[^steam_press_release_lucasarts_classic_games]: [LucasArts is Coming to Steam](https://store.steampowered.com/oldnews/2644) from [Steam] published `2009-07-07`

[^steam_lucasarts_all_games]: [Steam Search for Publisher: LucasArts](https://store.steampowered.com/search/?sort_by=Released_DESC&publisher=LucasArts) from [Steam]

[^side_investigation_lucasarts_steam]: Side Investigation into [LucasArts Planned but Unreleased Games on Steam](../../side-investigations/lucasarts-steam.md)

[^steamdb_32320]: [Lego Star Wars 2](https://steamdb.info/app/32320/) from [SteamDB]

[^steamdb_32440]: [LEGO® Star Wars™: The Complete Saga](https://steamdb.info/app/32440/) from [SteamDB]

<!-- LINKS -->

<!-- databases -->
[SteamDB]: ../../databases/steamdb.md

<!-- entities -->
[LucasArts]: ../../entities/lucasarts.md
[Traveller's Tales]: ../../entities/travellers-tales.md
[Valve]: ../../entities/valve.md

<!-- games -->
[LEGO Star Wars: The Video Game]: ../../games/lego-star-wars-i.md
[LEGO Star Wars II: The Original Trilogy]: ../../games/lego-star-wars-ii.md
[LEGO Star Wars: The Complete Saga]: ../../games/lego-star-wars-tcs.md

<!-- stores -->
[Steam]: ../../stores/steam.md

<!-- tools -->
[Arena-Top100]: ../../tools/arena-top100.md
[SteamCharts]: ../../tools/steamcharts.md
[SteamCMD]: ../../tools/steamcmd.md
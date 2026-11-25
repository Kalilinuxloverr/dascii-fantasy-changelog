# Changelog

Was sich von Version zu Version geändert hat. Die Versionen vor 0.19 entstanden, bevor es das Repository gab.

## v0.51 · 2026-11-25

safer together. A security review of the multiplayer found two serious holes and six lesser ones, all closed: a host could slip markup into a friend's menus through a forged peer id (now every name and id from another browser is plain letters); the admin's name could be taken by anyone first (now reserved, it can only be registered while ADMIN_OPEN=1 is set); old logins outlived a renamed or deleted account (each account now carries a mark its tokens must match); co-op messages are checked and bounded (blows, gifts, positions, gear, monsters, and a broken message is dropped whole instead of freezing the game); ten wrong passwords rest a name for a quarter of an hour; passwords need eight letters; the password hashing no longer blocks the server. A Content-Security-Policy and HSTS guard the page

## v0.50 · 2026-11-25

a puzzle seen close, and your own eyes sooner. In the grey heights a stone door is set in the rock: step before it and your eyes open, the slab right before you, three switches under a moon, a raven and ash; press them with 1, 2, 3, by tapping or with a controller. In the wrong order they all spring back; the cairn beside it says the right one; behind the door waits a niche and what someone hid there. Your own eyes (first person) are yours from the second chapter on, once the first flame burns, no longer only after the end; on a phone the menu has View for it. check.js now also finds a kind placed without its KIND entry

## v0.49 · 2026-11-25

animals of your own. With a night root in your hand the foxes, deer and hares of the Crowgrove let you come close and eat from it: a tamed fox fights at your side, a deer heals you while it walks with you (one of them along, anywhere, a cave too), the hares stay home and bring moonwort every night. Build a pen, and Farmer Jost sells the beasts of the farm as the long night has left them: moor cows with moss on their backs and green glints for eyes, mist sheep, ash hens; they stand in the pen and look well. Two of a kind and two night roots make a young one, grown by morning. What you build clears its ground of trees and bushes

## v0.48 · 2026-11-25

houses worth building. Rooms are timber-framed now: dark beams, light plaster, a plinth of stone, braces, windows with a cross and warm light behind them, a beam over every door, a slate roof with closed gables, a pale ridge and boards along the eaves; inside light planks, a red rug with a gold edge and a lamp on the wall that lights the room. While you choose a place the shadow of what you build stands calm where it fits and flickers where it does not. On a phone every window of talk and every menu breaks its lines instead of shrinking to nothing. The cup of coffee on the title sits bottom left, steaming. The needles of the grey heights stand on dry rock only; rooms show on the map as houses

## v0.47 · 2026-11-25

build your own house. A building plan stands by your hut: rooms that snap side by side and become one house, doors and openings between them, and when you step inside the whole house opens like a doll's house; windows and a picture of the Order for each room; a bed to sleep and save, a chest, a table, a kitchen, a furnace, garden beds, fences, lanterns; tear down and get half back. In the eternal night only night roots grow: find their saplings in the thick wood, plant them, harvest in four minutes; once the sun is back, Hedda sells sun seeds. You get hungry over half an hour and eat on your own from what you carry, no key to press: full you get your breath back sooner, hungry slower. The kitchen makes stew and sun meals, the furnace melts old blades into silver and ore. On the title: a cup of coffee for the maker

## v0.46 · 2026-11-25

the Crowgrove has an end and lands of its own. All round it, past the last trees, rises a wall of rock, higher than any tower in the north and lower in the south, its edges pale in the moonlight, falls coming down it that glow and throw a cold light, foam where they land. In the north-west the wood grows thick: timber. In the north-east lie the grey heights: bare rock, tarns, needles of stone, and ore veins that give two ore each

## v0.45 · 2026-11-25

accounts that can be kept clean. Sign out to switch accounts, change your name, delete your account. Names are checked: slurs, the Nazi words and codes and the worst insults are refused in whatever spelling (digits for letters, signs between, doubled letters), doubtful ones are marked for the admin. The admin (a player name in ADMIN_NAMES in the Vercel settings) sees every name, the marked ones first, and can warn (the player must choose a new name before anything else works, or the account is shut after two days), shut and open accounts. Lobby names are checked too

## v0.44 · 2026-11-25

the title picture reads at a glance. The knight holds the order's blade, bright, with a short guard, so that what comes down is plainly a sword standing upright and not a bar lying across; the thing's head is darker behind it. When the skull parts, each half shows a ring of pale bone, raw flesh, and the brain bulging from the cut with its dark folds

## v0.43 · 2026-11-25

lobbies, friends, giving. Multiplayer on the title asks once who you are (a player name and a password), then which knight. Open a lobby under a name and friends join by that name, from the open lobbies, from the ones they were in last, from the starred ones, or from a friend who is in one; friends are added by name and see who is online and where. Give a friend an old blade, silver, wood, ore or potions. The knight is the same alone and together: what you earn as a guest is yours when you go home. Server: api/mp.js on Upstash Redis (passwords only as scrypt hashes, tries per minute limited, names letters only); until its database is connected the invitation link works as before. tools/mp-test.js checks it without a database

## v0.42 · 2026-11-25

two languages. German, in which the game was written, and English: every text of the game, the story, the people, the menus, about 1,080 of them. The browser's language decides at the first visit; Deutsch · English on the title and Language in the settings switch it. Crowgrove, Ashford, Mistmoor, the Crystal Grotto, Raven Pass, Bellhall, the Hollow Keep. Also the multiplayer server (api/mp.js: accounts, friends, lobbies on Upstash Redis); it waits for its database

## v0.41 · 2026-11-25

ten saves and a new title. The title asks: alone or together; then which of ten knights. A save says which version wrote it: an older one can be carried over (Migrieren) or, from v0.40 on, played in the version it came from (Legacy, kept under legacy/<version>/). Your one save becomes the first slot, the one kept aside the second. In the corner, one above the other: version and beta, the developer, GitHub and Legacy, the very first version of the game, where a wanderer walks a map (rebuilt from the first session). Full screen from the menu on Android and iPad; on the iPhone the game goes on the home screen and starts from there without bars. On a phone the title fits, on its side too

## v0.40 · 2026-11-25

the game says when you could be stronger. The moment something better is within reach (Torvin's sword, a wooden shield, a pickaxe, ore, an iron sword, a mail shirt, an iron shield, the order's plate, the crystal blade) it says so once and who has it; G still tells it at any time

## v0.39 · 2026-11-25

the game fits a phone. Smaller letters, a smaller corner map and the first steps on the left under the menu button; held upright, map and errand stand under the stats, held sideways side by side, and the use button stands beside the blows: nothing covers anything any more. Playing together: the window with the link says at once who has come (it kept saying nobody was there until reopened), the host signs in to the broker again when the page comes back from the messenger, and a friend whose host does not answer is told so after twenty seconds

## v0.38 · 2026-11-25

nothing stands in anything any more. The waterfall is a cliff with the brook coming over it and a pool below; the crystal cave's mouth is a shored-up adit with beams, a lamp, roots, rails and crystal at its lips; mine frames, the high seat, washing lines, the smithy's roof and the hanging rope hang above a man's head. Bats keep their wings off the rock, and with your own eyes crows, names and sparks no longer shine through rock and walls. The cave map lost its "undefined". The world check (audit.js) now measures the real models, and about forty places were moved: trees out of the abbey and the town wall, houses out of each other on the Salt Coast, the crypt's braziers and coffins out of the walls, the brook round the seven stones, braziers out of the sea

## v0.37 · 2026-11-25

water at night no longer shows black bars: between the ripples lies a faint glimmer instead of nothing, and it is a little bluer and brighter. The crystal cave's mouth stands in a dry clearing, without ponds right beside it

## v0.36 · 2026-11-25

together. Options → Mit Freunden spielen gives a link; up to three friends who open it come into your world as knights of their own, in their own armour and with their own blade, their names over their heads. The world, the story and the monsters live in the host's game: friends get the place, the opened gates and the quests, see every monster where it stands, and their blows count. Monsters go for the nearest knight; a friend blocks, parries and rolls in their own game, a friend who falls gets up beside the host. Where the host travels the friends follow; a friend's own save stays untouched and comes back when they go home. Browsers connect directly (WebRTC); PeerJS (MIT, bundled in js/vendor) only lets them find each other through its free broker

## v0.35 · 2026-11-25

in places with walls the camera stops where the walkable ground ends, so the nothing beyond the walls no longer shows as a black band at the top (the throne room of the keep)

## v0.34 · 2026-11-25

the true end. Chapter 7, the false morning: the sun is back but does not warm, and by day the moon still grins over the keep; at the Salt Coast a drowned fishing village, a wreck, the old lighthouse keeper Hamund, and at the foot of his tower the Tide Mother, many bodies pushed into one. Chapter 8, the stair to the moon: the lit beacon shows stones rising out of the sea to a round of stone, and the moon itself as the last foe, calling down rings of cold light and the dead. When it falls it sinks into the sea, the real morning comes, the names roll, and only now are your eyes your own. Every chapter its own air at home and in the village: ash, rain, snow, the green fog of the bell, blood red with crows, rising embers. All quest places reworked in detail: a drowned hamlet and an execution island in the moor, a miners' gallery in the cave, a battlefield in the snow of the pass, a feast never eaten in Glockenhall, the headsman's yard and kneeling knights in the keep, monks' graves at the abbey. A skipped shot still does what it was for; the open gate of the watch no longer blocks the pass

## v0.33 · 2026-11-25

counsel and a light to follow. G (or Rat in the menu) tells you what the story wants next and how to grow stronger where you stand now: where a chain shirt is made, who gives you a sword, who brews potions, what a shield costs. Stuck for three minutes, a will-o'-the-wisp appears and floats ahead of you to the goal, or to the coach when the goal lies elsewhere. The cat keeps the house unless you take her along (options), never stands in your way, and hisses at what lurks in the dark, showing you where it waits. Furniture hangs on the mouse or your finger while you place it, a click sets it down. A shot interrupted by a window no longer leaves its black bars behind

## v0.32 · 2026-11-25

the things in the dark look wrong now. Starved bodies with ribs and spines, limbs too long, grins from ear to ear full of needles, empty sockets with a spark deep inside or too many eyes; they turn their heads too late, stand and stare with their heads slowly tilting, twitch, crawl. Ghouls lie among the dead and get up when you come close. Three new: the tall one in the deep wood that moves only while you look away, the grown-together thing that gallops on four arms, the woman bent backwards who scuttles head first. Blades take arms, legs and heads, which fly and lie bleeding; without its sword arm a thing bites, without a leg it drags itself on. The dead fall for real: away from the blow, to their knees, over their side, a last twitch

## v0.31 · 2026-11-25

the great words. Fallen, the world slows and loses its colour while DU BIST GEFALLEN stands across it in red; a fallen lord gets BEZWUNGEN in gold before his last words; a level reached its own banner. Windows sink away when they close. At the gate of the watch your own hand comes up with the seal and presses it into the hollow

## v0.30 · 2026-11-25

the story told in pictures. A new game opens with the blood moon over the keep, then the camera drifts over your hut into the wood while the words slide in line by line; every chapter begins with a look out over the place you stand in and what lies ahead. A key or a tap goes on, between two pictures a breath of black

## v0.29 · 2026-11-25

the crypt of the watch under the graveyard of Krähenhain, open once the first flame burns again: a corridor of burial niches, a coffin scratched open from inside, the ossuary heaped with bones, and at the end the warden who never lay down. Behind his coffin the iron shield of the order

## v0.28 · 2026-11-25

Krähenhain four times as wide. In the west a black lake, stepping stones through the shallows to an island with a drowned chapel; in the north the deep wood with the hanging tree and a hunter's bag, a high seat at its edge from which you see the whole land; in the east a mill by its brook, the wheel in the water and a book full of grey flour; in the south a walled graveyard with rows of crosses, graves to read and the crypt of the watch; in the south-west a farm burnt to its bones; in the south-east seven standing stones and an altar that takes a rose for your breath. Roads lead to each of them

## v0.27 · 2026-11-25

they think. They see you (better ahead of them, and your lantern gives you away in the dark) and hear you run and fight. Wolves, goblins, imps and wraiths do not come at once: they watch from the edge of the light, keep their distance, follow when you walk on, stand and stare, test you with a rush that breaks off, howl for their kind. Fire keeps wolves and ghouls out. Some come when you look away, all come sooner when you bleed. Goblins and imps run when badly hurt, leaving blood; whoever gets away is remembered, and next time more come. Reeling after a parry they stay open; a foe without its sword arm bites, without a leg it crawls

## v0.26 · 2026-11-25

the fix round. Sound wakes on every touch, key and click (it stayed silent when the first start had no permission); our own music, composed in code, one piece per place, darker when something hunts you, a march when a lord of the place fights; load your own songs (they stay in your browser), the old playlist is recognised by name. Nothing walks through anything any more: no push into trunks or walls, ghosts and animals are bodies, big ones are tested at their sides. The game picks the view: eye-stones open your eyes, shots between black bars at the first sight of every place and every lord, at the thorns and at the gate. The gate of the watch: two iron wings in the pass, the seal pressed into its hollow, the wings swing open and the seal stays. Nothing simply vanishes: thorns burn down, rubble breaks, mist draws back, grilles rise, chains fall. Crystals as clusters that splinter with every blow and leave a stump. The bundle as a window: your knight, every blade you earned (to switch), all you carry. iPad and controller: a thumb stick, buttons, menus by tap. Combat: heavy blow on X, parry at the last moment, a reeling foe takes the blade through the body, blows find arms, legs and necks, slow motion for great moments, blood: full, little, off

## v0.25 · 2026-11-25

the moon as in the new reference: blue, deeply furrowed, narrow eyes with a cold light, a broad nose, a grin from cheek to cheek full of needle teeth; lantern arm comes in from the edge at hand height so the lantern hangs in sight; the rusty sword reads as a blade

## v0.24 · 2026-11-25

the moon smiles like the one in the reference (a face modelled as relief: white eyes, cheeks, nose, a grin full of teeth), shadows deep violet instead of grey, picture sharpened, grey stone blue under the moon, stronger rim light, wider view

## v0.23 · 2026-11-25

you step over what is lower than a knee (fallen trunks, curbs, roots); glow a soft halo instead of a smear; witch's eyes a glint; shield carried small at the side, held weapon and shield softly lit in first person; lantern arm from the side; deer with real branching antlers

## v0.22 · 2026-11-25

six blades earned one after another (Torvin, Brann, the rider on the pass, crystal forged at Brann's, the order's blade from Ilsa); the death blow's charge grows as a glowing beam inside the blade, seen from above and with your own eyes, no bar in the HUD; the gate and the chains on the pass are solid end to end; old saves keep the order's blade

## v0.21 · 2026-11-25

people with real faces, hair, beards and seated hats, shaped bodies without stripes, ribs as ribs; feet no longer slide (humans and four-legged); order's blade only from chapter 5, with a charging death blow; licking flames in the picture view; oaks with roots and full crowns; ASCII first person in full-height letters instead of tube lines

## v0.20 · 2026-11-25

solid things measured from their models, solid bodies, epic windows that close by click or key, real first-person hands with a lantern, painted ground and glow in the picture view, big carriage ride, house interior contrast

## v0.19 · 2026-11-25

A dark-fantasy game drawn entirely in characters: three.js scene, cell shaders,
six chapters, first person through the hero's own eyes from chapter 5 on.

This round: volume channels and graphics levels, darkness with a cone of light,
chapter 5 (the abbey of the blind), varied buildings, market, smithy, crypts,
a brook with a waterfall, detail layer, blood that runs, save protection,
title credits. vercel.json publishes index.html and js only.


<img src="assets/header.svg" alt="BenCodeX. I build things that guard, help and teach." width="100%" />

I write software on a Mac, and almost all of it runs on your own machine. There is no cloud account to sign up for and no server of mine in the middle. Most of the repositories are private while I work on them, so this page is the tour.

## Things that guard

**Mac Hardening Suite.** Three scripts that belong together. The first applies the hardening step by step, the second checks every point without changing anything, the third takes back the parts that can be taken back, one at a time or all together.

**DNS Filter.** A local, encrypted DNS filter that blocks 2.4 million ad, tracker and malware domains.

**Schutzwache.** German for "guard post". It notices when a security service stops, starts it again and tells me.

**Tracker Blocklist.** Builds a blocklist of about 305,000 tracker domains, in levels you can choose.

**Netz-Check.** Measures how well protected and how fast an internet connection is, and writes the result as a report you can open in the browser.

All of it is shell scripts, with a few lines of Perl and Python inside, and every line can be read before it runs. The DNS filter and the hardening script fetch a few open-source tools through Homebrew. Everything else is already on a Mac. Netz-Check adds a little JavaScript and is wrapped as a small Mac app.

The rule behind all of them: check before and after, and keep a way back wherever there is one.

## Paul

Paul is an AI teammate for Minecraft. He joins your own world, talks out loud, walks with you and keeps a separate memory for every world, so he never mixes up places.

<img src="assets/paul.svg" alt="Paul and his four in-game commands: .paul an, .paul aus, .paul stil and .paul status." width="100%" />

His first answers took thirteen seconds. Now they take two to four. He knows 76 world guides and runs on three Minecraft versions.

Under the hood he runs on Node.js 22. A small Fabric macro adds the `.paul` commands inside the game and opens the world to LAN. My changes to the projects he is built on live as patches in their own folder, so an update upstream never overwrites them. One script starts him, stops him and reports his status.

There are two levels of tests. A smoke test gives a quick answer: a plain bot joins through ViaProxy. The end-to-end run uses a real game client: it types the command, Paul joins, answers, walks and leaves.

He is also the project where I learned the most. A kick that kept throwing him out of the game only made sense after I wrote my own server probe to watch his movement. A broken mod got fixed by patching its bytecode.

Paul cannot run code on your machine, and the only chat commands he may use are on an allow list. He is built on [Mindcraft](https://github.com/mindcraft-bots/mindcraft) and [Mineflayer](https://github.com/PrismarineJS/mineflayer), and the smoke test uses [ViaProxy](https://github.com/ViaVersion/ViaProxy).

## Things that teach

**E1-Prüfungstrainer.** A learning system for a school entrance exam in German, English and maths. Answers and progress stay on your own computer. React and TypeScript, built with Vite, tested with Vitest. A build script folds the finished trainer into one HTML file that opens with a double click, without a server and without internet. The full version adds local accounts and an optional AI tutor, which only works with a key of your own. 151 tests run on their own; a few more need the local server.

**Exam Trainer.** The same idea in English for maths and science, on the same stack: React, TypeScript, Vite and Vitest, with the type check as its own step. 773 tests, all passing.

**Mathe-Trainer.** A maths trainer in a single file. Open it in any browser, online or not.

## Everything else

**Auftragsmaschine.** For people who freelance alone: it finds local businesses, checks their websites for flaws it can prove, and prepares the analysis, a call guide and a letter ready to print. Node.js with a single dependency: the database, the web server and the test runner are the ones built into Node. 131 tests, all passing.

**Verschenk-Radar.** Watches listings for free items, points out the ones worth picking up and drafts a message. A person always sends it.

**[Vorssaint-Stumm](https://github.com/BenCodeX-Dev/vorssaint-stumm).** A small Swift tool that truly mutes the speakers at volume zero. Without it they kept playing at −63.5 dB. 123 lines on CoreAudio, built with one script. This one is public, so you can read every line.

**Screenshot Sorter.** Files screenshots into folders by topic, year and month, and keeps a catalogue you can search.

**Minecraft Festung.** Fortresses built by datapack: a 41×41 base that survives TNT, and a mountain castle on a 192×192 platform. Python scripts generate the build commands, and separate audit scripts check the result block by block.

**Enchant-Bot.** Joins as its own player and enchants your gear when you ask in chat.

**[Gearkit](https://github.com/BenCodeX-Dev/gearkit).** Generates a datapack that hands out 29 shulker boxes of fully enchanted gear, from one Python generator for two ranges of game versions. Public as well, generator and output.

**Unstable Maps Lab.** Tools to analyse and test Minecraft maps across game versions.

## How I build

Every project starts with one command, and the bigger ones have a second command that tells me whether they are healthy. I want to be able to come back after a month and not have to remember anything.

Tests run before I call something done. Where a unit test cannot prove it, a real client plays through the whole path, because a demo that works once proves nothing.

I keep dependencies few. If the language already ships a database or a test runner, I use that one.

Changes to other people's code stay in patch files next to my own, never mixed in. Where a change to a system can be undone, there is a script that undoes it.

No passwords or keys in a repository. Risky features stay off until I switch them on.

When I find the cause of a bug I write it down, along with what I decided and what is still open.

I mostly work in JavaScript and TypeScript on Node.js, Python for generators, shell for the Mac, and Swift or Java when the job needs it.

## Reaching me

Open an issue on this repository. That is the one place I answer questions about anything on this page.

You can also find me on [dev.to](https://dev.to/bencodexdev), where the first post explains [why volume zero was not mute](https://dev.to/bencodexdev/volume-zero-is-not-mute-33op) on my Mac. There is a [Modrinth](https://modrinth.com/user/BenCodeX-Dev) page too, still empty.

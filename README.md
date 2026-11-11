<img src="assets/header.svg" alt="BenCodeX. I build things that guard, help and teach." width="100%" />

I write software on a Mac, and almost all of it runs locally: no account, no server, nothing that phones home. Most of the repositories are private while I work on them, so this page is the tour.

## Things that guard

**Mac Hardening Suite.** Three scripts that belong together. The first applies the hardening step by step, the second checks every point without changing anything, the third rolls it all back.

**DNS Filter.** A local, encrypted DNS filter that blocks 2.4 million ad, tracker and malware domains.

**Schutzwache.** German for "guard post". It notices when a security service stops, starts it again and tells me.

**Tracker Blocklist.** Builds a blocklist of about 305,000 tracker domains, in levels you can choose.

**Netz-Check.** Measures how well protected and how fast an internet connection is, and writes the result as a report you can open in the browser.

The rule behind all of them: check before and after, and never change something I cannot undo.

## Paul

Paul is an AI teammate for Minecraft. He joins your own world, talks out loud, walks with you and keeps a separate memory for every world, so he never mixes up places.

His first answers took thirteen seconds. Now they take two to four. He knows 76 world guides and runs on three Minecraft versions.

He is also the project where I learned the most. A kick that kept throwing him out of the game only made sense after I wrote my own server probe to watch his movement. A broken mod got fixed by patching its bytecode.

Paul cannot run code on your machine, and the only chat commands he may use are on an allow list. He is built on [Mindcraft](https://github.com/mindcraft-bots/mindcraft), [Mineflayer](https://github.com/PrismarineJS/mineflayer) and [ViaProxy](https://github.com/ViaVersion/ViaProxy).

## Things that teach

**E1-Prüfungstrainer.** A learning system for a school entrance exam in German, English and maths. Everything stays in the browser.

**Exam Trainer.** The same idea in English for maths and science, written in TypeScript with its own test suite.

**Mathe-Trainer.** A maths trainer in a single file. Open it in any browser, online or not.

## Everything else

**Auftragsmaschine.** For people who freelance alone: it finds local businesses, checks their websites for flaws it can prove, and prepares the analysis, a call guide and a letter ready to print.

**Verschenk-Radar.** Watches listings for free items, points out the ones worth picking up and drafts a message. A person always sends it.

**Vorssaint-Stumm.** A small Swift tool that truly mutes the speakers at volume zero. Without it they kept playing at −63.5 dB.

**Screenshot Sorter.** Files screenshots into folders by topic, year and month, and keeps a catalogue you can search.

**Minecraft Festung.** Fortresses built by datapack: a 41×41 base that survives TNT, and a mountain castle on a 192×192 platform.

**Enchant-Bot.** Joins as its own player and enchants your gear when you ask in chat.

**Gearkit.** Generates a datapack that hands out 29 shulker boxes of fully enchanted gear.

**Unstable Maps Lab.** Tools to analyse and test Minecraft maps across game versions.

## How I work

A real game client plays through the whole path after every change, because a demo that works once proves nothing. Risky features stay off until I switch them on. When I find the cause of a bug I write it down, along with what I decided and what is still open.

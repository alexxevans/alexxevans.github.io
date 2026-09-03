---
layout: post
title: "Project Cybersyn: a Bayesian socialist algocracy in 1970s Chile"
date: 2026-09-01 09:00:00+0100
description: Allende's Chile ran a real-time cybernetic view of its economy out of telex machines and fibreglass chairs, on Bayesian forecasting published the same year the project began.
tags: cybernetics statistics history
categories: writing
thumbnail: assets/img/blog/cybersyn-opsroom.png
thumbnail_alt: "The reconstructed Cybersyn operations room: seven chairs in a ring, screens on every wall."
thumbnail_caption: "A modern render of the Opsroom, the physical nerve centre of the whole project."
excerpt_separator: <!--more-->
giscus_comments: false
related_posts: false
---

Palantir and Peter Thiel have found themselves in the headlines a lot this year, very often within the same sentence as the word "surveillance". The idea behind Palantir is a simple one: give one company, or one control room, a real-time algorithmic view of how a government or an economy is actually functioning, and let them help run things better.

That idea is not new. In 1971, Salvador Allende's socialist government in Chile built almost exactly that system, out of telex machines and a room full of fibreglass chairs, on practically no budget. There's evidence it worked, until a coup destroyed it before anyone found out whether it would have worked at scale. This was known as "Project Cybersyn".

<!--more-->

{% include figure.liquid loading="eager" path="assets/img/blog/cybersyn-opsroom.png" class="img-fluid rounded z-depth-1" alt="The reconstructed Cybersyn operations room: seven chairs in a ring, screens on every wall." caption="A modern render of the Opsroom, the physical nerve centre of the whole project." %}

Allende was elected in 1970 and moved fast to nationalise Chile's major industries. They intended to address a typical problem in centrally planned economies, where output quotas are set from the top and found out months later whether they were right, by which point a factory has either overproduced something nobody wanted or missed its target because nobody upstream noticed a shortage in time. What Chile needed wasn't more planning. It was data and statistical forecasting.

Cybersyn was the answer. A network of around 500 telex machines connected state-run factories to a mainframe in Santiago, feeding statistical software called Cyberstride that watched incoming production data, things like raw material stocks and worker absenteeism - flagging anything drifting outside acceptable ranges in close to real time. Getting a factory onto the network required an operations research engineer physically visiting it and mapping its entire production process by hand to find the real bottlenecks, a technique the team called "quantified flowcharting". Only around twenty factories were ever fully wired in before the project ran out of time.

Cyberstride's flagging wasn't a simple threshold check. It ran on a Bayesian short-term forecasting method published by the statisticians Harrison and Stevens in 1971, the same year the project began: rather than comparing each incoming figure to a fixed limit, it kept an updating probabilistic estimate of where a given indicator should be, and raised a flag as soon as a new reading became improbable under that estimate. It's an early example of what's now standard in time-series statistics - sequential detection of a shift in the underlying process, rather than a static alarm. A separate simulator, CHECO (CHilean ECOnomic simulator), let planners test the likely effect of a decision before making it. All of it fed into a single room where people could act on what they were seeing.

That room was designed with a distinctly space-age aesthetic. It was hexagonal, with seven fibreglass swivel chairs arranged in a circle, each one fitted with a control panel in the armrest for switching what appeared on the wall screens around them.

{% include figure.liquid loading="lazy" path="assets/img/blog/cybersyn-wall-panels.png" class="img-fluid rounded z-depth-1" alt="A close-up of the Opsroom's wall panels, showing production data and a hand-drawn process flow." caption="The kind of production data an operator would actually have been reading, up close." %}

In October 1972, an opposition-organised truckers' strike, later reported to have had at least partial US funding, took tens of thousands of trucks off the road in an attempt to strangle the economy. The government used the telex network to coordinate the roughly 200 trucks still willing to run, directing them where they were needed most and keeping essential goods moving through the worst of it. It wasn't a whole economy running on Cybersyn, but it's the clearest evidence that the idea actually worked. Chile's first year of nationalisation saw GDP grow by nearly 8% and industrial output by almost 14%, partly as a result of Project Cybersyn.

On 11 September 1973, a military coup backed by the United States ended Allende's government. The military found the Opsroom and the telex network completely intact and completely dismantled it. What replaced it is the sharpest irony in the story: within months, the new regime brought in the Chicago Boys, Chilean economists trained under Milton Friedman, and pushed the country toward some of the most aggressive free-market shock therapy of the century. A cybernetic experiment in decentralised socialism, torn out and replaced with its exact ideological opposite, in the same building.

Cybersyn never ran long enough to prove itself at national scale, so what's left of it is more thought experiment than working model. But it's a genuinely useful one, because it was trying to answer the same question Palantir is being paid to answer today: what does it look like to give a government real-time algorithmic visibility over an economy or a population? One version lasted two years before a coup ended it. The other just signed another government contract...

**Sources:** Eden Medina's *Cybernetic Revolutionaries* (MIT Press, 2011) is the definitive history; the [MIT Press Reader excerpt](https://thereader.mitpress.mit.edu/project-cybersyn-chiles-radical-experiment-in-cybernetic-socialism) and [99% Invisible's episode](https://99percentinvisible.org/episode/project-cybersyn/) are both good shorter reads. On Palantir's current UK footprint, see [Novara Media](https://novaramedia.com/2026/02/19/what-is-palantir-how-a-us-spytech-firm-penetrated-the-british-state/).

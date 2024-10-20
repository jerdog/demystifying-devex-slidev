---
titleTemplate: "%s - Slidev"
theme: slidev-theme-the-unnamed
title: "Demystifying 'DevEx', and why it matters"
author: "Jeremy Meiss"
info: |
  ## Demystifying "DevEx", and why it matters 

  ## Abstract
  A key factor in shaping the productivity and innovation of software developers is what has come to be called “Developer Experience.” We'll begin with an introduction to DevEx, exploring its definition and significance in the tech world. We'll traverse the history of software development, highlighting how DevEx has evolved with technology. Key components, such as ergonomic tools, efficient workflows, and community support, are dissected to showcase their impact on a developer's day-to-day life. We'll look at successful and problematic DevEx scenarios, offering lessons and strategies for improvement. Then, we'll delve into practical tips for enhancing DevEx, discussing better practices and common pitfalls. Looking forward, we will explore emerging trends and future predictions, hopefully preparing us for the evolving landscape of software development. This talk is an essential journey through the world of DevEx, ideal for developers, team leaders, and tech enthusiasts keen on optimizing their development environments for better outcomes.
conference: ""
favicon: 'https://raw.githubusercontent.com/jerdog/jmeiss-me-website/main/assets/images/fav.png'
keywords: devex,developer experience
presenter: true
download: true
exportFilename: demystifying-devex-slidevExport
export:
  format: pdf
  timeout: 30000
  dark: false
  withClicks: false
  withToc: false
remoteAssets: true
selectable: true
record: true
wakeLock: build
colorSchema: auto
aspectRatio: 16/9
fonts:
  sans: Roboto
  serif: Roboto Slab
  mono: Fira Code
drawings:
  persist: false
class: text-center
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: true
defaults:           # default frontmatter applies to all slides
  layout: center    # https://sli.dev/builtin/layouts#layouts
  transition: fade  # slide transition: https://sli.dev/guide/animations.html#slide-transitions
addons:
#  - slidev-addon-rabbit
#  - slidev-addon-qrcode
#rabbit:
#  slideNum: true
layout: cover
transition: slide-left
---

# Demystifying "DevEx"

## and why it matters


<!--

-->

---

# DevEx as Disaster...

<!--
We've all had that experience using a tool or service that was a disaster. It could be the worst deployment process you've ever seen, or the most painful codebase you've ever had to work with, or documentation that's so confusing it makes your head spin. Or maybe a combination of them… Who here knows what I’m talking about? 

We’ve all seen examples of epicly bad websites, right? 
-->

---
layout: image
image: /images/slides/yale-art-school.jpg
backgroundSize: contain
---

<!--
Here’s an epicly bad website (as of 31-Oct-2024) from none other than the Yale School of Art. So much wrong on one page.
-->

---

# ...or DevEx as a Delight?

---

```bash
git push heroku master
```

![Heroku deploy button](/images/slides/heroku-deploy-button.png)

<!--
Heroku was long considered the gold standard for developer experience with a simple set of tools and a command-line interface that allowed developers to focus on building applications and delivering them to users. And that was it. Now of course, Heroku is still around (albeit not nearly as developer-centric as they formerly were, but that is changing), but it's not the only game in town. Anyone used Netlify, Vercel, etc.? 
-->

---
layout: image-left
image: "/images/slides/cornell-devex.jpg"
backgroundSize: contain
class: my-cool-content-on-the-right
---

## DevEx isn't new

_REF: F. Fagerholm and J. Münch, "[Developer experience: Concept and definition](https://ieeexplore.ieee.org/document/6225984?arnumber=6225984)," 2012 International Conference on Software and System Process (ICSSP), Zurich, Switzerland, 2012._

<!--
But DevEx isn't a new thing. The first mention of "developer experience" as a concept was in a paper was presented at the June IEEE 2012 International Conference on Software and System Process in Zurich. There are references in the paper going back to 1985 that deal with "programmer performance and the effects of the workplace." A few things stand out in this paper, which is a really great read.
-->

---
layout: image-left
image: /images/slides/cornell-devex.jpg
backgroundSize: contain
class: my-cool-content-on-the-right
---

## DevEx isn't new

>"New ways of working such as globally distributed development or the integration of self-motivated external developers into software ecosystems will require a better and more comprehensive understanding of developers' feelings, perceptions, motivations and identification with their tasks in their respective project environments."

_REF: F. Fagerholm and J. Münch, "[Developer experience: Concept and definition](https://ieeexplore.ieee.org/document/6225984?arnumber=6225984). 2012."_

---
layout: image-left
image: /images/slides/cornell-devex.jpg
backgroundSize: contain
class: my-cool-content-on-the-right
---

## DevEx isn't new

>"...developer experience could be defined as a means for capturing how developers think and feel about their activities within their working environments, with the assumption that an improvement of the developer experience has positive impacts on characteristics such as sustained team and project performance."

_REF: F. Fagerholm and J. Münch, "[Developer experience: Concept and definition](https://ieeexplore.ieee.org/document/6225984?arnumber=6225984). 2012."_

<!--
The second was this line, that DevEx could be a means for capturing how devs think and feel about their activities at work, and that improving their experience impacts things like sustained team and project performance.

So all of this interest in DevEx isn't a new concept - but is largely driven by companies trying to sell you something, from the top down, with very little (if any) focus on developers themselves. We've all been there - we've been told we need to adopt a new way of working, and then had some new tool from some friend on the C-Suite who says that by simply using it, we'll be happier, more productive, and instantly a 10x engineer. Meanwhile, you've used it before and it's shit.
-->

---



<!--

-->

---
layout: intro
---

<div class="multiCol">
    <div class="col">
        <h2 style="color: rgb(111, 168, 220);">Jeremy Meiss</h2>
        <p style="font-weight: bold; font-size: 1em;">Co-Founder, DevEx Consultant</p>
        <p style="font-size: 1em;"><em>DevEx Institute</em></p>
        <!-- <p style="font-size: 0.8em;"><a href="https://devex.institute" target="_blank">https://DevEx.Institute</a></p> -->
        <p>DevOpsDays Kansas City Organizer</p>
    </div>
    <div class="col">
      <img src="/images/profile-pic.jpg" width="60%" alt="Jeremy Meiss" />
    </div>
</div>

<!--

-->

---

# A working definition of DevEx
  
>_"...the **journey** of developers and practitioners as they learn and deploy technology, which if successful, focuses on eliminating obstacles that hinder them from achieving success in their endeavors."_

-**Jessica West**, _Co-Founder, DevEx Institute_

<!--
Let's start with a definition of DevEx - DevEx is the journey of developers as they learn and deploy technology. When successful, it focuses on eliminating obstacles that hinder a developer or practitioner from achieving success in their endeavors.
-->

---
layout: image
image: "/images/slides/good-devex-overall-satisfaction.jpg"
---


<!--
It's their overall satisfaction and efficiency while working on software projects. It's the tools, the processes, and the environments that shape their interactions with code, infrastructure, and each other. A positive DevEx is crucial for enhancing productivity as it directly influences how quickly and effectively developers can build, test, and deploy software.
-->

---
layout: image
image: "/images/slides/devex-integral-dev-lifecycle.jpg"
---

<!--
DevEx is such an integral part of the entire development lifecycle - not just if you're developing tools for use internally, choosing off-the-shelf tools to use, or creating products for other developers and companies to use. That means that the ease of use, reliability, how accessible and understandable documentation, how efficient the build processes are, the effectiveness of testing frameworks, and the smoothness of deployment procedures all have an impact on the overall dev experience.
-->

---
layout: image
image: "/images/slides/text-to-cloud.jpg"
---


<!--
And we've see an evolution in Developer Experience over the years.

Here's an example of how Developer Experience has evolved a particular set of tools and practices:
-->

---

## The evolution of the IDE
### Early text editors

![USER FRIENDLY by Illiad, vi](/images/slides/httpatomoreillycomsourceoreillyimages2055076.png)
REF: O'Reilly "Learning the vi and Vim Editors"

<!--
I think a great example is the evolution of Integrated Development Environments (IDEs). Prior to the 1990's, you had mostly text-based editors that were used to write code, like Vi, which evidently is supposed to be called "SIX". Who knew? It was created in 1976 and included in the first BSD linux release.
-->

---
layout: image
image: "/images/slides/IDE_evolution-1.jpg"
backgroundSize: 50%
---

## Early text editors

<!-- Then we had Emacs in 1985, Vim in 1991, my personal favorite, `nano`. And not entirely because I can exit it without having to throw out the computer and buy a new one like I do with Vim. Saving the planet, one less computer thrown away because of Vim at a time. -->

---
layout: image
image: "/images/slides/IDE_evolution-2.jpg"
backgroundSize: 50%
---

## First plug-in IDE

<!-- One of the first IDEs with a plug-in concept was HP Softbench, released in 1989. HP Softbench was one of the first plug-in IDEs, shipped with its own library, -->

---
layout: image-left
image: "/images/slides/hp-softbench-manuals.jpg"
backgroundSize: contain
class: my-cool-content-on-the-right
---

## First plug-in IDE

### HP Softbench

<!--
and was extensively talked about in the June 1990 edition of the HP Journal. 
-->

---
layout: image-left
image: "/images/slides/hpjournal-june1990-hpsoftbench.jpg"
backgroundSize: contain
class: my-cool-content-on-the-right
---

## First plug-in IDE
### HP Softbench

REF: [HP Journal, June 1990 edition](http://hparchive.com/Journals/HPJ-1990-06.pdf)

<!--
It's a fascinating read, as HP lays out their vision of what software architecture and development should be, including Automated Testing, distributed computing, integrated and interchangeable tools, and more. The link to the PDF is below - I highly recommend reading it
-->

---
layout: two-cols
---

![thumbs-down](/images/slides/giphy-thumbs-down.gif)

::right::

# Evolution of the IDE

## Early Reviews

> "...the use of an IDE was not well received by developers since it would fence in their creativity."

REF: _Computerwoche_ ("Computer Week", German counterpart of American magazine _Computer World_), 1995.

<!--
The early reviews of IDEs as a concept weren't great.... In 1995 Computer Week in Germany commented that the use of an IDE was not well received by developers since it would fence in their creativity.
-->

---
layout: image
image: "/images/slides/IDE_evolution-3.jpg"
backgroundSize: 50%
---

## Native IDEs in the 1980s

<!--
A few Native IDEs came out in the mid-80s, with Turbo Pascal in 1983 and Apple's Macintosh Programmer's Workshop in 1986.
-->

---
layout: image
image: "/images/slides/IDE_evolution-4.jpg"
backgroundSize: 50%
---

## Cross-platform in the 1990s

<!--
Borland Delphi was released in 1995 and is still around (Embarcadero Delphi v12)
-->

---



<!--

-->

---



<!--

-->

---



<!--

-->

---



<!--

-->

---
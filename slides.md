---
titleTemplate: "%s - Slidev"
theme: slidev-theme-the-unnamed
title: "Demystifying 'DevEx', and why it matters"
author: "Jeremy Meiss"
info: |
  ## Demystifying "DevEx", and why it matters

  ## Abstract
  A key factor in shaping the productivity and innovation of software developers is what has come to be called “Developer Experience.” We'll begin with an introduction to DevEx, exploring its definition and significance in the tech world. We'll traverse the history of software development, highlighting how DevEx has evolved with technology. Key components, such as ergonomic tools, efficient workflows, and community support, are dissected to showcase their impact on a developer's day-to-day life. We'll look at successful and problematic DevEx scenarios, offering lessons and strategies for improvement. Then, we'll delve into practical tips for enhancing DevEx, discussing better practices and common pitfalls. Looking forward, we will explore emerging trends and future predictions, hopefully preparing us for the evolving landscape of software development. This talk is an essential journey through the world of DevEx, ideal for developers, team leaders, and tech enthusiasts keen on optimizing their development environments for better outcomes.
conference: "Developer Week 2025"
socialimg: '../images/bluesky-jerdog-white.png'
favicon: 'https://raw.githubusercontent.com/jerdog/jmeiss-me-website/main/assets/images/fav.png'
keywords: devex,developer experience
presenter: true
download: true
exportFilename: devweek2025-demystifying-devex-slides
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

# Demystifying "Developer Experience"...

## and why it matters


<!--

-->

---

# "Bad developer experience?"

## "You know it when you see it..."

<!--
We've all had that experience using a tool or service that was a disaster. It could be the worst deployment process you've ever seen, or the most painful codebase you've ever had to work with, or documentation that's so confusing it makes your head spin. Or maybe a combination of them… Who here knows what I’m talking about?

NordicAPIs gathered some examples a few years ago…
-->

---
layout: image-right
image: /images/slides/new-feature-fail.gif
backgroundSize: contain
class: my-cool-content-on-the-left
---

# Bad DevEx
## Common examples

- Poorly documented features (or bugs)

<!--
- Poorly documented features (or bugs)

We’ve all had those moments where we encounter changes to an application that either introduce new features, or in some cases, new bugs, that aren’t adequately documented or even mentioned as existing - even if the bug won’t be fixed for awhile and there are workarounds.

-->

---
layout: image-right
image: /images/slides/api-fail.png
backgroundSize: contain
class: my-cool-content-on-the-left
---

# Bad DevEx
## Common examples

- Poorly documented features (or bugs)
- Missing OpenAPI spec (or even APIs)

<!--
- Missing OpenAPI spec (or even APIs)

We’ve all worked with those companies that say they have a developer platform, but are missing documentation for their APIs, or even worse, no APIs at all.
-->

---
layout: image-right
image: /images/slides/missing-docs-fail.png
backgroundSize: contain
class: my-cool-content-on-the-left
---

# Bad DevEx
## Common examples

- Poorly documented features (or bugs)
- Missing OpenAPI spec (or event APIs)
- Downloading documentation… as a PDF, or access-gated

<!--
- Downloading documentation… as a PDF, or access-gated

Having to hunt all over for documentation, and it’s not been written, OR, to find it, and realize you have to download it as a PDF, or that it’s gated by a password. For a public tool.
-->

---
layout: image-right
image: /images/slides/missing-examples-fail.png
backgroundSize: contain
class: my-cool-content-on-the-left
---

# Bad DevEx
## Common examples

- Poorly documented features (or bugs)
- Missing OpenAPI spec (or event APIs)
- Downloading documentation… as a PDF, or access-gated
- Missing examples… of _anything_

<!--
- Missing examples… of _anything_

There’s the examples of different departments having different ideas of what has been built, without any examples of how to actually use it or put it together. Accessing a development tool shouldn’t be like putting together an IKEA piece of furniture.
-->

---
layout: image-right
image: /images/slides/ramiro-tweet.png
backgroundSize: contain
class: my-cool-content-on-the-left
---

# Bad DevEx
## Common examples

- Poorly documented features (or bugs)
- Missing OpenAPI spec (or event APIs)
- Downloading documentation… as a PDF, or access-gated
- Missing examples… of _anything_
- “CI as Magic 8-Ball”

<!--
- “CI as Magic 8-Ball”

And then there is Ramiro's story that I call "CI as Magic 8-Ball"

***What about epicly bad websites that would put ebaumsworld to shame?***
-->

---
layout: image
image: /images/slides/yale-art-school.jpg
backgroundSize: contain
---

<!--
And this is updated for Spring 2025.
-->

---
layout: image
image: /images/slides/yale-art-school-spring2025.jpg
backgroundSize: contain
---

<!--
-->

---

# What about a good Developer Experience?

---

```bash
git push heroku main
```

![Heroku deploy button](/images/slides/heroku-deploy-button.png)

<!--
Heroku was long considered the gold standard for developer experience with a simple set of tools and a command-line interface that allowed developers to focus on building applications and delivering them to users. And that was it. Now of course, Heroku is still around (albeit not nearly as developer-centric as they formerly were, but that is changing), but it's not the only game in town. Anyone used Netlify, Vercel, etc.?
-->

---
layout: intro
transition: fade | fade
title: "About Me"
---

<div class="multiCol">
    <div class="col">
        <h2>Jeremy Meiss</h2>
        <p style="font-weight: 900; font-size: 1.25rem;">Director, DevEx & DevRel</p>
        <p style="font-size: 1rem;"><em>OneStream Software</em></p>
        <!-- <p style="font-size: 0.8em;"><a href="https://devex.institute" target="_blank">https://DevEx.Institute</a></p> -->
        <p style="font-size: 1rem;">DevOpsDays Kansas City Organizer</p>
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
layout: section
---

# Developer Productivity != Developer Experience

<!--
Over the past few years, there's been a lot of talk about Developer Productivity. But it's important to understand that Developer Productivity and Developer Experience are not the same thing, even though a lot of companies selling you something would like you to think that they are, or that they're interchangeable as a term. They are not.
-->

---
layout: two-cols-header
---

# Developer Productivity != Developer Experience

::left::

## Developer Productivity

<v-clicks>

- [Focus:]{style="font-weight: 900; background: var(--slidev-theme-accents-red);"} _measured in terms of output, with an emphasis on efficiency and performance._

- [Context:]{style="font-weight: 900; background: var(--slidev-theme-accents-red);"} _metrics like "time to release", "number of pull requests", or "deployment frequency"._

- [Differs from DevEx:]{style="font-weight: 900; background: var(--slidev-theme-accents-red);"} _doesn't capture the full experience of developers._

</v-clicks>

::right::

<!--
## Developer Productivity
[click]Focus: measured in terms of output, with an emphasis on efficiency and performance.
[click]Context: metrics like "time to release", "number of pull requests", or "deployment frequency".
[click]Differs: doesn't capture the full experience of developers.
-->

---
layout: two-cols-header
---

# Developer Productivity != Developer Experience

::left::

## Developer Productivity

- [Focus:]{style="font-weight: 900; background: var(--slidev-theme-accents-red);"} _measured in terms of output, with an emphasis on efficiency and performance._

- [Context:]{style="font-weight: 900; background: var(--slidev-theme-accents-red);"} _metrics like "time to release", "number of pull requests", or "deployment frequency"._

- [Differs from DevEx:]{style="font-weight: 900; background: var(--slidev-theme-accents-red);"} _doesn't capture the full experience of developers._

::right::

## Developer Experience (DevEx)

<v-clicks>

- [Focus:]{style="font-weight: 900; background: var(--slidev-theme-accents-red);"} _holistic view encompassing all aspects of the developer journey (usability, efficiency, satisfaction, etc.)_
- [Unique:]{style="font-weight: 900; background: var(--slidev-theme-accents-red);"} _integrates elements of UX and productivity, but with a broader scope of psychological safety, community, and feedback loops._

</v-clicks>

<!--
## Developer Experience (DevEx)
[click]Focus: holistic view encompassing all aspects of the developer journey (usability, efficiency, satisfaction, etc.)
[click]Unique: integrates elements of UX and productivity, but with a broader scope of psychological safety, community, and feedback loops.
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

<!--
The first is where it talked about these New ways of working where development was globally distributed and integrating self-motivated external developers into software ecosystems and would require a better and more comprehensive understanding of developers' feelings, perceptions, motivations and identification with their tasks in their respective project environments.
-->

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
layout: image
image: "/images/slides/text-to-cloud.jpg"
---


<!--
And we've see an evolution in Developer Experience over the years.

Here's an example of how Developer Experience has evolved a particular set of tools and practices:
-->

---

# Evolution of the IDE

## Early text editors

![USER FRIENDLY by Illiad, vi](/images/slides/httpatomoreillycomsourceoreillyimages2055076.png)
REF: O'Reilly "Learning the vi and Vim Editors"

<!--
I think a great example is the evolution of Integrated Development Environments (IDEs). Prior to the 1990's, you had mostly text-based editors that were used to write code, like Vi, which evidently is supposed to be called "SIX". Who knew? It was created in 1976 and included in the first BSD linux release.
-->

---
layout: image-left
image: "/images/slides/IDE_evolution-1.jpg"
backgroundSize: contain
class: my-cool-content-on-the-right
---

# Evolution of the IDE

## Early text editors

- 1976: Vi

<v-clicks>

- 1985: Emacs

- 1991: Vim

- 1999: nano

</v-clicks>

<!-- [click]Then we had Emacs in 1985, [click]Vim in 1991, my personal favorite, [click]`nano`. And not entirely because I can exit it without having to throw out the computer and buy a new one like I do with Vim. Saving the planet, one less computer thrown away because of Vim at a time. -->

---
layout: image-left
image: "/images/slides/IDE_evolution-3.jpg"
backgroundSize: contain
class: my-cool-content-on-the-right
---

# Evolution of the IDE

## Native IDEs in the 1980s

<v-clicks>

- 1983: Turbo Pascal

- 1986: Apple's Macintosh Programmer's Workshop

</v-clicks>

<!--
A few Native IDEs came out in the mid-80s, [click]with Turbo Pascal in 1983 and [click]Apple's Macintosh Programmer's Workshop in 1986.
-->

---
layout: image-left
image: "/images/slides/IDE_evolution-2.jpg"
backgroundSize: contain
class: my-cool-content-on-the-right
---

# Evolution of the IDE

## First plug-in IDE

### HP Softbench

<!-- One of the first IDEs with a plug-in concept was HP Softbench, released in 1989. HP Softbench was one of the first plug-in IDEs, shipped with its own library, -->

---
layout: image-left
image: "/images/slides/hp-softbench-manuals.jpg"
backgroundSize: contain
class: my-cool-content-on-the-right
---

# Evolution of the IDE

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

# Evolution of the IDE

## First plug-in IDE

### HP Softbench

REF: [HP Journal, June 1990 edition](http://hparchive.com/Journals/HPJ-1990-06.pdf)

<!--
It's a fascinating read, as HP lays out their vision of what software architecture and development should be, including Automated Testing, distributed computing, integrated and interchangeable tools, and more. The link to the PDF is below - I highly recommend reading it
-->

---
layout: image-left
image: "/images/slides/giphy-thumbs-down.gif"
class: my-cool-content-on-the-right
---

# Evolution of the IDE

## Early Reviews

> "...the use of an IDE was not well received by developers since it would fence in their creativity."

REF: _Computerwoche_ ("Computer Week", German counterpart of American magazine _Computer World_), 1995.

<!--
The early reviews of IDEs as a concept weren't great.... In 1995 Computer Week in Germany commented that the use of an IDE was not well received by developers since it would fence in their creativity.
-->

---
layout: image-left
image: "/images/slides/IDE_evolution-4.jpg"
backgroundSize: contain
class: my-cool-content-on-the-right
---

# Evolution of the IDE

## Cross-platform in the 1990s

### 1995: Borland Delphi

<!--
Borland Delphi was released in 1995 and is still around (Embarcadero Delphi v12.2 is now out)
-->

---
layout: image-left
image: "/images/slides/IDE_evolution-5.jpg"
backgroundSize: contain
class: my-cool-content-on-the-right
---

# Evolution of the IDE

## The Web and the 1990s

<v-clicks>

- 1995: SGI WebMagic

- 1995: Microsoft FrontPage

</v-clicks>

<!--
With the launch of the World Wide Web, and then its explosion of growth, the IDEs started becoming more graphical and had a more modern look and feel. Who remembers the first HTML WYSIWYG editor? [click]SGI's WebMagic was released on January 25, 1995 built in less than 90 days. [click]FrontPage was soon to follow in October 1995 after Microsoft acquired it from Vermeer.
-->

---
layout: image-left
image: "/images/slides/IDE_evolution-6.jpg"
backgroundSize: contain
class: my-cool-content-on-the-right
---

# Evolution of the IDE

## Features & Usability

### Late 1990s to 2000s

<v-clicks>

- 1997: Macromedia Dreamweaver
- 1997: Microsoft Visual Studio
- 1999: Microsoft FrontPage 2000
- 2000: NetBeans
- 2001: IntelliJ IDEA
- 2001: Eclipse IDE
- 2002: Microsoft Visual Studio .NET

</v-clicks>

<!--
[click]Macromedia's Dreamweaver came out in 1997 (after Macromedia acquisition of Backstage from iBand in 1996) Dreamweaver completely changed the game in many respects, as Macromedia had a history of their products getting community-sourced tools, plugins, scripts, etc. [click]Microsoft released their first version of Visual Studio in 1997, and then [click]Microsoft FrontPage 2000 saw the first inclusion of plugins and integrations in early 1999 to make web management easier (FrontPage Server Extensions). [click]NetBeans was released in 2000 for Java, with [click]IntelliJ and [click]Eclipse following in 2001 and then along with [click]Microsoft Visual Studio .NET in 2002 with a more modern and feature-rich IDE for .NET development.
We started seeing IDEs which offered enhanced functionality and more sophisticated features like intelligent code completion, refactoring tools, and improved version control integration. We saw a noticeable increase in support for multiple languages and frameworks, making these IDEs more versatile.
-->

---
layout: image-left
image: "/images/slides/IDE_evolution-7.jpg"
backgroundSize: contain
class: my-cool-content-on-the-right
---

# Evolution of the IDE

## Lightweight & Configurable

### 2010s to Now

<v-clicks>

- 2008: Sublime Text

- 2015: Atom

- 2015: Visual Studio Code

</v-clicks>

<!--
### Late 2000s to now
[click]Late 2000s brought about more lightweight IDEs, like Sublime Text and later [click]Atom and [click]Visual Studio Code (VSCode) emerged, focusing on speed, user-friendly interfaces, and extensive plugin ecosystems. They catered to a broader range of developers by being less resource-intensive and more customizable. Even saw integrations with popular Ops tools as well.
-->

---
layout: image-left
image: "/images/slides/IDE_evolution-8.jpg"
backgroundSize: contain
class: my-cool-content-on-the-right
---

# Evolution of the IDE

## Cloud-based Options

### Now

<v-clicks>

- 2009: PHPanywhere (eventually becoming CodeAnywhere)
- 2010: Cloud9 (AWS bought it in 2016)
- 2018: Glitch
- 2019: GitPod
- 2020: GitHub Codespaces
- 2024: Google Project IDX

</v-clicks>

<!--
Then, we have seen the rise of the cloud and the arrival of cloud-based IDEs: The first was [click]PHPanywhere (eventually becoming CodeAnywhere) in 2009, followed by [click]Cloud9 in 2010 (before AWS bought it in 2016), [click]Glitch (2018), [click]GitPod (2019), [click]GitHub Codespaces (2020), and [click]Google’s Project IDX (2024). They've really changed the game by offering fully configured development environments in the cloud, accessible from anywhere, reducing the need for complex local setup. We went from this sentiment about IDEs...
-->

---

# Evolution of the IDE

## A result of DevEx

From this:
> "...the use of an IDE was not well received by developers since it would fence in their creativity."

<!--
We went from this sentiment about IDEs...
-->

---

# Evolution of the IDE

## A result of DevEx

### Things we never knew we needed...

To this:

- Code completion
- Code refactoring
- Syntax highlighting
- Debugging
- VCS integration (no more FTPing files around)
- Multi-language support
- Framework integration
- Pair programming


<!--
To a list of things we didn't even know we needed until we had them. And now, we can't live without them. You likely wouldn't even give an IDE a second look if it didn't have at least most of these features. And this is just the IDE. Anyone have some evolutions in other areas of the developer experience to mention?
-->

---
layout: image
image: /images/slides/devex-evolution.jpg
backgroundSize: contain
---

<!--
I go through all of that to illustrate how the overall Developer Experience with software development has evolved over time, leading to where we sit with IDEs now.
-->

---
layout: section
---

# Key Themes of Developer Experience

<!--
Let's talk about what the key themes are around a good developer experience
-->

---
layout: default
---

# Key Themes of Developer Experience

1. ***Developer proficiency & growth***
- Align tasks with expertise and skill level
- Focus on skill development, mentorship, structured work
- Provide challenging but meaningful tasks

<!--
1. ***Developer proficiency & growth***
Developers are most productive when **tasks align with their expertise and skill level.** Organizations should **focus on skill development, mentorship, and structured work** to reduce cognitive overload. **Providing challenging but meaningful tasks** helps maintain motivation and engagement.
-->

---
layout: default
---

# Key Themes of Developer Experience

1. Developer proficiency & growth
2. ***Work environment & productivity flow***
- Minimize interruptions, unnecessary context-switching, distractions
- A healthy physical and virtual work environment
- Give autonomy over work, tools, decision-making

<!--
2. ***Work environment & productivity flow***
**Minimizing interruptions, unnecessary context switching, and distractions** leads to better productivity. **A healthy work environment (both physical and virtual)** reduces burnout and supports long-term effectiveness. Developers perform best when given **autonomy over their work, tools, and decision-making** processes.
-->

---
layout: default
---

# Key Themes of Developer Experience

1. Developer proficiency & growth
2. Work environment & productivity flow
3. ***Collaboration & communication***
- Effective team collaboration
- Provide clear, accessible, relevant information
- Encourage psychological safety and supportive team culture

<!--
3. ***Collaboration & communication***
**Effective team collaboration** improves efficiency and problem-solving. **Providing developers with clear, accessible, and relevant information** reduces decision fatigue. **Encouraging psychological safety and supportive team culture** enhances engagement and retention.
-->

---
layout: default
---

# Key Themes of Developer Experience

1. Developer proficiency & growth
2. Work environment & productivity flow
3. Collaboration & communication
4. ***Code & tooling quality***
- High-quality, maintainable, well-documented codebases
- Intuitive, reliable, well-integrated tools and APIs
- Automation and developer-friendly tooling investment

<!--
4. ***Code & tooling quality***
Developers thrive when working with **high-quality, maintainable, and well-documented codebases**. **Tools and APIs should be intuitive, reliable, and well-integrated** into development workflows. **Investing in automation and developer-friendly tooling** reduces friction and improves efficiency.
-->

---
layout: default
---

# Key Themes of Developer Experience

1. Developer proficiency & growth
2. Work environment & productivity flow
3. Collaboration & communication
4. Code & tooling quality
5. ***Process & standardization***
- Balance structured process and developer flexibility
- Standardization that supports, not hinders, productivity
- Steadily evolving technical ecosystem with right resources

<!--
5. ***Process & standardization***
Striking a balance between **structured processes and developer flexibility** prevents bureaucratic slowdowns. **Standardization should support, not hinder, productivity**—use automation to enforce best practices. The **technical ecosystem should evolve steadily**, ensuring developers have the right resources without overwhelming them with constant change.
-->

---
layout: section
---

# How does DevEx apply to frontend developers?

<!--
As an example of applying these themes to a specific area, let's use frontend development which has some interesting and unique challenges. The key themes of DevEx have an important role to play in ensuring frontend developers can work efficiently, stay engaged, and build high-quality applications.-->

---
layout: two-cols-header
---

# DevEx theme ==> Frontend devs

## Developer proficiency & growth

::left::

<v-click>

### Why it matters{style="font-weight: 900; background: var(--slidev-theme-accents-red);"}

- Rapidly changing frameworks
- Critical mastery of JavaScript, CSS, accessibility, performance optimization
- Developers need time and resources to stay up-to-date and improve

</v-click>

::right::

<v-click>

### Strategies for enhancement{style="font-weight: 900; background: var(--slidev-theme-accents-red);"}

- Continuous learning & experimentation
- Mentorship & pair programming
- Clear career growth paths

</v-click>

<!--
## Developer proficiency & growth
[click]Why It Matters: Frontend developers need to continuously adapt to evolving frameworks, tools, and best practices to build high-quality, performant user interfaces.
[click]Strategy: Encourage continuous learning, mentorship, and clear career progression to foster professional growth and specialization.
-->

---
layout: two-cols-header
---

# DevEx theme ==> Frontend devs

## Work environment & productivity flow

::left::

<v-click>

### Why it matters{style="font-weight: 900; background: var(--slidev-theme-accents-red);"}

- Frequent iterations the norm
- Focus on creative problem solving
- Bottlenecks, distractions, and interruptions hinder productivity

</v-click>

::right::

<v-click>

### Strategies for enhancement{style="font-weight: 900; background: var(--slidev-theme-accents-red);"}

- Fast, configurable dev environments <logos-vitejs />   <logos-nextjs-icon />   <logos-docker-icon />
- Component libraries, design systems <logos-storybook-icon />   <logos-figma />
- Browser DevTools, performance monitoring <logos-lighthouse />

</v-click>

<!--
## Work environment & productivity flow
[click]Why It Matters: A seamless development workflow minimizes friction, accelerates iteration cycles, and allows developers to focus on solving creative UI challenges rather than fighting slow tools.
[click]Strategy: Provide fast, pre-configured development environments, reusable UI components, and real-time performance monitoring to streamline frontend workflows.
-->

---
layout: two-cols-header
---

# DevEx theme ==> Frontend devs

## Collaboration & communication

::left::

<v-click>

### Why it matters{style="font-weight: 900; background: var(--slidev-theme-accents-red);"}

- Interact heavily with designers, backend engineers, product teams
- Lack of clear communication slows down development
- Responsive behavior, accessibility, animations need structured workflows

</v-click>

::right::

<v-click>

### Strategies for enhancement{style="font-weight: 900; background: var(--slidev-theme-accents-red);"}

- Strong design-dev collaboration <logos-figma />   <logos-zeplin />
- Clear API specs & mocking strategies <logos-openapi-icon />   <logos-postman-icon />   <logos-json-schema-icon />
- Shared docs & communication <logos-confluence />   <logos-docusaurus />   <logos-slack-icon />

</v-click>

<!--
## Collaboration & communication
[click]Why It Matters: Frontend teams work closely with designers, backend engineers, and product teams, making clear communication and alignment critical to avoid inefficiencies and rework.
[click]Strategy: Foster strong design-dev collaboration, establish clear API specs, and document shared knowledge to ensure smooth cross-team workflows.
-->

---
layout: two-cols-header
---

# DevEx theme ==> Frontend devs

## Code & tooling quality

::left::

<v-click>

### Why it matters{style="font-weight: 900; background: var(--slidev-theme-accents-red);"}

- Poor tooling slows down development, increases bugs in production
- Inconsitent code bases lead to hard-to-maintain projects, tech debt
- Focus on accessibility, security, performance ensures high-quality standards

</v-click>

::right::

<v-click>

### Strategies for enhancement{style="font-weight: 900; background: var(--slidev-theme-accents-red);"}

- Standardized tooling & linting <logos-eslint />   <logos-prettier />   <logos-typescript-icon />
- Automated testing & CI/CD <logos-playwright />   <logos-cypress-icon />   <logos-github-actions />   <logos-circleci />
- Performance & accessibility audits <logos-lighthouse />

</v-click>

<!--
## Code & tooling quality
[click]Why It Matters: High-quality tooling and well-structured codebases reduce technical debt, improve maintainability, and enhance the performance, accessibility, and security of web applications.
[click]Strategy: Standardize tooling, enforce automated testing, and conduct regular audits to maintain consistency, reliability, and compliance with best practices.
-->

---
layout: two-cols-header
---

# DevEx theme ==> Frontend devs

## Process & standardization

::left::

<v-click>

### Why it matters{style="font-weight: 900; background: var(--slidev-theme-accents-red);"}

- Inconsistent processes slow down teams, create friction
- Standardized workflows reduce decision fatigue, cognitive load
- Defined processes for code reviews, versioning, onboarding == efficient, predictable dev cycles

</v-click>

::right::

<v-click>

### Strategies for enhancement{style="font-weight: 900; background: var(--slidev-theme-accents-red);"}

- Define best practices for code reviews
- Implement versioning & release management
- Project onboarding & documentation

</v-click>

<!--
## Process & standardization
[click]Why It Matters: Inconsistent development processes create unnecessary friction, slow down teams, and make it difficult to scale projects efficiently.
[click]Strategy: Define structured workflows for code reviews, versioning, and onboarding to ensure predictability, efficiency, and reduced cognitive load for developers.
-->

---
layout: section
---

# Practical Implementation

## Turning DevEx into Reality

<!--
In the remaining time we have, let's go over some practical steps you can take within your teams and organizations today.
-->

---
layout: image-right
image: /images/slides/start-small-win-big.jpg
backgroundSize: contain
class: my-cool-content-on-the-left
---

## Turning DevEx into Reality

1. ***Start Small, Win Big***

- Identify a pain point
- Define success

<v-click>

<h4 style="padding-top: 2rem;">Example: Streamline onboarding</h4>

</v-click>

<!--
Don't try to boil the ocean. Begin with a small, well-defined pilot project to demonstrate value quickly and build momentum. Identify a pain point being experienced (internal or external) that impacts productivity and morale. Define success before you start, so you can demonstrate the value of your work. [click]Let's say you choose to streamline the developer onboarding process. You might track metrics like time to first commit or time to productivity.-->

---
layout: image-right
image: /images/slides/feedback.jpg
backgroundSize: contain
class: my-cool-content-on-the-left
---

## Turning DevEx into Reality

1. Start Small, Win Big
2. ***Focus on feedback***

- Multiple channels
- Act on the feedback

<!--
Gathering regular feedback from developers is essential. Be the Voice of the Developer. They are the experts on their own experience, and their input is invaluable for identifying areas for improvement. Capture feedback from a variety of different channels and perspectives. But you also have to act on it. Let them know they are heard and the feedback is being used.
-->

---
layout: image-right
image: /images/slides/metrics.jpg
backgroundSize: contain
class: my-cool-content-on-the-left
---

## Turning DevEx into Reality

1. Start Small, Win Big
2. Focus on feedback
3. ***Metrics that matter***

- Measure the impact
- Communicate results

<!--
Measuring the impact of your DevEx initiatives is crucial for demonstrating their value and securing continued support. Focus on metrics that align with business goals, which could be: developer satisfaction scores, time to deploy, number of bugs, and employee turnover. Choose the metrics that are most relevant to your organization and your DevEx initiatives. Don't discount those that impact the bottom line either. And then communicate them clearly.
-->

---
layout: statement
---

# DevEx is...

>### "ruthlessly eliminating barriers (and blockers) that keep your practitioners from being successful"


<!--
I'll leave you with this, that DevEx is ruthlessly eliminating barriers (and blockers) that keep your practitioners from being successful.
-->

---
layout: two-cols
---


<div style="padding-top:200px; align-items: center; justify-content: center; margin: 0 auto; display: flex;">

  <h2>Thank you!</h2>

</div>

::right::

<p><img src="/images/bluesky-logo.svg" style="vertical-align: middle; display: inline; margin: 5px; max-height:50px; padding-right:10px">@jerdog.dev</p>
<p><img src="/images/linkedin.png" style="vertical-align: middle; display: inline; margin: 5px; max-height:50px; padding-right:10px">/in/jeremymeiss</p>
<p><img src="/images/devto.png" style="vertical-align: middle; display: inline; margin: 5px; max-height:50px; padding-right:10px">@jerdog</p>
<p><img src="/images/mastodon.png" style="vertical-align: middle; display: inline; margin: 5px; max-height:50px; padding-right:10px">@jerdog@hachyderm.io</p>
<p><img src="/images/www.png" style="vertical-align: middle; display: inline; margin: 5px; max-height:50px; padding-right:10px">jmeiss.me</p>
<p style="text-decoration: line-through;"><img src="/images/twitter.png" style="vertical-align: middle; display: inline; margin: 5px; max-height:50px; padding-right:10px;">@IAmJerdog</p>


<!--

-->

---
layout: end
---


<!--

-->

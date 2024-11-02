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
socialimg: '../images/bluesky-jerdog-white.png'
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
git push heroku main
```

![Heroku deploy button](/images/slides/heroku-deploy-button.png)

<!--
Heroku was long considered the gold standard for developer experience with a simple set of tools and a command-line interface that allowed developers to focus on building applications and delivering them to users. And that was it. Now of course, Heroku is still around (albeit not nearly as developer-centric as they formerly were, but that is changing), but it's not the only game in town. Anyone used Netlify, Vercel, etc.? 
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
layout: section
---

# Distinguishing DevEx from other Concepts



---
layout: two-cols-header
---

# Distinguishing DevEx from other Concepts

::left::

## User Experience (UX)

<v-clicks>

- [Focus:]{style="font-weight: 900; background: var(--slidev-theme-accents-red);"} _prioritizing the end users usability and overall experience; aim to make software intuitive, easy to use, and enjoyable to interact with._
- [Context:]{style="font-weight: 900; background: var(--slidev-theme-accents-red);"} _involves user research, wireframes, testing product to optimize user satisfaction._
- [Differs from DevEx:]{style="font-weight: 900; background: var(--slidev-theme-accents-red);"} _DevEx focuses on making tools, processes, and environments that devs use efficient and pleasant.

</v-clicks>

::right::

<v-click>

## Developer Productivity

</v-click>

<v-clicks>

- [Focus:]{style="font-weight: 900; background: var(--slidev-theme-accents-red);"} _measured in terms of output, with an emphasis on efficiency and performance._
- [Context:]{style="font-weight: 900; background: var(--slidev-theme-accents-red);"} _metrics like "time to release", "number of pull requests", or "deployment frequency"._
- [Differs from DevEx:]{style="font-weight: 900; background: var(--slidev-theme-accents-red);"} _they don't capture the full experience of developers, while DevEx encompasses efficiency, the satisfaction, well-being, and support structure of devs._

</v-clicks>

---

# Distinguishing DevEx from other Concepts

## Developer Experience (DevEx)

- [Focus:]{style="font-weight: 900; background: var(--slidev-theme-accents-red);"} _holistic view encompassing all aspects of the developer journey (usability, efficiency, satisfaction, etc.)_
- [Unique:]{style="font-weight: 900; background: var(--slidev-theme-accents-red);"} _integrates elements of UX and productivity, but with a broader scope of psychological safety, community, and feedback loops._

---
layout: intro
---

<div class="multiCol">
    <div class="col">
        <h2>Jeremy Meiss</h2>
        <p style="font-weight: 900; font-size: 1.25rem;">Co-Founder, DevEx Consultant</p>
        <p style="font-size: 1rem;"><em>DevEx Institute</em></p>
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

<!-- Then we had Emacs in 1985, Vim in 1991, my personal favorite, `nano`. And not entirely because I can exit it without having to throw out the computer and buy a new one like I do with Vim. Saving the planet, one less computer thrown away because of Vim at a time. -->

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
A few Native IDEs came out in the mid-80s, with Turbo Pascal in 1983 and Apple's Macintosh Programmer's Workshop in 1986.
-->

---
layout: image-left
image: "/images/slides/IDE_evolution-2.jpg"
backgroundSize: contain
class: my-cool-content-on-the-right
---

# Evolution of the IDE

## First plug-in IDE

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
Borland Delphi was released in 1995 and is still around (Embarcadero Delphi v12)
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
With the launch of the World Wide Web, and then its explosion of growth, the IDEs started becoming more graphical and had a more modern look and feel. Who remembers the first HTML WYSIWYG editor? SGI's WebMagic was released on January 25, 1995 built in less than 90 days. FrontPage (https://softpanorama.org/Office/Frontpage/history.shtml) was soon to follow in October 1995 after Microsoft acquired it from Vermeer.
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
- 1997: Netscape Composer
- 1997: Microsoft Visual Studio
- 1999: Microsoft FrontPage 2000
- 2000: NetBeans
- 2001: IntelliJ IDEA
- 2001: Eclipse IDE
- 2002: Microsoft Visual Studio .NET

</v-clicks>

<!--
Macromedia's Dreamweaver came out in 1997 (after Macromedia acquisition of Backstage from iBand in 1996) Dreamweaver completely changed the game in many respects, as Macromedia had a history of their products getting community-sourced tools, plugins, scripts, etc. Microsoft FrontPage 2000 saw the first inclusion of plugins and integrations in early 1999 to make web management easier (FrontPage Server Extensions). NetBeans was released in 2000 for Java, with IntelliJ and Eclipse following in 2001 along with Visual Studio which offered enhanced functionality and more sophisticated features like intelligent code completion, refactoring tools, and improved version control integration. We saw a noticeable increase in support for multiple languages and frameworks, making these IDEs more versatile. Microsoft Visual Studio .NET was released in 2002, offering a more modern and feature-rich IDE for .NET development.
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
Late 2000s brought about more lightweight IDEs, like Sublime Text and later Atom and Visual Studio Code (VSCode) emerged, focusing on speed, user-friendly interfaces, and extensive plugin ecosystems. They catered to a broader range of developers by being less resource-intensive and more customizable. Event saw integrations with popular Ops tools as well.
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
Then, we have seen the rise of the cloud and the arrival of cloud-based IDEs: The first was PHPanywhere (eventually becoming CodeAnywhere) in 2009, followed by Cloud9 in 2010 (before AWS bought it in 2016), Glitch (2018), GitPod (2019), GitHub Codespaces (2020), and Google’s Project IDX (2024). They've really changed the game by offering fully configured development environments in the cloud, accessible from anywhere, reducing the need for complex local setup. We went from this sentiment about IDEs...
-->

---

# Evolution of the IDE

## A result of DevEx

### Things we never knew we needed...

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
We went from this sentiment about IDEs...
-->

---
layout: image
image: /images/slides/devex-evolution.jpg
backgroundSize: contain
---

<!--
I go through all of that to illustrate how the overall Developer Experience with software development has evolved over time, leading to where we sit with IDEs now. Things we didn't know we would want back in the 1960s are now commonplace and the expeected norm now in the 2020s.
-->

---
layout: image
image: /images/slides/rise-of-devops.png
backgroundSize: contain
---


<!--
I would say one of the biggest contributing factors to where we are today with DevEx is the rise of DevOps.
DevOps emphasizes collaboration, automation, and continuous integration and delivery, which has led to the development of more integrated and streamlined development environments and tools. As a result we've seen in recent years a heavy emphasis on, and shift twoards, DevEx at all levels of the software development lifecycle and IT operations.
-->

---

# The Rise of DevOps...

## Software Developement before DevOps

<div v-click>

> _“It used to take weeks or even months to deploy a simple change.”_

</div>

<v-clicks>

- Manual, error-prone deployments

- Siloed teams with minimal collaboration

- Lengthy software development cycles

</v-clicks>

<!--
Discuss the inefficiencies of pre-DevOps practices. Explain how the traditional development process suffered from long deployment times, manual handovers, and frequent miscommunications between development and operations teams.
-->

---

## The Emergence of DevOps

<v-clicks>

- Automation

- Collaboration

- Continuous Integration

</v-clicks>

<!--
Explain that DevOps was born out of a need for faster and more reliable software delivery. Highlight how the principles of DevOps foster collaboration and introduce automation as a core part of the software lifecycle.
-->

---

## The Role of Automation in DevOps

<v-clicks>

- Jenkins

- Docker

- Kubernetes

</v-clicks>

<!--
Dive deeper into the significance of automation in DevOps. Discuss how automated build and deployment processes have revolutionized the developer workflow, allowing for rapid iterations and fewer errors.
-->

---

## DevOps paved the way for Modern DevEx

<v-clicks>

- Efficiency gains through reduced friction of deployments

- Shift from just code quality to developer well-being and satisfaction

- Reduced cognitive load

- Encouragement of experiementation and fast feedback loops

</v-clicks>

<!--
Explain that as DevOps improved workflows and reduced deployment pain points, it also opened the door for a more developer-focused approach. Discuss how the efficiency gained from DevOps practices enabled companies to focus on improving the overall experience of developers, not just the software being built.
-->

---

## DevEx is a natural evolution of DevOps


<!--
Key Point: “DevOps laid the groundwork, but DevEx takes it further by prioritizing developer satisfaction and ease of use.” Make the connection clear between DevOps and DevEx. Highlight how DevEx is not a replacement for DevOps but an extension that emphasizes the developer’s needs and experience.
-->

---

# The Rise of DevOps...

## ...and the Birth of Modern DevEx

### Developer Platforms and Internal Tooling

- Developer Portals

- Self-serve infrastructure

- API-Driven Infrastructure


<!--
Callout: “Companies are investing in platforms that abstract complexity.” Talk about the emergence of developer platforms designed to make accessing resources easy and intuitive. Explain how these platforms have become a key part of modern DevEx, enabling developers to deploy, test, and monitor their code efficiently.
-->

---

## The Birth of Modern DevEx

### Cultural Shift towards Collaboration and Experimentation

- Cross-functional teams

- Encouragement of feedbaack and continuous learning

<!--
Main Message: “A culture of collaboration is the foundation of great DevEx.” Discuss the cultural changes inspired by DevOps, such as the focus on collaboration and shared responsibility. Highlight how these cultural shifts have directly influenced the practices that now define modern DevEx.-->

---
layout: section
---

# Core pillars of Developer Experience

<!--

-->

---
layout: two-cols-header
---

# Core pillars of Developer Experience

## Developer Onboarding

::left::

<v-click>

### Effective Strategies{style="font-weight: 900; background: var(--slidev-theme-accents-red);"}

- Comprehensive onboarding kits

- Mentorship programs

</v-click>

::right::

<v-click>

### Measurements{style="font-weight: 900; background: var(--slidev-theme-accents-red);"}

- Time to first commit

- Time to first merge

- "_____"

</v-click>

<!--
Importance of Onboarding: The first few days and weeks can make or break a developer’s perception of an organization’s DevEx.

Effective Strategies:
- Comprehensive Onboarding Kits: Include environment setup guides, example projects, and walkthroughs.
- Mentorship Programs: Pair new hires with experienced developers to accelerate acclimatization.

Measurement: Use metrics like “Time to First Commit” or “Time to First Merge” to gauge onboarding success.
-->

---

# Core pillars of Developer Experience

## Documentation

- Living documentation

- Developer portals

<!--
Impact on Day-to-Day Productivity: Poor documentation is a common source of frustration. Good documentation, on the other hand, empowers developers to be self-sufficient.

Best Practices:
- Living Documentation: Ensure documentation is regularly updated and easy to navigate.
- Developer Portals: Create centralized knowledge hubs for internal and external developers.

Examples of Good Documentation: Companies like Stripe and Twilio are renowned for their clear and example-rich docs.
-->

---

# Core pillars of Developer Experience

## Continuous Feedback

- Regular surveys

- Feedback forums

- Act on feedback

<!--
Value of Continuous Feedback: Implementing effective feedback loops is essential for identifying pain points and iterating on DevEx.

Feedback Mechanisms:
- Regular Surveys: Quarterly satisfaction surveys to measure developer happiness.
- Feedback Forums: Internal communities where developers can voice concerns and suggest improvements.

Acting on Feedback: Showcase examples of companies with “You Said, We Did” initiatives that align priorities based on developer input.
-->

---

# Core pillars of Developer Experience

## CI/CD and Automation

- Automate everything

- Fast feedback loops

<!--
The Backbone of Modern Development: CI/CD pipelines and automation streamline development, reduce manual errors, and speed up delivery.

Key Practices:
- Automate Everything: From code linting to infrastructure testing, automation minimizes friction.
- Fast Feedback Loops: Optimize pipelines to provide immediate feedback on changes.

Pitfalls: Discuss scenarios where overcomplicated pipelines lead to more problems than they solve.
-->

---

# Core pillars of Developer Experience

## Infrastructure Orchestration

- Developer Self-Service

- Simplifying Deployment

<!--
Developer Self-Service: Infrastructure orchestration tools (like Kubernetes and Terraform) should be easy to use and developer-friendly.

Simplifying Deployment: Tools like Pulumi and Serverless Framework enable developers to deploy without deep DevOps expertise.
Challenges: Ensure the tools are well-documented and abstract away unnecessary complexity.
-->

---

# Core pillars of Developer Experience

## Culture and Team Structure

- Cross-functional teams

- Promote psychological safety

<!--
Impact of Culture on DevEx: A supportive, feedback-oriented culture is essential for a thriving developer experience.

Team Structure Matters:
- Cross-Functional Teams: Aligning teams with clear ownership reduces friction and confusion.
- Promoting Psychological Safety: Teams that feel safe to share concerns and experiment contribute to a stronger DevEx.

Example of Successful Structures: Discuss Spotify’s Squad and Guild model as a case study for empowering developers.
-->

---

# Core pillars of Developer Experience

## Developer Well-Being

- Flexible schedules

- Work-life boundaries

<!--
Balancing Productivity and Well-Being: Burnout is a significant threat in high-paced development environments. A good DevEx considers developer mental health.

Strategies for Well-Being:
- Flexible Schedules: Encourage autonomy and flexible hours.
- Work-Life Boundaries: Promote disconnecting from work to maintain a healthy balance.

Creating a Culture of Support: Initiatives like wellness programs, no-meeting days, and social activities can help.
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


<!--

-->

---


<!--

-->

---


<!--

-->


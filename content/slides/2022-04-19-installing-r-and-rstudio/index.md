---
title: "Installing R & Rstudio"
summary: ''
date: '2022-04-19T06:35:15+02:00'
tags: []
categories: []
authors: []
slides:
  theme: black
  highlight_style: dracula
  diagram: yes
  diagram_options:
    theme: base
  reveal_options:
    controls: yes
    progress: yes
    slide_number: c/t
    center: yes
    rtl: no
    mouse_wheel: yes
    transition: fade
    transitionSpeed: default
    background_transition: slide
    touch: yes
    loop: no
    menu_enabled: yes
---

# Installing R & RStudio

Peter Baumgartner via [Thought Splinters](https://notes.peter-baumgartner.net/)

---

## Controls

- Next: `Right Arrow` or `Space`
- Previous: `Left Arrow`
- Jump to slide with menue: <i class="fa fa-bars"></i>
- Start: `Home`
- Finish: `End`
- Overview: `Esc`
- Zoom: `Alt + Click`, Linux: `CTRL + Click`
- Speaker notes: `S`
- Fullscreen: `F`
- Pause presentation: `B` or `.`

---

## PDF Export

- Add "?print-pdf" to the end of the URL
- Open the in-browser print dialog (CTRL/CMD+P)
- Save to PDF
- Detailed guide: [PDF Export Documentation](https://revealjs.com/pdf-export/)

---

## Let's start! 

But note: For the installation process

🔴 you will need root access to your computer! 🔴

---


## Go to www.r-project.org

<img src="images/r-project-org-min.png" style="width: 60%" />

Direct your browser to the homepage of the R-project.

---

## Click on the [CRAN](https://cran.r-project.org/mirrors.html) link

<img src="images/r-project-org-2-min.png" style="width: 60%" />

CRAN stands for Comprehensive R Archive Network

---

## Choose a mirror location

<img src="images/choose-mirror-2-min.png" style="width: 60%" />

- Select the location nearest to you OR …
- Choose [0-Cloud](https://cloud.r-project.org/) which is operated 
by RStudio and will redirect you automatically to the nearest server.


---

## Select your operating system


<img src="images/cran-mirror-2-min.png" style="width: 60%" />


I recommend to download the precompiled version whenever possible.

---

## Some links to other resources

- I am on a Mac, so I will choose [Download R for macOS](https://cloud.r-project.org/bin/macosx/) for these slides.
- For other distributions see the following links for YouTube videos: 
  - [Windows 7](https://www.youtube.com/watch?v=eD07NznguA4), [Windows 10](https://www.youtube.com/watch?v=NZxSA80lF1I), [Windows 11](https://www.youtube.com/watch?v=jQgI8jCNIO4)
  - Linux Ubuntu: [Oct. 2020](https://www.youtube.com/watch?v=WpNd6j1nvEE), [Sep. 2021](https://www.youtube.com/watch?v=hVaiMTqDYSA), [Oct. 2021](https://www.youtube.com/watch?v=eE1zh0YVMeM), 
- Or search for another installation guide.

---

## [R for macOS](https://cloud.r-project.org/bin/macosx/)

<img src="images/r-for-mac-2-min.png" style="width: 60%" />

- Select the installer package for your macOS version and hardware: Intel or M1 Mac.
- For older operating systems: scroll down or click the "old" directory right top.

---

## Mental note: XQuartz

<img src="images/r-for-mac-3-min.png" style="width: 60%" />

- Always re-install XQuartz when upgrading your macOS to a new major version.
- We will therefore return later to this page.

---

## Download the installer program

<img src="images/download-installer-min.png" style="width: 60%" />

- Save the installer on your hard disk.

---

## Start und run the installer

There are three things to watch out.

<img src="images/license-agreement-min.png" style="width: 60%" />

1. You have to agree to the license.



---

##  Choose location

<img src="images/install-location-min.png" style="width: 60%" />

2. Select standard location (applications folder), e.g. click the "Install"-button.

---

## Allow installation

<img src="images/use-password-min.png" style="width: 60%" />

3. Allow the installer to install the software.

---

## Installation completed!

<img src="images/installation-success-min.png" style="width: 60%" />

We can now go ahead and install RStudio.

---

## Go to www.rstudio.com

<img src="images/rstudio-home-min.png" style="width: 60%" />

- Scroll the homepage down.
- Be aware that colors and content of the homepage change regularly.

---

## Look for the button …

<img src="images/rstudio-home-down-min.png" style="width: 60%" />

- … "Download Free Desktop IDE" (or similar).
- IDE stands for Integrated Development Environment.

---

## Rstudio Download Page

<img src="images/rstudio-download-min.png" style="width: 60%" />

- Scroll the page down until you see a row of buttons for free downloads or downloads to pay.

---

## Choose RStudio Desktop Free

<img src="images/rstudio-download-down-min.png" style="width: 60%" />

- Click the button for a free "Download" of the RStudio Desktop Open Source Licence.

---

### Download RStudio --- Finally!

<img src="images/rstudio-download-recommendation-min.png" style="width: 60%" />

- The page analysis your system requirements and recommends you already a version.
- If this version is not the correct one, then choose from the installer section. 

---

## Mac: Download the image

<img src="images/rstudio-download-image-min.png" style="width: 60%" />

- On my Mac it wants to download an image to my hard disk.

---

## Mac: Drag RStudio to the Applications Folder

<img src="images/rstudio-drag-into-applications-min.png" style="width: 60%" />

After extracting the image you can drag the program into the applications folder.

---

## Open RStudio …

<img src="images/rstudio-tested-min.png" style="width: 60%" />

- and write a simple calculation in the console window. I wrote `2 + 2 <enter>`,
- If you got the correct result: VOILÀ - you succeeded!👏👍

---

## Return to [R for macOS](https://cloud.r-project.org/bin/macosx/) page

<img src="images/click-xquartz-min.png" style="width: 60%" />

- Remember our mental note: We need to download XQuartz on a Mac installation.

---
## Download XQuartz

<img src="images/download-xquartz-min.png" style="width: 60%" />

- After downloading XQuartz open the saved image.

---

## Install XQuartz

<img src="images/xquartz-package-min.png" style="width: 60%" />

- Installing the XQuartz package is a standard process, with one exception…
---

## Allow software check

<img src="images/check-software-min.png" style="width: 60%" />

- Allow checking your installation requirements.


---

## After installing XQuartz

<h2 class="r-fit-text"> ✅  You are done! ✅   <h2>

## Close presentation

- Press back button of your browser.
- (not the back button of the slide!).

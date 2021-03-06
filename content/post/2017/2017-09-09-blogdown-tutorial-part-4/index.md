---
title: 'Blogdown tutorial (Part 4)'
author: Peter Baumgartner
date: '2017-09-09'
lastmod: '2021-05-19'
categories:
  - how-to
tags:
  - blogdown
  - netlify
  - github
slug: blogdown-tutorial-part-4
draft: no
summary: In this fourth part of the tutorial I will explain a method how to bring
  your website online. My preferred method is to transfer the files via GitHub to
  Netlify, a service specialized for quickly rolling out static websites.
image:
  placement: 2    
  caption: "[Different phases in the process of publishing blogdown websites. Image by ALison Hill: Up & running with blogdown in 2021](https://www.apreshill.com/blog/2020-12-new-year-new-blogdown/)"
  alt_text: "Pictograms of the different phases in the process of publishing blogdown websites."
  focal_point: "Center"
  preview_only: false
---

## Bring your website online: From blogdown via GitHub to Netlify

{{% callout note %}} Update 2021-05-19: Because of breaking changes in `Hugo` and new features in `blogdown` this post is partly outdated. Starting with [blogdown version 1.0]((https://blog.rstudio.com/2021/01/18/blogdown-v1.0/)) you do not build the website always from scratch.

Complement this sequence of the tutorial with reading [Up & running with blogdown in 2021](https://www.apreshill.com/blog/2020-12-new-year-new-blogdown/) by Allison Hill, co-author of the [blogdown book](https://bookdown.org/yihui/blogdown/). {{% /callout %}}

We start this last part of the tutorial [where we have finished last time](/2017/09/08/blogdown-tutorial-part-3/#inspect-post-locally).

### Ignore public folder

One benefit of using Netlify is that that there is no need to upload your large public folder to get your website. Netlify will compile the source files and build by its own the Hugo site. You should take advantage of this feature by telling RStudio that the `public`-folder does not need version control, committed and uploaded. Select the public folder under the Git tab on the right upper pane and select from the configuration menu `ignore…`. {{< figure src="images/ignore-public-folder.png" title="Ignore public folder" numbered="true" >}}

### Confirm .gitignore

This will bring up a window where you can specify which files are to be ignored. Confirm the inclusion of the public folder with clicking 'Save'. {{< figure src="images/git-ignore-public-folder.png" title="Confirm the exclusion of the public folder." numbered="true" >}} This saved file (`.gitignore`) will be added as modified to the version control. {{< figure src="images/gitignore-modified.png" title=".gitignore file added" numbered="true" >}}

### Clean up

Before we are going to rebuild the complete site, I recommend to take some precaution. To rebuild from a clean slate I restart R (Under the RStudio menu 'Session' or CMD-Shift-F10 on MacOS.) and clean up all unnecessary files ('Clean All' in the 'Build' tab under the 'More' menu in the upper right pane.) {{< figure src="images/clean-all.png" title="Rebuild website from a clean status." numbered="true" >}}

### Build website

Now you can safely (re-)build the website by clicking into 'Build Website'. You get a message of all the activities done, the time necessary for the build and were the output was created. \[Personal comment: Frankly I do not know if the last two steps are really necessary when Netlify is running its own scripts.\] {{< figure src="images/build-website.png" title="Rendering website content." numbered="true" >}}

### Commit changes

The next step is to select all changed files under the Git tab and to choose "Commit", write a commit message and to confirm these changes. {{< figure src="images/commit-changes.png" title="Select (stage) content for next commit." numbered="true" >}} {{< figure src="images/reviewed-changes.png" title="Bring all changes under version control and check if everything went smoothly."numbered="true" >}}

### Push changes

Now you can transfer all your committed changes to GitHub. After clicking on the push button a window opens and you can see if the changed files are transferred successfully. {{< figure src="images/push-changes.png" title="Push the committed files to GitHub."numbered="true" >}}

### Inspect repo

If you don't trust this process, you can direct your browser to your GitHub repository and check if really the last commit "First post" has safely arrived. {{< figure src="images/inspect-repo.png" title="Inspect your repo on GitHub to confirm the procedure."numbered="true" >}}

### Get Netlify account

The last task we are going to solve is the connection the GitHub repository to the Netlifly service. Go to <https://www.netlify.com/> and create a free new account ("Get started for free"). {{< figure src="images/create-account-on-netlify.png" title="Inspect your repo on GitHub to confirm the procedure."numbered="true" >}}

### Let Netlify access your repo

After the registration procedure you get a page where you can choose 'New Site from Git'. {{< figure src="images/netlify-empty.png" title="New Site from Git" numbered="true" >}} There are essential three step to create the new website: (A) Choose GitHub as your Git repository. This will bring up a window where you have to confirm that you will allow Netlify access to your GitHub account. {{< figure src="images/netlify-authorization.png" title="Autorize Netlify" numbered="true" >}} (B) Then you have to specify to which repository Netlify should connect. {{< figure src="images/netlify-choose-repo.png" title="Choose your website repository."numbered="true" >}}

### Deploy settings

In the third and last step (C in my former notation) on Netlify to create your website you have to specify the details (parameters) to let Netlify know which type of website it has to build. In the example in the screenshot I said that Netlify should watch my master branch, build a Hugo website from the public repository with the newest version of Hugo at the time of writing this tutorial (version 0.26). {{< figure src="images/netlify-deploy-settings.png" title="Specify the deploy settings." numbered="true" >}}

### Deploy website

After clicking "Deploy website" you can lean back and watch Netlify busy working on building the website. This may take for this initial step some time but later on Netlify will finish work almost immediately as it only builds the new/changed files incrementally. When the rolling down of the messages stops you should see as last line: "Site is live"! {{< figure src="images/netlify-site-is-live.png" title="Wait — and watch Netlify working until it is finished." numbered="true" >}}

### Preview deploy

Scroll back to the beginning of the log messages. You will see that Netlify has giving you a random URL but you can change this later on to your liking. Click "Preview deploy" to go to the URL of your new website. {{< figure src="images/netlify-preview-deploy.png" title="Inspect your random URL." numbered="true" >}}

### Website is online!

Congratulations! Your website is now online. {{< figure src="images/website-is-online.png" title="Your website is online." numbered="true" >}}

## Final comments

This was a very quick tour where I have covered just the things I believed to be essential. If you are (like me) new to static website generators then the different steps together seem overwhelmingly complex. But with patience and some trial and errors you should succeed --- as I have. There are many other (better) tutorials and How-Tos around. You should definitely read carefully the book [blogdown: Creating websites with R Markdown](https://bookdown.org/yihui/blogdown/) and the reports of different experiences from the new [rbind community](https://support.rbind.io/).

<span class='Z3988' title='url_ver=Z39.88-2004&amp;ctx_ver=Z39.88-2004&amp;rfr_id=info%3Asid%2Fzotero.org%3A2&amp;rft_val_fmt=info%3Aofi%2Ffmt%3Akev%3Amtx%3Adc&amp;rft.type=blogPost&amp;rft.title=Blogdown%20tutorial%20(Part%204)&amp;rft.source=Thought%20splinters&amp;rft.rights=CC%20BY-SA%204.0&amp;rft.description=In%20this%20fourth%20part%20of%20the%20tutorial%20I%20will%20explain%20a%20method%20how%20to%20bring%20your%20website%20online.%20My%20preferred%20method%20is%20to%20transfer%20the%20files%20via%20GitHub%20to%20Netlify,%20a%20service%20specialized%20for%20quickly%20rolling%20out%20static%20websites.&amp;rft.identifier=https%3A%2F%2Fnotes.peter-baumgartner.net%2F2017%2F09%2F09%2Fblogdown-tutorial-part-4&amp;rft.aufirst=Peter&amp;rft.aulast=Baumgartner&amp;rft.au=Peter%20Baumgartner&amp;rft.date=2017-09-09&amp;rft.language=en'></span>

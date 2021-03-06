---
title: How to produce bibliographic metadata for your web page?
author: Peter Baumgartner
date: '2019-06-19'
categories:
  - how-to
tags:
  - zotero
slug: how-to-produce-bibliographic-metadata-for-you-web-page
summary: 'The tutorial explains how to use Zotero to produce and embed bibliographic metadata into your web page. An annotated screenshot illustrates each of the 14 simple steps.'
commentable: true
draft: no
side_toc: no
links:
  - icon_pack: fas
    icon: book
    name: Another post on bibliographic metadata
    url: '/2019/06/19/bibliographic-metadata-for-your-web-page/'
  - icon_pack: fas
    icon: book
    name: Archiving quoted web resources
    url: '/2019/07/22/archiving-quoted-web-resources/'
image:
  placement: 2    
  caption: "Zotero is a free bibliography manager"
  alt_text: "Screenshot der Zotero Start Page"
  focal_point: "Center"
  preview_only: false
---

In an <a href="/2019/06/19/bibliographic-metadata-for-your-web-page">accompanying post</a> I explain why to provide bibliographic metadata for your web entries could be beneficial.

## Requirements

In this tutorial, I will show how to produce and embed bibliographic metadata into your web page. To follow this guide, I assume that:

1.  you have installed the standalone version of [Zotero](https://www.zotero.org/).
2.  you have installed the appropriate [Zotero connector](https://www.zotero.org/download/) (plugin) for your browser.
3.  you have a working knowledge how to use Zotero (There are many (video) instructions on the internet, see for instance the 'official' [Zotero Quick Start Guide](https://www.zotero.org/support/quick_start_guide) or the [introduction by the Idaho State University](https://isu.libguides.com/zotero)).

## Bibliographic metadata in 14 small steps

1.  Start Zotero and your browser. Go to the page where you want to embed the metadata. You see the Zotero icon for web pages in the place where your web browsers shows the symbols for its installed extensions. <img src="images/zotero-coins-01-min.png" alt="Screenshot of the target web page for embedding bibliographic metadata." class="border shadow" width="100%"/> <figcaption>**Figure 01:** Target web page for embedding bibliographic metadata.</figcaption>

2.  Click on the icon and download the rudimentary bibliographic information for the web page. <img src="images/zotero-coins-02-min.png" alt="Screenshot shows the menu to download the rudimentary bibliographic information with Zotero" class="border shadow" width="100%"/> <figcaption>**Figure 02:** Download the rudimentary bibliographic information with Zotero.</figcaption>

3.  Change to Zotero and inspect the new downloaded entry. You will notice that many details are still missing. <img src="images/zotero-coins-03-min.png" alt="Sreenshot of the Zotero bilbiograpy with the new downloaed biobliographic entry." class="border shadow" width="100%"/> <figcaption>**Figure 03:** Zotero bilbiograpy with the new downloaed biobliographic entry. </figcaption>

4.  Change the item type to an appropriate value: in my case "Blog Post". You will see that the Zotero icon changes to reflect the new value. Different item types have different fields. <img src="images/zotero-coins-04-min.png" alt="Annoted screenshot explains missing bibliographic information." class="border shadow" width="100%"/> <figcaption>**Figure 04:** The standard web page entry misses many information in its bilbiographic record.</figcaption>

5.  Add the relevant information as shown on the screenshot. Depending on the chosen item type, there are different fields to fill in. There is a list of item types, fields, and their meanings on a [Zotero help page](https://www.zotero.org/support/kb/item_types_and_fields). <img src="images/zotero-coins-05-min.png" alt="Screenshot shows the information added." class="border shadow" width="100%"/> <figcaption>**Figure 05:** Adding information into the bibliographic record.</figcaption>

6.  When you bibliographic entry is complete you can start the conversion and export procedure. Open the context menu (on MacOS is it a right mouse click). <img src="images/zotero-coins-06-min.png" alt="Screenshot show opening of the context menu of the bibliography entry to start the export" class="border shadow" width="100%"/> <figcaption>**Figure 06:** Opening the context menu of the bibliography entry to start the export.</figcaption>

7.  From the appearing drop down menu choose the "COinS" translator. <img src="images/zotero-coins-06a-min.png" alt="Screenshot shows choosing COinS as export translator." class="border shadow" width="100%"/> <figcaption>**Figure 07:** Choose COinS as export translator.</figcaption>

8.  Save the converted data in a file on your hard disk. The place is not essential as we only need the text inside the file. After we have copied the COinS data into our web site, we will delete our intermediary file. <img src="images/zotero-coins-07-min.png" alt="Screenshot shows preparation of saving the converted information." class="border shadow" width="100%"/> <figcaption>**Figure 08:** Prepare to save the converted information.</figcaption>

9.  File name and file extension are also irrelevant. Just check if your export format is "COinS". <img src="images/zotero-coins-08-min.png" alt="Screenshot shows MacOS Save File dialog window with export mode &apos;COinS&apos;." class="border shadow" width="100%"/> <figcaption>**Figure 09:** MacOS Save File dialog window with export mode "COinS".</figcaption>

10. Open the exported file with your text editor and select the COinS HTML code. You will see the text of your bibliography record [URL encoded](https://www.w3schools.com/tags/ref_urlencode.asp) in the COinS standard format. URL Encoding replaces unsafe ASCII characters with a "%" followed by two hexadecimal digits. But don't worry, it is not necessary to understand the code snippet. <img src="images/zotero-coins-09-min.png" alt="Screenshot shows exported COinS code in a text editor." class="border shadow" width="100%"/> <figcaption>**Figure 10:** Exported COinS code as it is seen after opening the file with a text editor.</figcaption>

11. Copy and paste the code in the source code of your web page. Again, the place does not matter. On a life web page visitor do not see these code but only the result -- the particular Zotero icon. <img src="images/zotero-coins-10-min.png" alt="Screenshot shows how the exported COinS code is inserted into the HTML source code of the web page." class="border shadow" width="100%"/> <figcaption>**Figure 11:** Embed the exported COinS code into the HTML source code of the web page.</figcaption>

12. Now inspect you life web page. You will see that the Zotero icon has changed from "Web Page" to "Block Post". Congratulation you made it! <img src="images/zotero-coins-11-min.png" alt="Screenshot of life inspection of the modified web page." class="border shadow" width="100%"/> <figcaption>**Figure 12:** Inspection the modified web page.</figcaption>

13. We need to check if everything works as intended. Save the new generated bibliographic metadata into your zotero database. <img src="images/zotero-coins-12-min.png" alt="Screenshot shows download of the new generated metadata." class="border shadow" width="100%"/> <figcaption>**Figure 13:** Download of the new generated metadata to test if everything works as intended. </figcaption>

14. Check if all the bibliographic metadata are imported correctly. <img src="images/zotero-coins-13-min.png" alt="Screenshot shows how the modified bibliographic entry is inspected in Zotero." class="border shadow" width="100%"/> <figcaption>**Figure 14:** Inspection of the modified bibliographic record in Zotero</figcaption>

## Wrapping up and additional information

<img src="images/zotero-menu-item-type-min.png" alt="Zotero drop down menu of different types of bibliographic entries." class="floatright"/>

You have learned to create, embed, and download bibliographic metadata from those web pages where you have access to the source code. There are further options in addition to what I have demonstrated in the tutorial:

-   *You are not limited to the item type "Block Post":* You can choose from all the 34 different types of bibliographic entries. But watch out: Every item type has its (slightly) different input form and Zotero icon. You need to know what kind of information each bibliographic record type needs.
-   *You are not limited to one COinS entry:* You can generate and embed as many bibliographic entries you want. If your web page has a list of references, you can offer visitors of your web page to download the bibliographic information for the full bibliography. The Zotero icon changes to a folder if there is more than one bibliographic entry to download.
-   *You do not need to generate a COinS entry by yourself if the bibliographic entry has a DOI:* I do not know how this works, but Zotero recognizes DOI entries. See as an example, my [blog post about data science education](https://notes.peter-baumgartner.net/2019/06/18/data-science-education-with-coursera/).

<span class='Z3988' title='url_ver=Z39.88-2004&amp;ctx_ver=Z39.88-2004&amp;rfr_id=info%3Asid%2Fzotero.org%3A2&amp;rft_val_fmt=info%3Aofi%2Ffmt%3Akev%3Amtx%3Adc&amp;rft.type=blogPost&amp;rft.title=How%20to%20produce%20bibliographic%20metadata%20for%20your%20web%20page?&amp;rft.source=Thought%20splinters&amp;rft.rights=CC%20BY-SA%204.0&amp;rft.description=The%20tutorial%20explains%20how%20to%20use%20Zotero%20to%20produce%20and%20embed%20bibliographic%20metadata%20into%20your%20web%20page.%20An%20annotated%20screenshot%20illustrates%20each%20of%20the%2014%20simple%20steps.&amp;rft.identifier=https%3A%2F%2Fnotes.peter-baumgartner.net%2F2019%2F06%2F19%2Fhow-to-produce-bibliographic-metadata-for-you-web-page&amp;rft.aufirst=Peter&amp;rft.aulast=Baumgartner&amp;rft.au=Peter%20Baumgartner&amp;rft.date=2019-06-19&amp;rft.language=en'></span>

---
title: Bibliographic Metadata for your web page
author: Peter Baumgartner
date: '2019-06-19'
lastmod: ~
categories:
  - app
  - bibliography
  - open-science
tags:
  - zotero
summary: 'With _Web 2.0_, we see a radical change in scholarly communication.
  This transition period poses problems for the researcher as the challenges have
  multiplied. On the one hand, there is a growing need to be present on different
  web channels  (blog, twitter, youtube, and much more). On the other hand, the more
  traditional ways of publications in high ranked peer review channels are still prevalent.
  I present in this post a workaround to fulfill both requirements at a certain level:
  Embed bibliographic metadata in your web pages so that they can be cited and count
  as a web publication.'
slug: bibliographic-metadata-for-your-web-page
bibliography: ["../../../../static/media/references.bib"]
commentable: true
draft: no
side_toc: no
links:
  - icon_pack: fas
    icon: book
    name: Archiving quoted web resources
    url: '/2019/07/22/archiving-quoted-web-resources/'
  - icon_pack: ai
    icon: zotero
    name: Produce metadata for your webpage with Zotero (Tutorial)
    url: '/2019/06/19/how-to-produce-bibliographic-metadata-for-you-web-page/'
image:
  placement: 2    
  caption: "ZoteroBib - a free online service by the team behind Zotero"
  alt_text: "Collection of books and mobile devices on blue background with a white header 'Cite anything'."
  focal_point: "Center"
  preview_only: false
---

With *Web 2.0*, we see a radical change in scholarly communication. On the one hand, there is a growing need for researchers to be present on different web channels (blog, twitter, youtube, and much more). On the other hand, the more traditional ways of publications in high ranked peer review channels are still prevalent. It is difficult for researchers to meet this twofold challenge at the same time: After all the day has only 24 hours!

## Double bind for ECRs

[<img src="images/Logo-Euraxess-min.jpg" alt="EUROAXESS log" class="border shadow"/>](https://euraxess.ec.europa.eu/)

<figcaption>

**Figure 1:** EURAXESS - Researchers in Motion is a unique pan-European initiative delivering information and support services to professional researchers.

</figcaption>

Especially for young researchers (so-called Early Career Researchers, or ECRs[^1] is this situation alarming and even existence-threatening. The find themselves in a double-bind: Should they more invest in traditional ways of career planning, or is it more promising to expand and foster their internet presence? I do not have a clear solution for myself. I think a transition period, the most secure strategy is to follow both paths.

> ECRs have both the most to gain and the most to lose from being at the forefront of changes to scholarly communications \[@eve_open_2014; @st.\_louis_open_2015\].

## COinS and Zotero

[<img src="images/zotero-logo-long.png" alt="Logo Zotero" class="border shadow"/>](https://www.zotero.org/)

<figcaption>

**Figure 2:** Zotero is a free, easy-to-use tool to help you collect, organize, cite, and share research.

</figcaption>

The only way I can think of to meet both challenges is to maximize the efficiency of *all* career moves. One of my aims with this blog on *Open Science Education* is to talk about technology supported new ways for research and publication to fulfill both requirements.

[<img src="images/zotero-logo-round-min.jpeg" alt="Logo Zotoro" class="floatright"/>](https://www.zotero.org/)With the following lines, I will show you how you can help your blog readers or website visitors to cite your posts and pages correctly and in way that they could count as a kind of publication.

My suggestion is

1.  to use the free research tool [Zotero](https://www.zotero.org/)
2.  to produce a specific HTML code (COinS = Context Objects in Spans) and
3.  inject this code into your web page.

[COinS](https://en.wikipedia.org/wiki/COinS) is a [microformat standard to embed bibliographic metadata](https://www.univie.ac.at/elib/index.php?title=COinS_Microfromat_Bibliographic_Metadata_for_Embedding_in_HTML) for Embedding in HTML. COinS include as HTML code all the information necessary to cite a publication correctly. It works for every type of publication (books, papers, web pages).

[<img src="images/zotero-startpage-min.png" alt="Zotero Start Page" class="border shadow"/>](https://www.zotero.org/)

<figcaption>

**Figure 3:** Zotero is designed to store, manage, and cite bibliographic references, such as books and articles. It is available for Mac, Windows, and Linux.

</figcaption>

{{% callout note %}} There are [several possibilities to generate COinS](https://en.wikipedia.org/wiki/COinS#Client_tools), but I will focus on Zotero. I am not going into further details here, but [I have prepared a tutorial](2019/06/19/how-to-produce-bibliographic-metadata-for-you-web-page/) with images from all the necessary steps to produce, embed, and download COinS. {{% /callout %}}

## References

<span class="Z3988" title="url_ver=Z39.88-2004&amp;ctx_ver=Z39.88-2004&amp;rfr_id=info%3Asid%2Fzotero.org%3A2&amp;rft_val_fmt=info%3Aofi%2Ffmt%3Akev%3Amtx%3Adc&amp;rft.type=blogPost&amp;rft.title=Bibliographic%20Metadata%20for%20your%20web%20page&amp;rft.source=Thought%20splinters&amp;rft.rights=CC%20BY-SA%204.0&amp;rft.description=With%20_Web%202.0_,%20we%20see%20a%20radical%20change%20in%20scholarly%20communication.%20This%20transition%20period%20poses%20problems%20for%20the%20researcher%20as%20the%20challenges%20have%20multiplied.%20On%20the%20one%20hand,%20there%20is%20a%20growing%20need%20to%20be%20present%20on%20different%20web%20channels%20%20(blog,%20twitter,%20youtube,%20and%20much%20more).%20On%20the%20other%20hand,%20the%20more%20traditional%20ways%20of%20publications%20in%20high%20ranked%20peer%20review%20channels%20are%20still%20prevalent.%20I%20present%20in%20this%20post%20a%20workaround%20to%20fulfill%20both%20requirements%20at%20a%20certain%20level:%20Embed%20bibliographic%20metadata%20in%20your%20web%20pages%20so%20that%20they%20can%20be%20cited%20and%20count%20as%20a%20web%20publication.&amp;rft.identifier=https%3A%2F%2Fnotes.peter-baumgartner.net%2F2019%2F06%2F19%2Fbibliographic-metadata-for-your-web-page&amp;rft.aufirst=Peter&amp;rft.aulast=Baumgartner&amp;rft.au=Peter%20Baumgartner&amp;rft.date=2019-06-19&amp;rft.language=en"></span>

[^1]: There are different definitions for ECRs around, varying how many years after a Ph.D. are included. The period starts from [4 years](https://blog.jobs.ac.uk/all-things-research/phd-ecr/) and goes to in some institutions to [10 years](https://blog.soton.ac.uk/athenaswan/ecrs/what-is-an-ecr/). A more detailed description of different research profile descriptors has the European Research Commission ([EURAXESS](https://euraxess.ec.europa.eu/europe/career-development/training-researchers/research-profiles-descriptors))

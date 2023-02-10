# FOIL Website: [foil.bme.utexas.edu](https://foil.bme.utexas.edu/)

Source code for the Functional Optical Imaging Laboratory (FOIL) website powered by [Hugo](https://gohugo.io/) and hosted on [GitHub Pages](https://pages.github.com/). The website design uses [Wowchemy](https://wowchemy.com/) with the [Research Group](https://github.com/wowchemy/wowchemy-hugo-themes/tree/main/starters/research-group) theme.

![Mockup](https://user-images.githubusercontent.com/867617/166167908-bb9de21f-10b7-420c-9d8d-e0382cd716df.png)


## Table of Contents

* [Add New Publication](#add-new-publication)
* [Add New Lab Member](#add-new-lab-member)
  * [Move Lab Member to Alumni](#move-lab-member-to-alumni)
* [Add New Research Project](#add-new-research-project)
* [Testing Site Locally with Hugo](#testing-site-locally-with-hugo)
* [Deployment](#deployment)

## Add New Publication

Publications are organized into directories in [`content/publication/`](content/publication/) using a `surname-year` nomenclature based on the first author. In the event an author has multiple publications in the same year, append a single digit counter (e.g. `surname-year-1` and `surname-year-2`) to distinguish the different works.

Details of each publication are described in the `index.md` file contained within the publication's directory. _This is the only file necessary to add a new publication to the website._ The base template is shown below or can be copied from an existing publication.

<details><summary>index.md (Click to View)</summary>

```markdown
---

title: "Title"
authors:
  - Firstname Lastname
  - Andrew Dunn
date: "YYYY-MM-DD"
doi: ""
publication: "*A Journal Name*"

abstract: Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

tags:
  - LSCI

# Associated Projects (optional)
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   Publication will be listed on project page.
projects:
  - laser-speckle-contrast-imaging
  
---
```

</details>

### Tips

* Author names should be entered as `"Firstname Surname"` without middle names or initials. This will help ensure that authors are properly linked together across publications and show up on lab member profile pages. Flags such as equal contribution can be indicated using the `author_notes` parameter ([example](content/publication/luan-2017/index.md?plain=1)).

* The digital object identifier (DOI) parameter is used to link to the publication on the journal website. Additional links, such as bioRxiv preprints, can be defined using the `links` parameter ([example](content/publication/sullender-2022-1/index.md?plain=1)).

* [MathJax](https://www.mathjax.org/) is supported natively in abstracts and titles using `$...$` to enclose the command ([example](content/publication/dunn-2005/index.md?plain=1)).

* Assigning _tags_ allows for similar publications to be automatically linked together. Assigning _projects_ will result in the publication showing up on the respective project pages. See existing publications for the most commonly used options.

* To include a PDF file, simply add it to the publication directory using the same name as the directory (e.g. `surname-year/surname-year.pdf`). To include a BibTeX reference, simply add a `cite.bib` citation file to the publication directory.


## Add New Lab Member

Lab members are organized into directories in [`content/authors/`](content/authors/) using a `firstname-surname` nomenclature without middle names or initials. This helps ensure that publications are correctly linked to lab member profiles. Details of each lab member are described in the `_index.md` file contained within the lab member's directory. _This is the only file necessary to add a new lab member to the website._ The base template is shown below or can be copied from an existing lab member.

<details><summary>_index.md (Click to View)</summary>

```markdown
---

# Join date
date: "YYYY-MM-DD"

# Display name
title: Andrew Dunn

# Role/position
role: Professor

# Organizations/Affiliations
organizations:
- name: Biomedical Engineering
  url: https://www.bme.utexas.edu/

interests: 

education:
  courses:
    - course: Ph.D. in Biomedical Engineering
      institution: University of Texas at Austin
      year: 1997

# Social/Academic Networking
# For available icons, see: https://wowchemy.com/docs/getting-started/page-builder/#icons
#   For an email link, use "fas" icon pack, "envelope" icon, and a link in the
#   form "mailto:your-email@example.com" or "#contact" for contact widget.
social:
- label: Email
  link: "mailto:adunn@utexas.edu"
  icon_pack: fas
  icon: envelope

user_groups:
  - Principal Investigator

---
```

</details>

### Tips

* Any number of affiliations can be specified using the `organizations` parameter ([example](content/authors/andrew-dunn/_index.md?plain=1)). Any number of academic degrees can be listed using the `education` parameter ([example](content/authors/andrew-dunn/_index.md?plain=1)). Any number of external links can be specified using the `social` parameter ([example](content/authors/colin-sullender/_index.md?plain=1)). There are [many icons](https://wowchemy.com/docs/getting-started/page-builder/#icons) available for use.

* The `user_groups` parameter controls which section a lab member appears under on the [People](https://foil.bme.utexas.edu/people) page. The current options include: `Principal Investigator`, `Postdoctoral Researchers`, `Graduate Researchers`, and `Undergraduate Researchers`. New groups can be defined, but for them to be included on the [People](https://foil.bme.utexas.edu/people) page, they must be added to the `content.user_groups` section of [`content/people/people.md`](/content/people/people.md?plain=1).

* To include a profile picture, simply add an image named `avatar.png` or `avatar.jpg` to the lab member's directory.


### Move Lab Member to Alumni

To transition a lab member to alumnus status, simply swap the `user_groups` parameter to `Alumni`. The `date` should be changed to the date of departure and the `role` updated to specify the years of involvement (e.g. `Ph.D. Student (2005 - 2010)`). If a lab member had multiple roles during their tenure, use the most recent ([example](content/authors/lisa-richards/_index.md?plain=1)).


## Add New Research Project

Research projects are organized into directories in [`content/project/`](content/project/). Details of each project are described in the `index.md` file contained within the project's directory. _This is the only file necessary to add a new project to the website._ The base template is shown below or can be copied from an existing publication.

<details><summary>index.md (Click to View)</summary>

```markdown
---

title: 
summary: 

tags:
- LSCI

weight: 

image:  
  caption: 
  
  # Placement options: 1 = Full column width, 2 = Out-set, 3 = Screen-width
  placement: 1
    
  # Focal point options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point: Center

  # Set `preview_only` to `true` to just use the image for thumbnails
  preview_only: false

---

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

```

</details>

### Tips

* The `weight` parameter controls the order of projects on the home page.

* The `tags` parameters are used to filter projects for display on the home page. The currently enabled tags are `LSCI` and `Multiphoton Microscopy` (see `content.filter_button` section of [`content/home/projects.md`](content/home/projects.md?plain=1)).

* To add a featured image, simply add an image named `featured.png` or `featured.jpg` to the project's directory. Specify a caption using the `image.caption` parameter. This image will be used for previews and in the project header.

* The text of the project page is defined after the frontmatter (i.e. after the closing `---`). MathJax is supported natively using `$...$` to enclose the command ([example](content/project/oxygen-imaging/index.md?plain=1)). Media files should be placed in the project directory and shown using the `figure` and `video` shortcodes ([example](content/project/clinical-speckle-imaging/index.md?plain=1)).

* Publications that specify a project will be automatically listed on the project page.


## Testing Site Locally with Hugo

_Useful when making significant changes or you want to see edits without immediately publishing_

1. Install Hugo - https://gohugo.io/getting-started/installing
2. Clone website repository and enter directory

   ```bash
   git clone https://github.com/UTFOIL/foil.bme.utexas.edu.git
   cd foil.bme.utexas.edu
   ```

3. Serve site locally: `hugo server -D`
   * Access in web browser at http://localhost:1313/
   * Should automatically update as you edit website files
  

## Deployment

GitHub Actions are used to [automatically build and deploy](.github/workflows/GitHubPages.yml) the website when a push is made to the `main` branch. The compiled website is pushed to the [`gh-pages`](https://github.com/UTFOIL/foil.bme.utexas.edu/tree/gh-pages) branch for deployment via GitHub Pages. Pull requests will result in the website being built _without_ deployment.

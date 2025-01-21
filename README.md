# csz.academy

 [![License: AGPL v3](https://img.shields.io/badge/License-AGPL%20v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0.html)
 [![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)


This is the repository for [csz.academy](https://csz.academy).

## Licensing

Two licenses apply:

 - [AGPL-3.0 or later](./LICENSE.AGPL-3.0-or-later) applies to
   - Code used to generate the webpage
   - Code which is part of the content if no other license is specified within 
	 the same post
 - [CC-BY-NC-4.0](./LICENSE.CC-BY-NC-4.0) applies to any non-code content
   if not specified otherwise.
Official CSZ Blog.

## How to create your author profile

Create a file under the member directory [_members](https://github.com/csz-academy/csz.academy/tree/main/_members) with your acronym as filename. Then add a frontmatter with your personal information.

```md
---
type: member
acronym: <<acronym>>
display_name: <<displaynam>>
roles: ["author"] <-- Your Roles in this project, can also be "architect" or similar
github: <<github username>>
web: <<Your HomePage>>
---

<<Your Profile Page Content>>
```

## Directory Structure

### Posts
Every post is a single unit which contains all markup- and asset files.
At a minimum you create the following structure
```
_posts/
└── <<Year>>/
	└── <<Month>>/
		└── <<Day>>/
			└── <<post-title>>/
				└── <<Year>>-<<Month>>-<<Day>>-<<post-title>>.MARKUP
```

#### Using Assets

Drop the assets next to your post:
```
<<post-title>>/
├── archive.zip
├── image.png
└── <<Year>>-<<Month>>-<<Day>>-<<post-title>>.MARKUP
```
And you can link them in your post like this:
~~~
![My Image](image.png)
[Download Archive here](archive.zip)
~~~
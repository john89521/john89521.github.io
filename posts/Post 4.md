---
title: Node with text
layout: home
---  

classDiagram
    note "From Duck till Zebra"
    Animal <|-- Duck
    note for Duck "can fly\ncan swim\ncan dive\ncan help in debugging"
    Animal <|-- Fish
    Animal <|-- Zebra
    Animal : +int age
    Animal : +String gender
    Animal: +isMammal()
    Animal: +mate()
    class Duck{
        +String beakColor
        +swim()
        +quack()
    }
    class Fish{
        -int sizeInFeet
        -canEat()
    }
    class Zebra{
        +bool is_wild
        +run()
    }


# How to deploy

```mermaid 
Flowchart TD
	A[Deploy to production] --> B{Is it Friday?};
	B -- Yes --> C[Do not deploy!];
	B -- No --> D[Run deploy.sh to deploy!];
	C ----> E[Enjoy your weekend!];
	D ----> E[Enjoy your weekend!];
```

[GitHub blog](https://github.blog/2022-02-14-include-diagrams-markdown-files-mermaid/)  
**NOTE:** The link below is written just like in HTML  
<a href="https://mermaid.js.org/" target="_blank">Mermaid website</a>





----

[^1]: [It can take up to 10 minutes for changes to your site to publish after you push the changes to GitHub](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/creating-a-github-pages-site-with-jekyll#creating-your-site).

[Just the Docs]: https://just-the-docs.github.io/just-the-docs/
[GitHub Pages]: https://docs.github.com/en/pages
[README]: https://github.com/just-the-docs/just-the-docs-template/blob/main/README.md
[Jekyll]: https://jekyllrb.com
[GitHub Pages / Actions workflow]: https://github.blog/changelog/2022-07-27-github-pages-custom-github-actions-workflows-beta/
[use this template]: https://github.com/just-the-docs/just-the-docs-template/generate

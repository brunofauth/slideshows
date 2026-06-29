THIS REPO WAS INSPIRED IN THE IDEAS PUBLISHED IN
[THIS GIST](https://gist.github.com/amdevine/1f5fc940983e22524ecd345904ad6459)

[See this in GitHub Pages](https://brunofauth.github.io/slideshows)

# Docs for me in the future



## Hosting another pandoc-markdown based revealjs slideshow

**These infos assume you've already made your slideshow using
[slide-gen](https://github.com/brunofauth/Slide-gen.git)**

1. Create a new directory under slideshows/

2. Put your compiled revealjs slideshow under said directory
    - When compiling with pandoc, use --standalone, but do not use
      --embed-resources (we are going to get them from this repo's revealjs
      submodule

3. Put the img/ dir you're probably gonna have inside the dir you made earlier

4. run `scripts/prepare-slideshow-html slideshows/<dir-you-created>/index.html`,
   to point `<script>` and `<link>` tags to the reveal.js/ submodule, and,
   hopefully, strip undesired comments

5. Take a peek at `slideshows/<dir-you-created>/index.html` to see if any
   secrets have leaked

6. run `scripts/mkindex`

7. add, commit and push

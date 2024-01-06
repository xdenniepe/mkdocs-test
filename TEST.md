# mkdocs-test

## REFERENCE:
>   https://squidfunk.github.io/mkdocs-material/creating-your-site/

#
1. `docker pull squidfunk/mkdocs-material`
2. `docker run --rm -it -v ${PWD}:/docs squidfunk/mkdocs-material new .`
   -    create a new documentation
3. Add this to mkdocs.yaml
   ```
   theme:
        name: material
   ```
4. To run:
   ```
    docker run --rm -it -p 8000:8000 -v ${PWD}:/docs squidfunk/mkdocs-material
   ```
5. To Build: 
    >   When you're finished editing, you can build a static site from your Markdown files
   ```
    docker run --rm -it -v ${PWD}:/docs squidfunk/mkdocs-material build
   ```
6. Publishing Site:
   -    https://squidfunk.github.io/mkdocs-material/publishing-your-site/
7. Customization:
    -   https://squidfunk.github.io/mkdocs-material/customization/
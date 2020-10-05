# webpage

## Usage

### modifying a page


### adding a page

mkdocs needs a `.md` file in `docs/` and the correct "link" in `mkdocs.yml`

example:
* e.g. i want to add `foo.md` to the "bar" kategory on the webpage
1) create the md file   
   * `touch docs/bar/foo.md` 
   * edit `foo.md` using markdown syntax
2) "link" the `foo.md`
   * `nano mkdocs.yml` 
   * go to `# Navigation`
      * this represents the "kategories" written as plain text
      * you should understand this based on the structure ;) buut:
   * add this:

```yml
- whateveryouwant: 
        - whateveryouwant2: bar/foo.md

```


## Detailed style tutorial [here](https://squidfunk.github.io/mkdocs-material/)




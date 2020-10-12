webpage
===

## Modifying a page

* simply go to the coresponding `.md` file edit it and commit
* done

## Adding a page or changing structure

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

## Change webpage appearance and style

* Detailed style tutorial can be found [here](https://squidfunk.github.io/mkdocs-material/)
* a docker will render the local webpage so you can check what is happening
* to do a "dry run and live test" run the following commands:

```bash
git clone https://github.com/CaSe-group/case-group.github.io.git
# or if repo exists
git pull

# within the directory of the git do
docker run --rm -it -p 8000:8000 -v ${PWD}:/docs squidfunk/mkdocs-material
```

* open the local webpage in your browser via `http://0.0.0.0:8000/`
   * or click [this link](http://0.0.0.0:8000/)
* now you can check the changes



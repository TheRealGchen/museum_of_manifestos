# Museum of Manifestos

This is a static website which houses the content for the `museumofmanifestos.org` website. 

## Style

The website is meant to be minnimum, basically a static HTTPS site where the main content is either raw text itself or pdf's. It should be optimized for viewing on browsers, and have an optional dark mode. The style is reminiscent of 90's era websites

## Running

The website is meant to be ran on a hosted site. To run locally, simply navigate to the base of the repo and spin up a python http server

```bash
python -m http.server 8000
```

That will create a server on port 8000 to look at

## Tests

This repo should use [lychee](https://github.com/lycheeverse/lychee) to check for broken links. To do so add the following into `.git/hooks/pre-push`

```bash
echo "Checking for broken links"
lychee .
```

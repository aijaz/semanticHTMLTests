# semanticHTMLTests

I'm trying to make the website for my soon-to-start service be Reader-mode friendly. I hear that Semantic HTML (HTML5) is the way to go. It appears that neither Apple
nor Google document how their reader-friendly mode works. They probably don't want adverrtisers to abuse it. 

The page I most importantly wanted to render correctly was the "results" page. You can see a live view of it at https://cani.contact/aijaz (Please keep in mind that
website isn't live yet!)

I've put this repo up for people who are academically interested in what finally got it to work. 

Basically, having a structure that looked like this:

```
main
  article
    section
  article
    section
    section
    section
    section
  article
    section
    section
```

didn't work. 

What worked is 
```
article
  section class=result
  section class=head
    section
    section
    section
    section
  section class=head
    section
    section
```

Two resources that helped me get here: 

- https://dev.to/kenbellows/stop-using-so-many-divs-an-intro-to-semantic-html-3i9i
- https://www.client9.com/designing-html-for-safari-reader-mode/ (Thanks to Aaron Brager @getaaron )



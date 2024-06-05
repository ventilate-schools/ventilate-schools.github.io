---
layout: page
title: Tools For Working on Entries
permalink: /tools-for-working-on-entries/
---

# Tools for working on entries.

## Leaning a little about "Markdown"

When writing text the page pertinent to a single school, we're writing in a little language called Markdown.

**Here is how you you make links to another page online:**

```
[This link links to Google](https://google.com)
```

That looks like this [This link links to Google](https://google.com) when the site has been regenerated after a commit

All hyperlinks start with https:// Some older hyperlinks start with http:// (no s) but that's fewer and fewer over 
time.

## Google search to find answers

Searching for a school name to fill in the blanks is just fine. Try to worry about the authenticity of the site you 
have found. Know too that Wikipedia can be inaccurate for periods of time. This was a real moment in Wikipedia's
history: [many years of fake Scots language articles added without detection](https://en.wikipedia.org/wiki/Scots_Wikipedia#:~:text=These%20articles%20have%20been%20described%20as%20%22English%20written%20in%20a%20Scottish%20accent%2C%22%20with%20gibberish%20and%20nonsensical%20words%20and%20spellings%20not%20present%20in%20any%20Scots%20dialect).

## Research

### Wikidata

There is a huge structured database online called [WikiData](wikidata.org). You find a school there, see lots of data for it, navigate 
to related nodes. For school systems like Boston in the USA, it is much more complete than for (say) Welsh schools.  It has 
its own query language, too, if you have some programming skills. https://w.wiki/9yVC is a query that shows the schools 
in Boston, and retrieves the wikipedia page URL and the School's own website. Well, it does if they are known in Wikidata
else that's blank. For the Welsh school data in WikiData there's no useful "Schools in Wales" node to use as the basis 
for a query. *Not yet*, that is, as anyone can furnish those missing facts. Wikipedia links for welsh schools there should
have links to en.wikipedia.org and cy.wikipedia.org when appropriate.  

### AIs and wiki-data

Microsoft's CoPilot AI has some understanding of
data that's held in Wikidata even if it cannot yet run it's own queries.  You could take the query string for Boston 
above and ask CoPilot to give you one which was "like this query but for Wales instead of Boston" (or your LEA). Not
as of May 2024 because of missing data, but one day there will be a query you can run.

### AIs in general

It is a bit hit ans miss at the moment if you wanted to get a listo of schools in and area, and also get secondary 
information for them like website URL.  Try Perplexity.AI, but note that the alternate AIs leap-frog each other from
one week to another.

### Google.com - Searching within a site

That best-ventilation school in Texas has a site: Abrome.com. Say it was too big to click around to navigate. You can 
ask Google to find a single page you might be looking for. Try this in Google's search bar: "ventilation site:https://www.abrome.com". 
You find a few links, mostly blog entries, but the first link is a policy page and that is exactly what we want.

### Search generally

Searching for a school name to fill in the blanks is just fine. Try to worry about the authenticity of the site you 
have found. Know too that even Wikipedia can be inaccurate for periods of time. This was a real moment in Wikipedia's
history: [many years of fake Scots language articles added without detection](https://en.wikipedia.org/wiki/Scots_Wikipedia#:~:text=These%20articles%20have%20been%20described%20as%20%22English%20written%20in%20a%20Scottish%20accent%2C%22%20with%20gibberish%20and%20nonsensical%20words%20and%20spellings%20not%20present%20in%20any%20Scots%20dialect).

# Initial population of area data

An area is a whole small country, a state or province. Maybe even a city if it is large. Initial population will lead to a lot of TODOs markers for people to replace with facts after population.

For a state, province, city, we'd already made a simple list of school districts (not always called districts). Wikipedia sometimes has that. If it is tabular online, you can paste it into Excel or GoogleSheets then pick out the first column just to get the district names.

This is what we're handing to Perplexity.AI (pro mode):

``` 
For AREANAME school districts ONE, TWO, THREE, FOUR	, make a python dict of all schools (no placeholders) like so: ```schools = {
    "District Name": [
    {
        "school_name": "School Name Here",
        "address": "School address here with commas",
        "phone": "school phone number here"
        "website": "URL here"
        "student_count": 1234 
    },
    {  ...
    }
], ...
}```. If anything can't be found, specify "TODO". Give me the answer in a codefence
Sources
```

That's up to 30 districts at a time, but it sometimes stops short of giving you all that you sought. Some copy/paste and changing the prompt to remove previously answered districts is required. That goes into `make_markdown.py` in order to generate the markdown pages per school.

## Coder setup of a new area

``` 
## Say Zzz is the name of the area you're wanting to create, and it doesn't make sense to be part of a larger area.
 
mkdir Zzz
git clone git@github.com:ventilate-schools/MN.git # Minnesota
cp MN/_config.yml Zzz/ 
cp MN/Gemfile Zzz/ 
cp MN/Gemfile.lock Zzz/ 
cp MN/README.md Zzz/ 
cp MN/make* Zzz/ 
cp MN/404.html Zzz/ 
cp MN/TODO.md Zzz/
cd Zzz
git init
# A git commit here if you're likely to make a mess and want to rollback to undo your mess. 
```

`make_markdown.py` is the source you want to edit. It'll have `Minnesota` and `MN` refs you'll need to change. The big list-dict at the top is what you'll need to change for your new Perplexity.AI results.

Whenever you've run `make_markdown.py` you'll also need to run `make_grade_subtotals_and_totals.py` too.

Check this in. Turn on Github pages. Change GitHub actions settings to reduce 90 days of log storage to 1 (to be kind to Github). 

When you're ready transfer the GitHub repo ownership to `ventilate-schools` and it should be part of the main site (that's automatic). Keep your admin/committer rights, of course.
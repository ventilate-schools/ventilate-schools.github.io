---
layout: page
title: More areas - how to?
---

Other countries may be listed here later. Or states/provinces, or even cities if the list of schools would be too large otherwise. Each of these would need (say) ten people willing to oversee the curation of all the pages for that area. It only takes one person to make the list of all schools for that area, but momentum needs other people to step in and take ownership of the quality of the updates per school.

Some of those people volunteering should be individuals with significant GitHub skills - maybe software developers who're COVID-is-airborne savvy and have kids themselves. Or a school's IT teacher who does not want to get reinfected with COVID again. 

People getting GitHub accounts to do this work may be happy to pick a pseudo-name that doesn't identify them. With that, each subgroup should work out how to trust the contributors and how to quickly vet people for trustworthiness. You don't want to admit people that'll edit pages down to "it is just the flu, losers".

# GitHub savvy coder/developers...

1. Git clone <https://github.com/ventilate-schools/AB>. Do not fork it on GitHub, you won't be able to donate it back (step 15)
2. delete the .git/ directory
3. Delete all the directies that contain Alberta schools. They all start with a capital letter: `find . -maxdepth 1 -type d -name '[A-Z]*' -exec rm -rf {} +`
4. Edit `make_markdown.py` to change `AB` to the name of the repo you're thinking of, like `Los_Angeles`. Also `Alberta` to `Los Angeles`. Be sure sure to delete all inside `schools = { }` first.
5. Same for `_config.yml`
6. Go off to AI to get a list of school districts inside the state/province/city you're dealing with
7. Get AI to turn that into `schools= { "district_name": [ {"school_name": "School Name"] }`
8. Pretty-print that same code block in your IDE
9. Taking one set of schools at a time (AI can't do too much in one go), ask AI to fill in address, phone, website, student_count but not to fake any data, instead leaving "TODO" placeholders. Lots of trial and error needed.
10. Run `python3 make_python.py` and examine the result.
11. Delete product of #10 and refine python script as applicable
12. Git init, git add . (as you'd expect). Make a `Los_Angeles` (or whatever) repo on GitHub, do the `git remote add` line is suggests (and main branch) 
12. Commit and push
13. Go back into GitHub settings for that repo and turn on GitHub-Pages
14. Go check the site online soon after
15. File an issue in <https://github.com/ventilate-schools/ventilate-schools.github.io/issues> suggesting a transfer of the ownership to the 'ventilate-schools' org. Engage in the resulting convo. If completed the 'site' automatically and fairly instantly goes into <https://ventilate-schools.its-airborne.org/Los_Angeles> (or whatever). 
16. Continue providing some form of leadership for `Los_Angeles` (or whatever)

You can also engage @Its_Airborne on Twitter/X.com to discuss things. 

**See also:**

* Our [site technologies](./site-technologies/)
* Our [tools for working on entries](./tools-for-working-on-entries/)
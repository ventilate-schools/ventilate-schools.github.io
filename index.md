---
layout: page
title: Schools Ventilation Project
---

# Rationale as a Haiku

<div>
In halls of learning,<br>
Air flows with wisdom and care,<br>  
Safe breaths everywhere.
</div>

# Contribute

So, this is a wiki - like Wikipedia, but for schools and their air-quality. You can contribute to this wiki by editing the pages here. Look for "edit this page" links at the bottom of each page. and ready the [contributing and rules](contributing-and-rules.md) guide.

# NEWS

* Jun 11, 2024: [Corsi-Rosenthal Foundation US: Upgrade your air with a DIY classroom project.](https://www.cleanairk12.com/)

# Kids and teachers being sick all the time is not normal

COVID-19 has weakened people's immune systems to many diseases. Those could be repeat infection of Covid-19, or Flu, RSV, Staph, Strep, Measles, and others.

We have to lower transmission in schools as kids bring it home to parents, too. We **know exactly how to do this** _without_ putting everyone in masks, making people attend school remotely, or implementing any form of lockdown again.

## COVID is Airborne (a fact suppressed at the start)

See [COVID Is Airborne](covid_is_airborne.md)

# Ventilation work for schools allowing healthy full attendance

See [Ventilation Work Needed ](ventilation_work_needed.md)

# Schools ventilation action plan

See our [Action Plan](action_plan.md)

# Mapping the world's schools

* UK: **[Wales](Wales/)**, [**Isle of Man**](https://ventilate-schools.its-airborne.org/IoM/)
* **[USA](USA/)** - just a few states for now, some partial at that
* **[Canada](Canada/)** - just a couple of provinces for now

You're invited to help edit the data within. Sake a look at one of the Welsh schools and see what is marked as TODO. We have some advice on [contributing and rules](./contributing-and-rules/), some [tools for working on per school entries](./tools-for-working-on-entries/), and a [discussion of the technologies we use for this site](./site-technologies/)

You're also invited to help create a list of schools for your country, state, province, region or large city - contact @Its_Airborne on Twitter/X.com

# Adding Other countries?

Other countries may be listed here later. Or states/provinces, or even cities if the list of schools would be too large otherwise. Each of these would need (say) ten people willing to oversee the setup and curation of each school's page. Some of those people should be individuals with significant GitHub skills - maybe software developers who're COVID-is-airborne savvy and have kids themselves. Or a school's IT teacher who doesn't want to get reinfected with COVID again.

If Welsh schools get some traction on this site, we will be open to other countries. For now, we just want every Welsh school graded, then some of them moving in the right direction, before launching a campaign for more areas of the world.

# Grading of schools

Grades of 0 to 5 ("very poor" to "excellent") should be established by 2025.

See [Grading schools](grading.md) for a breakdown of what each grade means.

# DIY air filters

## Pics

<div>
   <!-- thanks to https://rushabhshahprograms.github.io/ImageSlider-Frontend for the slider -->
   <style>
.gallery{
    width: 900px;
    display: flex;
    overflow-x: scroll;
}
.gallery div{
    width: 100%;
    display: grid;
    grid-template-columns: auto auto auto;
    grid-gap: 20px;
    padding: 10px;
    flex: none;
}
.gallery div img{
    width: 100%;
    filter: grayscale(100%);
    transition: transform 0.5s;
}
.gallery::-webkit-scrollbar{
    display: none;
}
.gallery-wrap{
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 10% auto;
}
#backBtn, #nextBtn{
    width: 50px;
    cursor: pointer;
    margin: 40px;
}
.gallery div img:hover{
    filter: grayscale(0);
    cursor: pointer;
    transform: scale(1,1);
}
   </style>
    <div class="gallery-wrap">
        <img src="https://rushabhshahprograms.github.io/ImageSlider-Frontend/images/back.png" id="backBtn">
        <div class="gallery">
            <div>
                <span><img src="https://www.texairfilters.com/wp-content/uploads/PC-Fan-CR-Box.jpeg"></span>
                <span><img src="https://pbs.twimg.com/media/FxTzGa8XwAYXosr?format=jpg&name=large"></span>
                <span><img src="https://pbs.twimg.com/media/GB4pWZAXcAA5qVt?format=jpg&name=4096x4096"></span>
            </div>
            <div>
                <span><img src="https://pbs.twimg.com/media/GB2GUucXUAAWS93.jpg"></span>
                <span><img src="https://preview.redd.it/rwh3ct9gqm261.jpg?width=1080&crop=smart&auto=webp&s=be3e1187e14f721cde3bda7b6e39966e588b5428"></span>
                <span><img src="https://pbs.twimg.com/media/GNcwUVXW4AAPp0-?format=jpg&name=large"></span>
            </div>
        </div>
        <img src="https://rushabhshahprograms.github.io/ImageSlider-Frontend/images/next.png" id="nextBtn">
     </div>
    <script>
        let scrollContainer = document.querySelector(".gallery");
        let backBtn = document.getElementById("backBtn");
        let nextBtn = document.getElementById("nextBtn");
        scrollContainer.addEventListener("wheel",(evt)=>{
            evt.preventDefault();
            scrollContainer.scrollLeft += evt.deltaY;
            scrollContainer.style.scrollBehavior = "auto";
        });
        nextBtn.addEventListener("click",()=>{
            scrollContainer.style.scrollBehavior = "smooth";
            scrollContainer.scrollLeft += 900;
        });
        backBtn.addEventListener("click",()=>{
            scrollContainer.style.scrollBehavior = "smooth";
            scrollContainer.scrollLeft -= 900;
        });
    </script>
</div>

Note: Ionization of the air is not recommended as it creates ozone, which is harmful to people. Upper room ultraviolet technology may play a part in virus inactivation as the technology reaches mass production.

## Resources

* [Try this DIY indoor air purifier to get cleaner air](https://www.youtube.com/watch?v=FJFdLbpNK4Y) - 2.5-minute video from Washington Post
* [5th Graders Make DIY Air Purifiers for Entire School](https://www.youtube.com/watch?v=qZzzEKElIFo) - 3-minute video from Jeffco Public Schools (Colorado)
* [The Homemade Air Purifier That’s Been Saving Lives During the COVID-19 Pandemic](https://www.smithsonianmag.com/innovation/homemade-air-purifier-thats-been-saving-lives-during-covid-19-pandemic-180979681/) - Smithsonian Magazine
* [Do-it-yourself portable air cleaners](https://schools.forhealth.org/diy-air-cleaners/) - Schools For Health site
* [This DIY box helps clear indoor air of the coronavirus. Why aren’t more people using them?](https://www.latimes.com/california/story/2022-07-20/diy-push-to-rid-indoor-air-of-covid) - L.A. Times
* [Air filter workshops protect people from dangers of wildfire smoke](https://www.sfu.ca/sfunews/stories/2024/05/sfu-air-filter-workshops-protect-people-from-dangers-of-wildfire.html) - Simon Fraser University (video clip says wildfire smoke but these also scrub covids from the air)

# Global school ventilation improvement efforts so far and resources

* Boston, USA: [CO2 monitors in 4322 classrooms](https://bostonschoolsiaq.terrabase.com/)
* Berkeley, California: [CO2 monitors in 687 classrooms](https://berkeleyusdpublic.iaqdashboard.ca/public-portal.html)
* Lübeck, Germany: [CO2 monitors in 2200 classrooms and 28 nurseries](https://www.luebeck.de/de/stadtentwicklung/smart-city-luebeck/projekte-und-massnahmen/frische-luft-fuer-klare-koepfe.html). See also a [press article on that](https://www.luebeck.de/de/stadtentwicklung/smart-city-luebeck/projekte-und-massnahmen/frische-luft-fuer-klare-koepfe.html)
* Latvia: [CO2 monitors in 875 schools and social centers / 14000 classrooms](https://co2.mesh.lv/)
* Connecticut: Schools have a [state-wide grant for HVAC work to tap into](https://portal.ct.gov/das/grants/hvac-grants?language=en_US) and a [resource on terminology including DIY air filters](https://portal.ct.gov/hvacgrants/-/media/das/office-of-grants-administration/hvac-forms/air-cleaner-and-air-purifier-technology-guidance.pdf)
* French group "Nous Aerons" (Let's Air) lists [dashboards that show live CO2 levels for classrooms](https://nousaerons.fr/#dashboards). Their list includes many of the above.
* Australian activists have created [Covid Safety for Schools](https://www.covidsafetyforschools.org/) which is a comprehensive resource for teachers, parents, and students. The materials are initially for Australia but are applicable to any other country on earth. 

# Technologies we use and tools for fact-finding 

* See [site technologies](./site-technologies/)
* See [tools for working on entries](./tools-for-working-on-entries/)

# Site ownership

This site is edited by volunteers who are interested in accelerating the work to complete the adequate ventilation of schools. Volunteers includes parents and kids. This effort was not commissioned by education authorities or governments. The volunteers are in groups around countries, states, provinces, and cities.

If you want to launch another small country (e.g. Luxembourg), or a whole state/province (Nova Scotia), or a City (New York), you should have your own team ready to curate the entries for each school. A decent percentage of that team should have some software development skills and GitHub experience. You'd make a GitHub repo like `Wales` get it ready, then ask us to slot it into the main site. Pick a name that represents the hierarchy - Canada_Nova_Scotia)

[Edit this page](https://github.com/ventilate-schools/ventilate-schools.github.io/edit/main/index.md).

# SELF INTRO

## name, title, company
- meaning of design architect
	- i'm in this role because of a new path we've taken in dev and design
	- it's far from perfect yet, but we've learned a great deal on the way
		- i'm here to share some of what we learned

## i'm also on the company softball team
![hnnnnggggg](http://tottara.kounatta.com/picture.php?/6309/search/62)

## and the bowling team
![bowling](https://scontent-a.xx.fbcdn.net/hphotos-xpf1/t1.0-9/1240043_10153264417595014_313566537_n.jpg)

---

# TOPIC INTRO

## confessions of a sass hater
HEADLINE: "Sass won't fix this, let's focus on bigger problems"
- "Sass won't help you write better CSS; it creates an incentive to make the worst parts worse"
	- nesting
	- mixins duplicate rules, dissuade responsible one-to-many class definitions
	- mixins may also discourage smart element defaults


## warming up to sass
After 4 years...
- realization that sass is an indication of the maturity of our field
	- package management
	- optimization through pre-compilation
	- polyfills
	- variables
	- functions
	- calculations
- as long as you realize that at the end of the day Sass compiles into a declarative language, you're golden.

## what "future tools" means
We have more at our disposal than ever before (modern browsers, standards, the rise of github, etc).
This talk won't be covering new technologies in web development; it's about
the tools we can build right now to push our craft forward and hone the process
of making a product for the web.

---

# yes, meetup has a design team now
[oldthemes](https://docs.google.com/a/meetup.com/presentation/d/1d1l0ijsVgnhS9scNJzQXsYGP1ZB4JzMp0DTR08TQ3sw/edit#slide=id.gdd6f5325_320)
- without a design team, this was not only ugly, it lacked good UX design.
	- Allowing changes to text colors and background colors
		- color blind orgs made horrible pages for users with normal vision
		- orgs with normal vision made horrible pages for color blind users
- tl;dr, if there were a design team involved in the decision, one of meetup's biggest missteps may not have happened

## dark ages of design at meetup
- no central voice
- you could tell who built a page
- inconsistent brand
- inconsistent UI
- awful code
- making the users do our job
	- "the leadership team"

---

# (bad) workflow examples
### TODO: chart of segmented, siloed development

# GOOD workflow examples
### TODO: chart of "design vocabulary/foundation" as the middle layer

---

# TOOL #1: style foundation
- "It's up to you how you want to define 'foundation' depending on your needs, but here's how we think of it at Meetup"
- why live style guides fail
	- overly specific "legos" (there's a tool to fix that)
	- documentation is hard to maintain (there's a tool to fix that)
	- we don't live in a web-only world anymore (there's a tool to fix that)
	- require cut-over rewrites (there's a tool to fix that)

## document flow, rational css, SMALL SHARP TOOLS
- unix philosophy and CSS
	- markup flexibility
- interface first
- smart element defaults
- modifiers!
	- about class semantics
	- about concern separation
- __extends rely on selectors, selectors rely on ancestry = markup + style tightly coupled__
- keeping the foundation low-level
	- keeps updates infrequent, reduces regression risk
	- keeps "interface" easy to understand

### TODO: set up one-to-many demonstration with modifiers vs. extends

### Why is separation of content and presentation a best practice in the first place?
It encourages loose coupling between style and content, allowing them to change independently

### "Semantic" style modifiers via Sass extends:
	- generates selectors that have a one-to-one (selector-to-element) relationship
	- without applying a class to an element, you must create an ancestry-based selector (or ID)
		- if the DOM changes, the style might break
		- you ould use all IDs instead, but why
	- As a result, the relationship between presentation and content is more likely to be tightly coupled, as the CSS needs to know about the DOM

### "Unsemantic" modifier classes:
	- class selectors have a one-to-many relationship with DOM elements
	- the DOM ancestry can change, and the applied classes will still work
	- the coupling between content and presentation is loose, because the CSS does not need to know about DOM structure

### WHY STYLEGUIDES FAIL...
- doubling up on styleguide/api
- docs go stale

---

# TOOL #2: Hologram
1. show hologram homepage
2. show completed sassquatch docs
3. show some code in sassquatch (tables, one html_example)


---

# TOOL #4: The Cascade
Strangler vines!

- cascade is a thing
	- style ordering is an instruction, as much so as any style
	- that's why we don't have Sass path globbing; it's the same as the compiler throwing out code
	- use it with intent!
	- ... and it makes CSS the perfect candidate for strangling!

---

# TOOL #3: Rothko, because native apps matter

---




TODO: http://shayfrendt.com/posts/upgrading-github-to-rails-3-with-zero-downtime/
TODO: separate outputting from non-outputting sass

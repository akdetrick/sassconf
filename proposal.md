# Notes

### Main points
1. Making the most out of a custom framework
2. Ensure design ideas make it to the end
3. Make the old new


### talking points
- Sass has matured to something beyond a convenient way to write css
	- you can do things with Sass that you couldn't do before
- Design consistency is code consistency
- How to design style systems with Sass
	- specificity, etc
- Design-driven development?
- making the most out of a live styleguide and component library
- cross-platform colors!
- **tools-first approach**
	- sassquatch
	- swatches
- standardized patterns help kill legacy CSS
	- strangler applications

### Materials
- shane's inventory (of old shitty stuff)
- strangler vine photos
- sassquatch svg
- flowcharts, lol


### [design-driven development](https://www.youtube.com/watch?v=cBydEpkXl_c) notes
- consistency == value == trust
- define the problem and let designers do their job


---------------------

# design-driven development (or a less boring title)

Live style guides are widely accepted as a best practice in building user interfaces, but they don't always live up to their promise in practice.

As a Design Architect at Meetup, I've facilitated the transition from ad-hoc UI code to a more modern approach over the last 3 years. We've learned a great deal about what works and what does not when trying to implement a custom CSS foundation and other design-driven tools.

In this talk, I'll be going beyond the basic idea of a live style guide, demonstrating tools and techniques that can help your ideas thrive. Fully automated documentation, package management, cross-platform color management, authoring best practices, and the strangler pattern [1] will be covered.

This talk doesn't dive too deeply into advanced features of Sass, focusing instead on novel approaches to the process of building user interface with Sass. Beginners should be able to follow the topics presented, but all makers of the internet should be able to find relevance in this talk.

I'll be building on some material from related talks I've given at two NYC meetups, but bringing brand new ideas to SassConf. I want to leave attendees feeling empowered to tackle legacy code as well as ready to build their own custom style foundation.

All software referenced in my talk will be open source under the MIT License.

[1] - http://martinfowler.com/bliki/StranglerApplication.html

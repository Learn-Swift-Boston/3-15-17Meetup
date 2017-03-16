# 3-15-17Meetup

**Joe taught us about his experiences making tvOS apps**
* a short history of tvOS. 
* He taught us about the similarities between iOS and tvOS (tvOS is a subset of iOS). 
* We learned a little about creating tvOS UI
  * TVML -- javascript generates TVML that is then used to make the UI
  * Swift allows for more options when making a tvOS app UI, but TVML is quicker
  * There is limited capability to reuse nibs (with some slight modification)
* [Cocoapods](https://cocoapods.org/) allows you to import 3rd party libraries
* tvOS apps can only be 200 MB (but [App Thinning](https://developer.apple.com/library/content/documentation/IDEs/Conceptual/AppDistributionGuide/AppThinning/AppThinning.html) helps)
* Then got a walk through a few of the tvOS apps he and his team have worked on
  * We talked about some of the UI elements (tab bars, collection view, and the focus engine)
  * How tvOS uses the delegation pattern to inform you what item the user has selected using the Apple Remote
  * The different concerns about layout when developing for iOS vs. tvOS
  
**Lu did a presentation about size classes and how it can help make more beautiful apps that can transition from portait to landscape**
* how apps like YouTube and Duolingo use size classes to adjust the way, and the amount of, content that is displayed
  * and even how Apple's calculator and calendar apps can reveal hidden, extra, content
* Any x Any replaced with C and R (Compact and Regular sied screens)
* combining autolayout and size classes lets us show and hide content based on screen size or orientation
  * constraints can be conditionally added per size class either using "vary for traits" or the Size Inspector
  * look for commonalities between your different variations to simplify/reduce the number of constraints you need to create
* Sometimes all you need is a Stack Views to help you show/hide different elements
  You can checkout Lu's sample code on [her Github](https://github.com/neugierige/RotationDemo)

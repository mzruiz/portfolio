Hola!

My name is Matt and I'm from Philly, PA. I earned my Bachelor’s Degree of Computer Science in 2018 from West Chester University of Pennsylvania. Prior to college I spent weekends and summers as an apprentice in a relative’s Contracting company. I've always enjoyed working.

I no longer specialize in electrical outlets and now spend my time building mobile apps with React Native, JavaScript, TypeScript, Swift, Firebase, and more. I hope to use my experience as a Salesforce Developer/Trainer to push the boundaries of mobile development.  

To learn how I got to this point, please checkout my [about](https://github.com/chooch620/portfolio/blob/master/about.md) section.

### Table of Contents

- [Projects](#projects)
  - [TeenPros](#teenpros)
  - [BoxBets](#boxbets)

# Projects

## TeenPros

[TeenPros](teenprofessionals.com) has reduced the cost of local professionals by up to 80%. This mobile platform consists of two iOS applications, TeenPros: Requester and TeenPros: Worker, that work together to connect homeowners who need help and young people who want to work.

Currently, TeenPros services a few dozen users in the South Jersey area.

Initially, these apps were built using **Swift** and **Firebase**. There were two developers: myself and a friend Dan. We had weekly sprints for the 15 months up to our March 2020 launch and have since moved them to bi-weekly. We used **Github** to manage our issues and source code and utilized **Asana** to handle sprint planning/execution/retrospects. Neither of us had any mobile experience going into this and are happy with the MVP.

**Tools**
* Swift
  * We followed the [MVC Design Pattern](https://developer.apple.com/library/archive/documentation/General/Conceptual/CocoaEncyclopedia/Model-View-Controller/Model-View-Controller.html) set forth by Apple.
* Xcode
  * Project security, configuration, builds, testing, and development were done using the Xcode IDE (not like there's a choice).
* CocoaPods
  * Third-party applications were leveraged using the [Cocoapods](https://cocoapods.org/) dependency manager.
* MapBox
  * When a Worker is accepted for a job, they need to know how to get there. Instead of relying on Apple's or Google's Map applications, we decided to use MapBox to provide our own unique experience. Workers receive turn-by-turn navigation thanks to the [Navigation SDK for iOS](https://docs.mapbox.com/ios/navigation/overview/).
* Stripe
  * Instead of trying to handle this ourselves we leveraged the easy-to-use API given to use by [Stripe](https://stripe.com/). A custom multi-step checkout flow is provided to both the Requester and Workers. 
  * Both parties can provide unique codes at checkout which:
    * Can apply a discount
    * Can increase the $/hr rate for Workers
    * Support local organization
* Firebase
  *  A NoSQL database made sense due to the difference among job types. The JSON structure provided the flexibility needed.
* Node.js/Firebase Cloud Functions(FCF)
  * From Push Notifications to the handling of CRUD events, the combination of Node and FCF made implementing application logic seamless. 
  * Asynchronous processes were designed, executed, and tested in at a much quicker rate than its Swift counterparts.
* Apple Developer Program/TestFlight
  * After 8 months of development we were able to get the applications into the hands of testers and launched a focus group from October 2019 - December 2019. A few dozen users completed over 20 jobs during those three months.
  * Data collected from this focus group was used to streamline our registration and job creation process.


## BoxBets
[BoxBets](boxbetsapp.com) is revolutionizing your betting experience. Track, share, and keep your bets going with our mobile application. We focus on what makes daily-competition among loved-ones so great - and that's raising the stakes.

BoxBets is social media platform that supports:
* Posting images/videos,
* User profiles,
* Following other users,
* Liking/Commenting/Sharing,
* In-app purchases,
* and more.

**Tools**

* React Native/JavaScript
  * Reusable components are made using function components and hooks
* Redux
  * Application state is managed using [Redux](https://redux.js.org/)
* React Navigation
  * React Navigation 5 makes things easy with it's move towards a component-based API
* Jest/ESLint/CircleCI
  * Component, redux, user interaction, navigation, and E2E tests allow us to catch bugs and edge cases
  * Static code analysis makes sure we follow proper coding standards
  * Continuous Integration allows us to automate our builds so that we can fail faster
* npm
  * We used npm as our package manager
  * Many common components have been extracted to their own npm [modules](https://www.npmjs.com/~trouthousetech)
* Firebase
* Node.js/Firebase Cloud Functions(FCF)
* Stripe
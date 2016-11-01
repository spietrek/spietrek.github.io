---
layout: post
title: React Native
---

2015 was a good year overall. It was a year of regrouping after a tough 2014. During 2014, I worked on a very stressful project, working 70-90 hours per week for 5 months, and burned out (partially difficult client and partially me being a workaholic). I hit rock bottom around Memorial Day 2014 and vowed to never put myself in that situation again. I focused the past 18 months on a work/life balance and doing things I enjoy (learning new technologies and public speaking). The technologies I had the opportunities to work with in 2015 include AngularJS, iOS and Swift, and ReactJS. I hope to continue expanding my knowledge in those technologies and expand in others in 2016.

### 2015 Achievements

+ Major projects. I spent the majority of 2015 on three major projects.
  - A single page application hosted in SharePoint using AngularJS 1.4x.
  - An iOS project written in Swift.
  - Small ReactJS project in order to "kick the tires" using ReactJS.
+ AngularJS. I have spent the past 3.5 years developing in AngularJS and really enjoy it. It is a great library for developing single page applications. Furthermore, since I do a lot of work in SharePoint, it is a great library for developing single page applications for SharePoint. In 2015, I had the opportunity to be a tech lead on a 5-month project with an outsourced team. After spending the majority of my team building AngularJS applications as the sole developer, I was working with a team of 3 developers. This provided a great opportunity to design the application to support multiple developers. Really focused on using directives for everything.
+ AngularJS Seed Project. I am a huge fan of John Papa. He is a great teacher and has a similar development methodology as me. As many of the single page applications I build are hosted in SharePoint, I needed a framework which could be repurposed across my team. I took the Hot Towel application and enhanced it to work in SharePoint. This included hooking up a common service for data access with SharePoint lists and styling to work in a SharePoint site. You can find my [SharePoint Projects project](https://github.com/spietrek/SharePoint.Projects) on my Github.
+ ReactJS. I have always been interested in ReactJS with the amount of coverage it receives. Many of the people I follow on Twitter are ReactJS developers. I spent some time in 2015 reading up on ReactJS and always looked for opportunities to use it on a client project. Last November I was tasked with developing 6 components to be deployed to a SharePoint site with data stored in SharePoint lists. I could have selected any library but went with ReactJS. Wow! I was really impressed from the very beginning. I am a huge fan of the component model.
+ iOS and Swift. I have always been interested in creating iOS applications. I spent some time a few years ago learning Objective C and gave up due to the complexity and not having a Mac hurt as well. Late summer I finally got a Macbook Pro to use. Oh boy! What a joy. The OS X operating system "just works". All the tools I used on Windows (Brackets, Atom, Code) all work on OS X. I also had the ability to install Xcode and start playing around with Swift. I spent quite a bit of time in the Swift Playground working on different examples. In November I had the opportunity to work on a new iOS project which uses Swift. I can't say things have gone perfectly; however, it has been the most enjoyable developing time I have had in quite some time.
+ Editors. I came into 2015 using WebStorm. I found it a great editor for developing JavaScript applications. I ran into issues with it with version 10 on my Surface Pro 3 (the resolution was wonky and caused things to be too small to be read). I looked for alternatives and found Brackets. Brackets is a great editor. Simple, great plug-ins, and fast. I used Brackets on my 5-month SPA development. During the past few months I tried out different editors. My favorite editor at the moment is Atom. There are numerous plug-ins, and although it is not the fastest (especially in Settings), it is my preferred editor at the moment.
+ Presentations. After a slow 2014, I had the "bug" to start presenting again. I was able to present at SharePoint Cincinnati, SharePoint Saturday DC, SharePoint Saturday NYC, and SharePoint Engage.
+ Git. I have used Git for the past few years but didn't push my Git skills too far. On the iOS project, I was tasked with improving my Git skills. Firstly, my co-worker recommended SourceTree. What a great tool! I love being able to create a new feature and have SourceTree create a new branch for me. Secondly, I spent quite a bit of time reading up on Git and learning things in more detail.

### 2016 Goals

For 2016, my list of goals is ambitious. I would rather aim high and fall short rather than aim low and meet all my objectives.

+ Continue learning vanilla JavaScript including ES6 and ES7.
+ Expand AngularJS knowledge (1.5+ and 2.0).
+ Continue expanding ReactJS knowledge (React and Redux).
+ Build a prototype in [React Native](https://facebook.github.io/react-native/).
+ Build knowledge on creating Cloud-Native applications for Azure.
+ Build NodeJS skills.
+ Create 1 iOS/Swift application and deploy to App Store.
+ Update my [Building SharePoint Single Page Application using AngularJS presentation](https://github.com/spietrek/spsnyc2015) to AngularJS 2.0 and ReactJS.
+ Present at 4-6 SharePoint conferences (hopefully SharePoint Cincinnati, SharePoint Saturday DC, SharePoint Saturday NYC, SharePoint Saturday Chicago, SPTechCon Boston, and SharePoint Engage).
+ Write 4 technical blogs.
+ Look for opportunities to present at a non-SharePoint conference.
+ Attend the [RWDevCon Conference](http://rwdevcon.com/) in March.
+ Create my own ReactJS seed project.
+ Work/life balance.

React Native overview. Companies are always looking for silver bullets for their mobile development. Many applications such as Cordova and Ionic allow for write once, deploy everywhere through a WebView; however, HTML5 mobile applications have some disadvantages. React Native takes a different approach. React Native is “learn once, write everywhere”. With React Native, you can use the same code base for both iOS and Android assuming you use common components. React Native provides the necessary support to create to create custom components which target platform specific functionality (either components or API’s). <p> React Native is a framework from Facebook that lets you build native iOS and Android applications. Your application logic is written and runs in JavaScript. React Native uses the React programming model so if you are comfortable building web-based applications using React, you will be able to pickup React Native very quickly. <p> http://www.ibm.com/developerworks/library/mo-bluemix-react-native-ios8/ 

1.	Discuss React Native architecture. As mentioned above, React Native is built on React’s model of “virtual DOM”. Unlike React which targets browsers, React Native’s virtual DOM targets components which are true native iOS/Android components. This connection, or bridge, is handled by the React Native’s team creating JavaScript components to native components bridges using native code. React Native includes many of the native components; however, if there are cases where there are not React Native “bridges”, either another open-source developer has created the bridge or you can also create a bridge by writing Objective C, Swift, or Java code.

2.	Installation. Installation is straightforward and is detailed on the React Native Getting Started page. 
a.	Requirements include installing Homebrew (good package manager for OSX), Node.JS (4.0 or newer), and Xcode 7.0 (or newer). 
b.	Once Homebrew is installed, go ahead and install Node (brew install node), watchman (brew install watchman), and flow (brew install flow). 
c.	For Android development, if you did not install Xcode (which installs Git), go ahead and install Git (brew install git). You can find the rest of the Android setup installation instructions here. A couple notes on Android development. I went with using Genymotion for emulation. I also installed Android Studio. I attempted to run my application through VS Code’s debugger without Android Studio but ran into too many issues. Opening the application in Android Studio will configure the application to run through the VS Code debugger.
d.	To install the React Native command line tools, run the following command in the terminal. You may need to run with sudo if you receive an EACCESS: permission denied error.
i.	npm install –g react-native-cli
e.	To initialize a React Native application, navigate to the location where you want to create the new project in terminal, and run the following command. The React Native command line tools will create the project folder, run npm install, and create the iOS and Android projects.
i.	react-native init MyNewProject
f.	Your terminal should look like the following after a successful React Native init command.
i.		
3.	Walk through a sample application (e.g. folders, files, etc.). Once created, you can immediately run your application in an emulator. Let’s start with iOS. Open the iOS project in Xcode, select an emulator device, and run the application.
a.	Your application should look like the following.

b.	Select the emulator window and type Cmd + D to bring up the dev menu. On a physical device, you can bring up the dev menu by shaking the device.
i.	Reload: Will restart your application.
ii.	Debug in Chrome: Will allow you to use Chrome’s Developer Tools. I personally use the integrated VS Code debugger, which I will cover later, that allows me to set breakpoints, view watches, etc. within VS Code (under the covers, Chrome Developer Tools integrates into VS Code). Note: You may need to stop/restart the debugging occasionally due to timeout errors or when adding new files to the project.
iii.	Enable Live Reload: If enabled, will refresh the application in the emulator when a source code change is saved. Currently (version .21), when changes are made, the application is reloaded within the device. Hot module replacement will be coming in version .22. HMR allows for the current state to be kept so when JavaScript changes are made, you will not lose your state. This will save a significant amount of time during the development process.
iv.	Start Systrace: Will allow you to profile your application. Before starting the trace, you will need to install trace2html (brew install trace2html). After doing what you need, you can stop the trace from the dev menu, and the trace information will be displayed in your default browser. The React Native team has identified a handful set of slow performing activities you should review.
v.	Show Inspector: Will allow you to inspect a given component. This will include component type, style information, and margins/padding. In addition, it will show performance timing information for the application.
vi.	Show Perf Monitor: Will show performance information including memory and frames per second (fps).
c.	The sample application is simple but it shows quickly how quickly you can get a React Native application up and running. Now that we have seen the sample application running in the debugger and the dev menu, let’s turn our focus to the source code. <p> I have the application opened in VS Code. Let’s walk through the files and folders

i.	.vscode: VS Code specific files. This includes configuration files for React and React Native extensions and debugging configuration files.
ii.	android: Folder for the Android project.
iii.	ios: Folder for the iOS application.
iv.	.flowconfig: Configuration file for flow. 
v.	.gitignore: Configuration file for ignoring folders and files from your Git repository.
vi.	.watchmanconfig: Configuration file for watchman.
vii.	index.android.js: The entry point of your application for Android.
viii.	index.ios.js: The entry point of your application for iOS.
ix.	package.json: Configuration file for your application. Includes scripts to start the application, developer dependencies (not deployed with your application), and dependencies (generally end user dependencies).
x.	tsconfig.json: TypeScript configuration file.
4.	Walk through a sample component. Below is the code for the MyNewProject application. The details for the file are defined below.

a.	Import – The import is use to define which modules can be used within the React Native component. In the example above, we are importing React along with a list of other modules including the following:
i.	AppRegistry: JavaScript entry point to running all React Native applications.
ii.	Component: Base React Native component. Includes all lifecycle features needed to run.
iii.	StyleSheet: Abstraction similar to CSS style sheets used for layouts and styles.
iv.	Text: React Native component for displaying text.
v.	View: React Native container component that supports nesting. Maps to native component UIView and android.view.
b.	Class – Using ES6, we can create classes. Here we are defining our MyNewProject component which extends the base component. Each React/React Native component requires a render function to define how the component should be displayed. Within the render function will be our JSX. JSX is a JavaScript syntax extension similar to XML. You use JSX, similar to HTML, to define the subcomponents which will be used in the main component and to support binding. In the example above, each component will have only one root element. In the MyNewProject component, the parent is defined as a View. Within the view are three Text components to display verbiage. The class is used to hold other functions for business functionality.
c.	StyleSheet – React Native uses Flexbox, or Flexbox Layout model, through a polyfill to support all layouts and styles within the application.
d.	Exports (not shown) – For most components, we will need to export the component to make the module available in other components through their imports.
e.	RegisterComponent – Provides the JavaScript entry point of our application.
Components, Animation, and Events
1.	Cross platform components (e.g. View, ScrollView, ListView)
2.	Native components (NavigatorIOS, ActivityIndicatorIOS, SegmentedControlIOS, TabBarIOS, Android ones)
3.	Animation (LayoutAnimation)
4.	Events (Touchable / TouchableHighlight / TouchableOpacity, PanResponder / Responder, DeviceEventEmitter)
Native Communication
1.	Native Modules
2.	Native Views
3.	React-native-search-bar integration example
Cross Platform Options
1.	Platform.OS === ‘android’ || Platform.OS === ‘ios’
2.	Separate files with ‘*.android.js’ or ‘*.ios.js’
GitHub Viewer Application Walk Through
Tools
1.	Nuclide
2.	DecoSoftware
3.	VS Code
4.	Genymotion
Resources
1.	React Native site
2.	Videos (React, React Native, Flexbox, ES6)
3.	Books (React, React Native, ES6)
4.	GitHub (search for react native apps)
5.	Js.coach


[Leave Feedback](https://github.com/spietrek/Feedback/issues/new)

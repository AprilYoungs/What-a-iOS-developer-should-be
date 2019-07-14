# interview


## Tell me about yourself

### basic information


### work experience, what did you grow from that and project

### interesting in xxx.com

- make sure to review the company’s website and social media platforms before your phone interview. “You should be able to speak confidently about the company priorities, the industry the company is a part of, and how you can assist the organization in meeting and exceeding its goals,” says

## 

### tech interview

- start simple and then expand

- don’t afraid to ask questions

- following the S.T.A.R. method: Situation, Task, Action and Result. First, present and analyze a specific situation you faced. Then explain the task you had to accomplish and what steps you took to address the problem. Finally, describe what were the results of your efforts.

## questions, prepare

## questions

### Why do you want to work for this company?

- the reason why I want to quit my current job,


### explain your strengths and weaknesses

- weakness:非计算机相关专业,基础知识相对薄弱.  
  strengths:学习能力强,非计算机相关专业出身,能够学好iOS开发,能够根据使用需求不断的学习新知识,解决工作中遇到的问题. 比其他计算机专业的同事,对自然科学方面的认知比较多

  
  
  遇到不懂的问题, 尝试去理解,用已知的去解答, 或者说出自己可以实现的路径
 a perfectly acceptable answer to an interview question is “I don’t know, but” followed up with a train of thought as to how you would go about finding the answer or a first potential solution

## 測試的方法, 自動化測試
?? 查一下
## 性能優化的方向,及指標, 方法
内存优化, 避免内存泄漏, 僵尸对象, 图片文件优化, 音频文件优化, 数据库优化, 耗时操作在非主线程

#### [[⬆]](#contents) <a name='general'>General Questions:</a>

* What did you learn yesterday/this week?
> 我最近在学习数据结构与算法, 同时也在leetcode上做算法题的练习
* What excites or interests you about making software?
> 现在是移动互联网的时代, 基本上人手一台手机, 能够做一款好用, 提高生活便利性的软件, 让我觉得很有成就感.
* Which version control systems are you familiar with?
> Git 和 SVN 都有使用过, 不过我更倾向于使用Git, Git现在更加流行, 在开放的代码管理库 比如 Github, 码云上都是使用Git做版本管理.
* Do you have experience working with projects on GitHub?
> 在Github上边的项目一般是个人项目, 用来记录自己的学习和练习的项目. 没有在Github上跟网友合作开发过项目, 不过跟同事会合作开发公司项目.
* Do you contribute to any iOS open source projects on GitHub or a similar site?
> 这个目前还有没有, 不过我最近遇到一个问题, 我使用的一个三方库, 国际化做得不到位, 我准备改进完善一下他的国际化功能, 然后提交给第一作者
* Can you describe your workflow when you work on creating an iOS app?
> 1. 看原型图和UI设计图, 充分了解开发需求  2. 根据UI效果找到通用样式和组件, 创建基本组件, 并定义好主题样式. 3. 创建基本类, 一般是基本控制器. 4. 添加常用三方库, 网络请求, 约束, 还有其他检测 和 辅助类的 三方. 5. 开始按照MVC的架构编写代码 6. 写代码的过程中也会根据遇到的问题, 不断创建工具类. 7.代码写完, 自测通过后会给测试人员测试 8. 测试通过后产品验收. 9. 有问题的话, 重复 7.8 10. 准备好软件介绍相关资料, 提交应用到app store
* Are you familiar with CocoaPods? Can you explain what they are and how they work?
> 使用三方库的时候,一般需要去github上找到对应的版本, 然后下载拖拽到工程中, 然后链接framework,还要添加依赖的系统framework,这个过程比较繁琐. 如果使用cocoapods就简单多了. 我使用cocoapods来获取常用三方库, 它是一个管理三方依赖库的工具, 使用它可以指定三方版本, 也可以通过它来更新三方版本, 只要指定版本, 然后pod install就可以了, pod update 的话会更新到最新版本. pod库分公开库和私有库, 公开库是提交到官方论坛被审核通过的库, 使用时不需要指定路径. 私有库就是没有提交审核的库, 使用时需要指定路径. 私有库提交审核通过之后就可以变成公有库, 不再需要指定路径.
* In general, explain software licensing and how this applies to work we do.
> 定义了软件, 项目被合法使用和传播的范围. 不同的license定义了不同的权限, 这个一般在开源项目上使用. 目前还没有用到!!
* Describe your general testing practices when building an iOS app.
> 我目前一般是人工去测试的. 界面上会使用不同设备去看是否准确好看, 反复实验各种操作流程, 确认都能正确运行. 打印数据, 溯源, 寻找错误开始的地方并纠正.!! 
* How can apps support other languages, date formats and currencies?
> 在应用中配置国际化文件, 并选择优先语言, 配置不同语言的语料文件, 应用中使用到文字时, 要调用localized string, 应用会根据系统语言使用对应的当地字符串. 如果配置表里没有对应语言则使用优先语言. 时间格式和货币, 则可以根据获取当前系统的区域来调用不同的样式, 可以写一个函数来实现这个功能.
* What is Instruments and how is it useful?
apple 提供给用来debug,查看应用性能的工具. 可以用来查看运行内存使用情况, 并检测是否有内存泄漏, 还有僵尸对象的捕捉. 还可以用来看应用运行的帧率. 

#### [[⬆]](#contents) <a name='tech'>iOS Technologies Questions:</a>

* 解释一下消息轉發機制
> 因为OC是运行时语言, 编译时有方法没有实现也可以编译通过, 不会报错, 只有当程序运行到某个没有实现的方法时, 才会出错, 不过处理得当也可以避免报错带来的崩溃. OC运行方法时会动态的解析方法, 当运行时遇到未知的方法并不会直接报错, 而是启动消息转发机制, 去检测有没有动态添加的方法. 我们可以利用这个消息转发机制来拦截, 处理没有实现对应方法导致的程序崩溃. 比如后端有时会在返回的数据中返回 null 的数据, OC解析数据时会解析成NSNull 类, 然后后面的代码尝试去解释数据就会导致崩溃. 这个时候给NSNull类写一个分类, 并实现 forwardingTargetForSelector 方法, 把NSNull类无法实现的方法, 推送给对应的类(NSNumer,NSString,NSArray, NSDictionary), 就可以避免报错了, 让程序正常运行啦.

* Explain Handoff, and in general, how it allows iOS and Mac/web apps to communicate?

* What technologies/services are contained inside of iCloud?
* What is an iOS extension? Can you list a few examples of popular/common extensions?
* What is HealthKit?
* What is HomeKit?
* What is Apple Pay? Could you describe a way we could use it in our applications?
* Explain application sandboxing.
* What is VoiceOver? Explain some of the accessibility features included in iOS and how developers can utilize them.
* How does application multitasking work on iOS?
* What features does Game Center offer for iOS games?
* What are iBeacons?
* What is Cocoa/Cocoa Touch?
* Explain in general, what Core Audio, Core Data, and Core Location are, and how they help iOS apps.
* Describe the role of SpriteKit and SceneKit.
* What is Metal?
* What is the responder chain? How does it work?
* What are the different actions that buttons and other controls can respond to?
* What is the role of the application delegate?
* Explain NSUserDefaults. How would you serialize an array to disk?
* How would you store user's credentials?
* Explain Keychain Services.
* Why are caching and compression important on mobile devices?
* Explain ~/Documents, ~/Library, ~/tmp. What directory is ~ on iOS?
* How does AirPlay work? How would you use it (programmatically) to enhance the utility and presentation of an app?
* Give a brief overview of what sensors, IO and communication methods (Wifi, telephony, etc) are available on iOS. How can you make use of these?
* What are the hardware performance differences among the iPad 2 / iPad mini 1-3, iPad Retina, iPad Air 2, iPhone 5, 5s, 6, and 6+. What do these constraints mean for performance intensive apps?

#### [[⬆]](#contents) <a name='code'>Coding Questions:</a>

* What does Cocoa Touch include and not include?
* Why do Cocoa Touch classes start with two capital letters?
* What is Swift, what is Objective-C and how do they relate and compare?
* Explain why optionals are useful in Swift.
* Explain `NSError` and how it works (or doesn't) in Swift.
* How does `instancetype` work and how is it useful?
* When is `let` appropriate in Swift? `var`?
* Why and where is the `map` function useful.
* How do you track down bugs? What are your tools of choice?
* You found a bug in Cocoa. What do you do?
* There is a regression in a new distributed version of our app causing crashes. How do you mitigate it? How will you prevent new bugs from reaching customers?
* How are Objective-C classes implemented? Describe how the Objective-C runtime is implemented.
* What security does iOS offer to protect customers and privileged information?
* Our app downloads data and displays it immediately. In accordance with MVC where is the best place to perform the download?
* How does MVC influence the design of a codebase?
* What methods are part of the controller life-cycle? The view life-cycle?
* What design patterns does iOS make use of? What design patterns do you use in your codebase?
* What queues does iOS provide and how can you best utilize them?
* Give a brief description of how `UIScrollView` is implemented. How does it operate with gesture recognizers, multiple touches and the run loops?
* What API would you add or improve on iOS?

#### [[⬆]](#contents) <a name='ui'>Interface Questions:</a>

* What is the screen resolution of the iPhone 5, 6, 6+. and iPad Air 2?
* What units is the resolution measured in?
* Explain the purpose of Interface Builder, what is a NIB file?
* What image filetype should iOS UI assets be saved in?
* Describe some differences between a Storyboard and a standard NIB file.
* What is the device status bar? How tall is it in points? Is it opaque or transparent? What does it do during a phone call or navigation?
* What is a navigation bar? Can you show me an Apple app on your phone that uses a navigation bar?
* What is a tab bar? What is a toolbar? Compare and contrast them.
* What is a table view? What is a collection view?
* Describe when a popover is most appropriate.
* What is a split-view controller?
* What sort of content would be appropriate to place in a picker view?
* When are a label, text field and text view appropriate?
* What does a segmented control do?
* What is a modal view?
* What kind of notifications does iOS offer?

#### [[⬆]](#contents) <a name='design'>Design Questions:</a>

* What is an iOS app icon? Describe it as best as you can.
* What is the smallest size an app icon could be? What's the largest size it could be?
* Can an app icon contain any transparency?
* How does a Newsstand icon differ from a regular app icon?
* Explain a launch image.
* Describe the purpose of Auto Layout, and in general, how it works.
* Describe the role of animation in design of software.
* Describe the role of interactivity and feedback when designing software.
* What are some differences to take into account when building an iPhone app vs an iPad app?
* Describe the importance and role of prototyping when working on an app design.

#### [[⬆]](#contents) <a name='appstore'>App Store Questions:</a>

* How do In-App Purchases work? What can be purchased with IAP?
* Have you ever submitted an app to the App Store? Can you explain the general process?
* What is iTunes Connect?
* What is a provisioning profile?
* What is an App ID?
* What are the differences between Development and Production iOS signing certificates?
* How is TestFlight used? How were UUIDs used in ad-hoc app distribution?
* When do purchase receipts need to be verified?
* What is required to display iAds?


Threading — main vs. background thread
This question was masked as a tableview with bad scrolling performance.
First stop, cellForRowAtIndexPath. Sure enough, an image is being called from disk every time the system asks for a cell. That’s an expensive operation.
Instead of loading it on the main thread every time the tableView asks for a cell, we should move the loading to a background thread so that the main thread (which is where the UI drawing occurs) can proceed while that thread does some work and then update the UI once the loading in the background is done.
My first solution to this was to move the image loading code into viewDidLoad, put each image into an array and access a pre-loaded image each time. Sounds great but that solution might not scale. What if you have 500 images? 10,000 images?
Another solution could be to use background threads and keep the main thread free of image loading blockage. This was the right answer.
This means we need to separate the code that loads the image and sets the image (this was done in one line) into two lines so it can go into 2 queues
I ended up using a GCD dispatch_queue to solve this. I also could have used an NSOperationQueue or block.
Views — frames and bounds and lifecycle methods
Next up, a view which loaded in portrait mode but when rotated to landscape stayed in portrait. This one seemed pretty simple but taking a step back, there are a lot of ways to solve this. Which one do we choose?
Size classes? Auto layout constraints? Storyboard or code? UIViewController Rotation methods such as willRotateToInterfaceOrientation:duration: and such?
I don’t really want to write constraints in code or in storyboard during a quick programming challenge — this probably isn’t the right approach and I suspect the interviewer is looking for something more practical.
Is there a solution that might be faster than another?
The problem was that the view was setting its frame once in viewDidLoad to the superview’s frame (portrait mode) and on rotation it was never reset. So how can we reset the frame each time it rotates?
Sounds like a lifecycle method could be appropriate here.
I chose to override viewWillLayoutSubviews and set the view’s frame to the bounds of its superview. This works because it’s called before the system actually lays out the view hierarchy and it gets called on rotation.
There is likely a better solution but given the time constraints, it did the job
Dependencies and coupling — protocols, delegates, notifications
Here is where things got interesting. I’m not going to go directly into what was discussed. Instead I’ll let Mr. Socrates take over from here.
What is code coupling? What does it sound like?
What’s a dependency? How might an object depend on another object?
Can you have more than one dependency? Can you have no dependencies?
What is the impact of depending on multiple objects? Does it mean something is tightly coupled?
When can we use coupling advantageously? When is it disadvantageous?
Can something be loosely coupled?
What’s strong decoupling? (not a real question, more of an inside joke! but this does sort of make sense in a double negative kind of way)
What design patterns does Objective-C use that would be considered tightly coupled? Loosely coupled?
What is a one to one coupling/relationship? One to many?
Where would you categorize delegates, protocols, and notifications within this framework of thinking?
Bonus: What is dependency injection? Why might it be useful?
Learning List and Questions To Consider
Things that did not come up during a mock interview but I found interesting to think about in no particular order.
Describe Atomic vs. Nonatomic
Which one is default behavior?
Does using atomic mean you get thread-safety?
Why would you choose to use one over the other?
Thread safety
What does it mean to be thread-safe?
What objects are thread-safe? Non thread-safe?
Memory management
What is ARC? Why does it exist?
What’s it doing under the hood? How did it used to work before ARC?
What is memory?
How much memory does our app get to use?
How much memory is on an iPhone 5, 6, 6s, 6+?
How can we respond to memory warnings in our app?
Retain Cycles
What’s a strong reference? Weak? How about copy, assign, retain?
Which types of objects typically use each type in property declarations? Why?
Why should you try to avoid retain cycles?
How would you create a retain cycle?
How would you break a retain cycle?
Blocks — when to use self, __weak self, __strong self
__weak self — what does this line of code do?
__strong self — how about this one?
Why do we care about the above 2 lines of code?
How do these answers help you understand retain cycles?
Views — rendering, layout and subview management
What is a UIView responsible for?
What is a frame? Bounds?
What happens when a user touches the screen? How does the system decide what view handles a gesture? Can you override that behavior?
What does is UIView’s superclass? How might this help you understand how the system determines which view receives touch events?
What methods are called throughout a view’s lifecycle?
Can you think of ways those lifecycle methods might be useful?
Other Important Lifecycles
What states can an application be in?
What methods are called before an application displays something on screen?
How does the UIViewController lifecycle work? What methods are called? When are they called?
How can we respond to these lifecycle events?
Objective-C Runtime
What does this term mean?
What role does NSObject play in all of this?
What does it mean to be “Objective-C”? Can you describe what C is?
How did Objective-C become Objective? What methods does the runtime implement to make messaging between objects happen?
Were there any languages that were inspirations for Objective-C?
Are there any interesting things we can do by understanding how Objective-C works under the hood?
Stack vs. Heap
What is the stack? The heap?
Why does Objective-C primarily allocate memory on the heap?
Does it have anything to do with the way it uses pointers?
What’s a pointer?
How long does the stack exist? The heap?
What implications does this have for memory management?
Explain how a UITableView and UITableViewController work together
How does the interaction between these classes utilize the delegate pattern?
How does it make use of protocols?
Why did Apple make the choice to implement a method to dequeue a cell and reuse it? Might this have something to do with memory management?
What kind of design decisions could you make to ensure smooth tableview scrolling?
# WhitehousePetitions
Repo following Project 7: Whitehouse Petitions - JSON and NSData on www.hackingwithswift.com. The goal is to learn how to parse JSON and get familiarity with UITabBarController.

The second part of this project follows Project 9: Grand Central Dispatch at www.hackingwithswift.com.

## Concepts Learned/Practiced in Project 7
* Parsing JSON
* UITabBarController
* NSData
* ```guard``` keyword
* Continued use of ```if let``` for optional binding to see if an optional has a value and assigning to a variable or constant if it does have a value.
* Simple error handling
* Adding another tab to UITabBarController which displays another view controller(done in code)

## Concepts Learned/Practiced in Project 9
* Grand Central Dispatch(GCD) framework
  * ```dispatch_async()``` method
* Closures - used in concert with the ```dispatch_async``` to wrap code that is to be executed asynchronously on background queues.
* Four background queues (in order of highest to lowest priority):
  1. User interactive queue
  2. User initiated queue
  3. Utility queue
  4. Background queue
* Using ```[unowned self] in``` to avoid strong reference cycles
  * Example from project:

  ```
  dispatch_async(dispatch_get_global_queue(QOS_CLASS_USER_INITIATED, 0)) { [unowned self] in

    //code wrapped within this closure...
    
  }
  ```
## Attributions
* [Project 7: Whitehouse Petitions: JSON and NSData @ www.hackingwithswift.com](https://www.hackingwithswift.com/read/7/overview)
* [Project 9: Grand Central Dispatch @ www.hackingwithswift.com](https://www.hackingwithswift.com/read/9/overview)

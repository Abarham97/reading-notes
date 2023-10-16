## shared preferences:
- it is used to save small collection of key-values A SharedPreferences object points to a file containing key-value pairs and provides simple methods to read and write them.
- calling the shared preferences :
    - getSharedPreferences() : Use this if you need multiple shared preference files identified by name.
    - getPreferences(): Use this from an Activity if you need to use only one shared preference file for the activity.
- When naming your shared preference files, you should use a name that's uniquely identifiable to your app. A good way to do this is prefix the file name with your application ID. 
- to Write a shared preferences file Pass the keys and values you want to write with methods such as :
    - putInt() 
    - putString()
- To save changes :
    - apply() 
    - commit()    


## Espresso 

- Espresso  is used to write UI TEST 

- Espresso tests state expectations, interactions, and assertions clearly without the distraction of boilerplate content, custom infrastructure, or messy implementation details getting in the way.

- Espresso is targeted at developers, who believe that automated testing is an integral part of the development lifecycle. While it can be used for black-box testing, Espresso’s full power is unlocked by those who are familiar with the codebase under test.

- Packages :
    - espresso-core - Contains core and basic View matchers, actions, and assertions
    - espresso-web - Contains resources for WebView support.
    - espresso-idling-resource - Espresso's mechanism for synchronization with background jobs.
- Espresso tests consist of two primary components: UI interactions and assertions on View elements. UI interactions include tap and type actions that a person may use to interact with your app. Assertions verify the existence or contents of visual elements on the screen
-  Run > Record Espresso Test->Select Deployment Target window, choose the device on which you want to record the test. 

## Lifecycle of a task and its back stack

- Task:

A task is a collection of activities that the user interacts with when using an Android app.
Each app can have multiple tasks running simultaneously, each with its own back stack.
Tasks are isolated from each other, and their activities do not directly interact with activities in other tasks.

- Back Stack:

The back stack is a stack-like structure that holds a history of activities within a task.
When you launch a new activity, it is added to the top of the back stack.
The user can navigate between activities by pressing the back button, which pops activities off the stack in reverse order.

- Lifecycle of a Task:

When an app is launched, it typically starts a new task with a single activity at the root.
As the user interacts with the app, activities are added to the task's back stack.
Activities in the back stack are paused or stopped when they are not in the foreground.
When the user presses the back button, the top activity is popped off the stack, and the previous activity in the stack becomes visible.
The user can also navigate to specific activities by launching them directly from other parts of the app.

- Task Affinity:

You can specify a task's affinity using the android:taskAffinity attribute in the manifest file.
Activities with the same task affinity are grouped together in the same task.
This can be useful for defining the relationships between activities and how they interact with each other across different tasks.


## Questions
1- What is a technology you’ve used before that is similar to Shared Preferences? 

i think it was redux in reacte 

2- Why is testing important? Give at least 4 reasons, and explain which is the most important to you and why.

 - Identifying Bugs and Issues.
 - Quality Assurance.
 - Documentation and Verification
 - Regression Testing

 - Identifying Bugs and Issues is the most importent beacuse you have to make a prograem without any problem.


3- Create an analogy for Tasks and the back stack. Have we used a similar system before? Explain

 Imagine you have a stack of books or plates, and each item represents an activity in your Android app. The top book/plate on the stack is the currently visible activity, and the rest are stacked beneath it, representing the history of activities in your app. As you interact with your app, you're essentially adding and removing items from the stack. When you open a new activity, it's like placing a new book/plate on top of the stack. When you press the back button, you're taking the top book/plate off the stack, revealing the one beneath it.
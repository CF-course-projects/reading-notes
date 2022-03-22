# The backstack
- The backstack is a stack wherein new processes are added on top of the stack
- when the user hits 'back' the top frame (most recent process added to it) is popped off the stack

## Back button fatigue
- for situations with many stacked instances -> 'back button fatigue'
- you can add launchMode="singeTop" to your activity's manifest page
- Or you can add the flag in your intent statement:
  - Intent.FLAG_ACTIVITY_SINGLE_TOP;
- The back button should NOT cross into different tasks
- Clicking a notification from a different app puts a new task in the foreground
- TaskStackGBuilder for notifications
  - TaskStackBuilder is a synthetic stack used to keep track of the processes created from notifications.

## Back press behavior for root launcher activities
- Root launcher activites are those which declare an ***intent*** fitler with both ***ACTION_MAIN*** and ***CATEGORY_LAUNCHER***
- These are unique activities because they act as entry points into your app from the app launcher and are used to start a task

### System behavior on Android 11 and lower
  - The system finishes the activity.

### System behavior on Android 12 and higher
  - The systems moves the acitivity and tasks to the background instead of finishing it. This activity is the same as when a user hits the home button

## Background and foreground Tasks
  - The background and foreground tasks are each a stack. The foreground task becomes the background stack when the users goes to the home screen or begins a new task
  - When in the background, all activities (stack frames) in the task (stack) are stopped, but the task remains in intact
  - A task can then return to the foreground so that the user can pickup where they left off.
  - Note: there can be multiple background tasks (stacks)

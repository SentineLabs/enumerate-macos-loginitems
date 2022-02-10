# enumerate-macos-loginitems
Xcode Playground written in Swift that will return a list of all applications that use SMLoginItem API to start up at user login. 

LoginItems can be included within an application's bundle, so simply checking the System Preferences "Users and Accounts | LoginItems" pane is no longer sufficient. 

This playground parses the backgrounditems.btm file and produces a readable output of all Login Items for the user account that owns that file.

Typically, the file is found at ~/Library/Application Support/com.apple.backgroundtaskmanagementagent/backgrounditems.btm.
    
Note, that "Login Items" is a specific mechanism for persistence defined by Apple and is unrelated to any other means of persistence like LaunchAgents, etc.

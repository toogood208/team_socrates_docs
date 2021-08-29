# HNGi8 Team Socrates Flutter Docs

> Please read to get familiar with the whole flutter project strucure and architecture we're using.

[Click this to go to the main project repo](https://github.com/zurichat/zc_app)

The main aim of this doc is to provide team socrates with a overview of the various functions, constants, etc. That have been declared in the project.  

Please do ensure that you read through and follow this guides appropriately.
Thank You.

* [app-routing:](app_routing.md) This directory contains the app router files that are used to navigate between the screens of the app. **app_navigator.dart** contains simplified MaterialPageRoutes functions, **app_router.dart** handles the actual screen to be navigated to based on the string provided by the **router_names.dart** file.
* [general-widgets:](general_widgets.md) This directory contains the list of widgets classes that can be reused in the different parts of the application.
* [package:](package.md) This directory contains API and local database operations; the only two ways the application is provided with data or sends data out. *This can be repackaged and published later as a standalone plugin/package.*
  - **base/local_db:** This directory contains and manages anything related to the CRUD operations.
  - **base/server_request:** This directory contains separate classes for requests made on the api (POST, GET).
* [utilities:](utilities.md) This directory contains subdirectories for utility classes, functions, mixins and even extension classes.
  - **constants:** Houses constant values like the base API url.
  - **extensions:** Houses dart extension methods.
  - **mixins:** Houses mixin dart files .

* [view-models:](view_models.md) This directory houses the all the view model files. That is, a viewmodel class to a screen as viewmodels are used to house the data of a specific UI - separating UI code from logic code.
* [views:](views.md) This directory houses the UI dart files. A subdirectory is created for each screen where everything related to the screens are saved.

* [Example:](examples.md) You may find some project usage examples here, maybe, just maybe.
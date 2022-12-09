General comments for both files

1.there are no any try catch have been used in all the files. We must use the try catch so that we can handle error and return a response if any error occured.

2. There are no any comment against any function that will be help ful of the new developers


BookingController.php
1. we can use Auth::user() instead of $request->__authenticatedUser in wholecontroller. Because we have to use the laravel authentication method for
authorizing the user and getting the detail of the authorized user.

2. In the update method we can use the laravel array except method that is Arr::except instead of using the core php function. There is no problem if we use the 
array_except function but we are in laravel framework so our first periority is to use the laravel available method and functions.

3. In whole controller you are using $request->__authenticatedUser first we have to check that the user is logged in or not. Or we can place all these routes that are 
hitting in this controller in the Auth middleware.

4. Almost code is good and the naming convention of the variable is also good a developer can easily understand the what is the purpose of the variable and functions. 
So there are no any important and big changes are required in the bookingcontroller.php file.



BookingRepository.php
1. In the getUsersJobs function to getting the emergencyJobs and noramlJobs, we can use the laravel query function instead of running the loop.

2. there are no any try catch have been used in all the test case files. We must use the try catch so that we can handle error and return a response if any error occured.
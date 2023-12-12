# Structure

## Templates
* base.html: main template for navigating to other templates. Route: /
* add_driver.html: the template used for adding the driver. 
    * Route: /
    * After adding driver, the system will navigate to driver details and passes new driver's information to driver details to display
* courselist.html: the template used for displaying all courses. 
    * Route: /listcourses. 
    * Data passed: courseList (list of courses from database)
* driverdetails.html: template used for displaying driver details. 
    * Route: /driverdetails/<int:driver_id> . 
    * Data passed: driver_details (details of the driver), runs (details of the run).
    * Fromt his template, the system can navigate to edit run information and pass run details and driver details to update results for driver
* driverjr.html: the template used for displaying the list of junior drivers. 
    * Route: /driverjr
    * Data passed: junior_drivers (list of junior drivers)
* driverlist.html: the template used for displaying the list of drivers. 
    * Route: /listdrivers. 
    * Data passed: driverList (list of drivers from database)
    * From this template, the system can navigate to driver details to show all information about driver.
* edit_run.html: the template used for editing run information.
    * Route: /edit_run/<int:dr_id>/<crs_id>/<int:run_num>
    * Data passed: run details for editing and then pass driver details to update results for the driver.
* results.html: the template used for displaying results. 
    * Route: /results. 
    * Data passed: results_list (result for each driver), 
* search.html: the template used for searching drivers
    * Route: /search
    * Data passed: drivers (driver details for query database)
* top5graph.html: the template used for displaying bar charts. 
    * Route: /graph. 
    * Data passed: names (name of the driver), seconds (total seconds for each driver)

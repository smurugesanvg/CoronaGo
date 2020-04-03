## Installation

##### Frontend    
Run `npm install`  
Run `npm run hmr` &rarr; this will run the app in Hot Module Replacement mode. Configure the port number in `package.json` file. Default Port is 4202  
Run `ng build` or `ng build --prod`.   
Then copy the files in `dist` folder and paste it in the `Webcontent` folder in the backend

##### Backend

##### Demo
Please [click here for the demo.](docs/translations.md)
## API Codes needed

## Supported Login Methods
The application currently supports `Google login` method. But the application is extendable to accomodate login with `email` and `OTP`

## Logic
The application has 4 types of users in primary.
* Patient
* Doctor
* Hospital Admin
* State/Goverment Login
Any user of the application is a patient by default. The other permissions can be given in the `Applicaion Users` page.
    ##### Patient Information
    Patient can provide his basic information in this section. 
    ##### Patient Questionaire
    Patient fills the questions which mainly focuses on the symptoms. Based on the data provided in `Patient Information` and `Patient Questionaire`, the `Risk Level` (High, Medium, Low) of the patient is calculated.
    ##### Doctor Login &rarr; Not Yet Assigned
    Doctor can view the list of patients along with the risk score in this view. Based on the risk score doctor can decide wheter `Consultation is Required` or `Not Required` for that patient.
    ##### Doctor Login &rarr; My Patients &rarr; Not Yet Scheduled
    All the patients who are marked as `Consultation Required` will be shown here.
    ##### Doctor Login &rarr; My Patients &rarr; Scheduled
    Doctor can schedule consultation for a patient under the `Doctor Consultation` tab in `Patient Questionaire` page. The call will be over a GoToMeeting service. All the patients with whom the call is scheduled will be listed here.
    ##### Hospital Admin &rarr; Doctor Activity Log
    The admin can view the consultation status of each doctor for a particular day.
    ##### Hospital Admin &rarr; Stock in Hospital
    The admin can log the number of items (Gloves, Gown, Sanitizer) etc, which is in stock with the hospital and how many more are required.
    ##### State Admin &rarr; Heatmap
    This view shows the density of High risk patients on each area based on the zipcode they entered in the `Patient Information` page.
    ##### State Admin &rarr; Stock Level by Hospital
    This view shows the stock of items in each hosptial
    ##### State Admin &rarr; Stock Level by Item
    This view shows the stock in every hospital by each item.

## Contributing to the Project
Please refer the CONTRIBUTING.md file for more information

## Issue Reporting
All issues should be reported in the format given in ISSUE_TEMPLATE.md file.

## Code of Conduct
Any discussion/contribution on the project should follow the code of conduct as documented in CODE_OF_CONDUCT.md file.

## License

    


Contribution Guide
===================

Hello, and thank you for giving PriJour a try.
If You are not familiar with the 
- :doc:`Features and Functions <userManual>`,
be sure to check it out.



The source code is at https://github.com/dhruvinfo28/private-journal.


How to file a bug Report?
-------------------------
A bug report must be filed as a GitHub issue.


Try looking for a similar GitHub issues before creating a new one. If you don't find something similar, move on to the next step:


Include as much detail as possible in your report. Include a detailed overview of the bug. Add screenshots whenever possible.

Submitting Contributions
-------------------------
* Prerequisites include familiarity with GitHub and the project's  - :ref:`Tools and Technologies` . 
* Make yourself familiar with the source code.
* Fork the project.
* Identify any bugs or solve any GitHub issues and submit a pull request to fix them.
Opening a pull request
-----------------------

Before submitting the pull request, first describe the changes you made. You should write a descriptive title for your pull request, and then include more details in the body of the pull request. If there are any related GitHub issues, make sure to mention those by number.


Running the project locally
----------------------------
1. Clone the project.
On your terminal run the following command::
  git clone https://github.com/dhruvinfo28/private-journal



2. You must have mongodb installed. Follow `this guide <https://docs.mongodb.com/guides/server/install>`_ to install mongodb for your PC.
3. Run the command
in a new terminal::
   mongod
   
(*If there is no error message, move on to step 4.*)


You need to udate your Windows Path environment variable.For this:
      * Find Mongo's bin folder. (If you're not sure where it is, it's probably in  C:\\Program Files\\MongoDB\\Server\\4.4\\ , 4.4 was the latest stable version at the time,but this can be different for you)
      * Copy the path of the bin folder
      * Search Edit the System Environment Variables on your PC
      * Click on "Advanced" tab and then "Environment Variables"
      * Highlight the "Path" variable, click "Edit"
      * This will bring up the "Edit environment variable" window, click "New"
      * Paste your path to the bin folder. Make sure it ends with a \\
      * Press OK


Again run the mongod command. If should not give any errors.


4. In the server.js file
replace line 21 with::
 const MONGO_URI = `mongodb://127.0.0.1:27017/dbName`

(here dbName can represent any databse name)



5. Replace 
line 29 with::
  keys:['sample']
  
(where sample can be any name)



6. Open the middlewares/passportConfig.js
   and use your own `google OAuth credentials <https://developers.google.com/identity/protocols/oauth2/web-server>`_ for lines 18-19.

7. Run the following 
commands on the terminal::
    npm install
    npm run dev

8. The website will be live at port 3000.   
   

.. _Tools and Technologies:

Tools and Technologies
-----------------------
.. image:: assets/html5.jpg
   :alt: html
   :height: 50px
   :width:  50px

.. image:: assets/css3.jpg
   :alt: css3
   :height: 50px
   :width: 50px

.. image:: assets/js.jpg
   :alt: js
   :height: 50px
   :width: 50px

.. image:: assets/ml.jpg
   :alt: ML
   :height: 50px
   :width: 50px

.. image:: assets/ibmwatson.jpg
   :alt: IBM Watson
   :height: 50px
   :width: 50px 

.. image:: assets/nodejs.png
   :alt: NodeJs
   :height: 50px
   :width: 50px

.. image:: assets/mongodb.jpg
   :alt: MongoDB
   :height: 50px
   :width: 50px   


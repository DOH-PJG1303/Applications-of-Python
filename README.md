# Applications of Python

This repo contains training material, setup instructions, and code examples for the "Applications of Python" presentation.

## Start here!

### Python Setup

If you are interested in running any code or starting to work with Python, I would recommend that you start with the `python_setup.md` file.
Simply click into this file on your desktop computer and follow the step-by-step instructions. 
Note that python can take a while to download.
Afterwards, you can set up your own virtual environment by continuing to follow the instructions.
Note that when setting up the virtual environment, you might find it easy to work out of Visual Studio Code (see next section below).

### VS Code

If you would like to download Visual Studio Code, the most used IDE for developers, you can find the downloads page [linked here](https://code.visualstudio.com/download).
Visual studio code is a great IDE because you can add extensions, perform regex find and replace, split screens, manage Github, connect to databases, and access terminals all in the same location.
And that's just the tip of the iceberg!
Watch YouTube videos, search the web, or ask your favorite LLM about all of the cool features you can access via VS code.

### Explore!

Feel free to explore the repo from here on out!
As long as you downloaded Python and followed all the instructions in the `python_setup.md`, all of the code should be ready to play with.
Here are some things to note:

- Scripts with folders are setup in a numbered order of how they should be run or have been run.
  - in order to fully access the `02_web_scraping.ipynb`, you need to follow instructions and run the `01_selenium_setup.ipyb` file
- If you are a GitHub user and plan on making adjustments to this code / want to work out of this Repo
  - any file you add or label with a prefix of "secret" will be hidden from Github as described in the `.gitignore` file.  This feature is utilized in the `01_selenium_setup.ipynb`

---------------

### Notes on Record Linkage Data

Feel free to use the two synthetic datasets found as described by `Machine_Learning/Data/synthetic_df*.csv` to train a model of your own.
Please give credit to the owner of this data, PJ Gibson <peter.gibson@.doh.wa.gov> if you present your model at any conferences or in any papers.
Hare are a couple of things to note when you create your own model:
* There are data elements for more fields than [fname,lname,dob,phone,add] that can be utilized for model training.
  * The features that you utilize and compare should be dependent on the features available to you  
* The first synthetic dataset reflects the absolute truth behind the data on all fields.  The second dataset is a manipulation of the first with inserted missingness, typos, nicknames, field swapping, ect.
* You can choose your own blocking scheme.
* You can choose any model that you think performs best.  I found that the neural-network model was my best performing one. You may choose differently.
* It is not guaranteed that you will match the quality of human manual reviewers.  This synthetic data is not the exact data I used for my model training as described in the presentation.
* When creating the data, any person living in a building with 75+ units was given the same phone_landline as all others within that same building_id.
  * A mobile phone number is something that is extremely identifiable, but can be shared in several scenarios unaccounted for in the larger simulation, hence the adjustment.  
  * Shared phone numbers are common in workplaces (extensions), prisons, schools, long term care facilities, and other congregate living facilities.


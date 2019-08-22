# Fall2019CourseProjectTDA
The RAIK383H course project for TD Ameritrade during Fall semester 2019.

# GitHub Student
GitHub offers unlimited private repositories to students. Your code is required to be in a private repository to adhere to UNL's academic integrity policy.

A .edu email address is required to apply to GitHub Student. Navigate to [settings](https://github.com/settings/emails) and add your huskers.unl.edu address to your list of emails.

Navigate to [GitHub Student](https://education.github.com/pack), log in with your GitHub account, and click "Get your Pack". Follow the instructions, verifying your identiy as necessary. It may take multiple days for GitHub to approve your request, so apply early.
* Note: due to a policy change by GitHub involving huskers.unl.edu addresses, your huskers.unl.edu email may not sufficiently verify your identity as a student. If you have an option to submit additional identification, you may submit a picture of your NCard or download an Unofficial Transcript from MyRed (which shows your in progress classes for this semester). GitHub support said that an NCard may not be sufficient, but upperclassmen have used it successfully.

# Cloning the Repo
Only 1 person needs to clone the repo per team. Once this section is done, the remaining members of the team will clone the new repository.

## Option 1
There is a "Use this template" button on the [starter code project repo](https://github.com/raik383h/Fall2019CourseProjectTDA). You can hit that button and follow the UI.

## Option 2
Open Git Bash and navigate to the directory in which you want to place the project.

Run `git clone https://github.com/raik383h/Fall2019CourseProjectTDA.git`. This clones the project on to your repository.

Run `cd Fall2019CourseProjectTDA`.

Run `git remote remove origin`. This disconnects your copy of the repository from the original repository.

Create a private repository under your account on GitHub. Name it `Fall2019CourseProjectTDA`.

Run `git remote add origin https://github.com/<username>/Fall2019CourseProjectTDA.git`. This connects your local repository to your GitHub repository.

Run `git push origin master`. This pushes the code from your local repository to your GitHub repository. The code should now appear on GitHub.


## Adding Team Members

You have now successfully cloned the repo. Now you need to add your team members as collaborators so they can contribute code.

Go to Settings > Collaborators in your GitHub repo (https://github.com/<username>/Fall2019CourseProjectTDA/settings/collaboration).

Add each of your teammates' GitHub usernames and click "Add Collaborator". This sends an invitation to each team member. Team members will need to accept their invitations. If an invitation does not go through, you may need to cancel it and resend it.

Once your team members have been added as collaborators, they can clone the repo to their machines by running `git clone https://github.com/<username>/Fall2019CourseProjectTDA.git` (note that <username> is the username of the person who created the private repo).

You should also add MatthewMeacham, lbogus, and raik383h as collaborators so we can see your repositories and evaluate your code.

You are now ready for development.


# Running the C# API
Open the `TDAProject.sln` solution file in [Visual Studio](https://visualstudio.microsoft.com/downloads/). Right-click the `Web` project, and hit "Set as StartUp Project". Then hit the green run button in the toolbar. 
> If you don't have the .NET Framework 4.7.1 SDK installed, you can download the developer pack from [here](https://dotnet.microsoft.com/download/visual-studio-sdks?utm_source=getdotnetsdk&utm_medium=referral) 

# Running the Angular UI
Make sure you have Node installed on your computer. You can test this by typing `node -v` in a terminal (we recommend either Git Base or Powershell for Windows). You should have at least version 8.9.x installed. If the command is not recognized or you have an older version, download and install NodeJS from [here](https://nodejs.org/en/).  

Ensure you have npm installed--this should be installed already if NodeJS is installed. You can verify by typing `npm -v` in a terminal. You should have at least v5.5.1 installed.
> If you cannot use the npm command, it likely did not get added to your [path](https://stackoverflow.com/questions/27864040/fixing-npm-path-in-windows-8-and-10)

Navigate to the project using the terminal, and then go to `app > tda-project-ui`.

Install the necessary packages to run the project from that directory with the command `npm install`.

Install the Angular command line interface with the command `npm install -g @angular/cli`. You may need to restart your terminal to use the `ng` command.

Add npm global modules to your path. This step may not be necessary if you've already added npm to your path according to the above steps. Run `ng` in your terminal to see if it already works. On Windows 10, search "path", which should bring up an option to "Edit the system environment variables". Select Environment Variables > Path > Edit. Select New and add C:\Users\<username>\AppData\Roaming\npm .

Run the UI project by typing `ng serve`. This command launches the server, watches your files, and rebuilds the app as you make changes to those files. Navigate to `http://localhost:4200/` to see your running front-end.

For editing the Angular front-end, we recommend using [Visual Studio Code](https://code.visualstudio.com/download).
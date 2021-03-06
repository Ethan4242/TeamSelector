## Synopsis
The Team Selector assigns people to projects. 

The program will take the inputed data, and output a close to optimal assignment in seconds. This output file lists the members of each project and the average on the team for each factor (Ex: Year in school, ability, cost, etc..)

Members can be a person, object or place and a project can be a team or location. Is it maleable and can be used for many different applications. All it takes is the creativity of the user.

## Main Method Code Example
Here is a brief example of the main sequence of the program. The program is meant to be run with the correct input files and then prompts the user for data needed.

Algorithm: Assigns all members to first choices, checks which team does not have enough people, deactivates that, and then reruns assignment without assigning to the deactivated team. This is repeated until all teams have enough members.


// Gets all of the Projects and the Members from the files

allProjects = reader.inputProjectInfo(minMem, maxMem,projectFileName);

allMembers = reader.inputMemberInfo(allProjects, memberFileName);

// Determines which projects are most popular and sorts the list

calculateProjectPopularity(allMembers);
sortByProjectScore(allProjects);

// Assigns members to teams and outputs to a file

runSimulation(outFileName);

## Motivation

At the University of Wisconsin-Madison, Insight Wisconsin (InsightWisconsin.org) is a student organization that does project-based engineering projects. We needed a way to reduce the hours it took to assign teams, so we developed this application that could consistently and accurately assign members to teams.

This application has cut down the assignment of 100 members from 4 hours to 2 or 3 seconds.

Additionally, this has been a learning experience for the developers, so this is not meant to be a commercial application. This is meant to give people a way of assigning members to teams in an easy way.

## Installation
1) Type the code below in the command shell or terminal.
git clone https://github.com/Ethan4242/Team-Selector.git

2) Download the appropriate project and member templates (See file format instructions)

3) Save the templates in the same folder as the .java files.

4) Compile the program using javac *.java in the terminal after cd Team-Selector

5) Run the program by typing
java TeamSelector

## Contributors

Original Authors: Ethan Young and David Seamon

This is an open source project that anyone can contribute to. Feel free to locate issues and add features to this project.

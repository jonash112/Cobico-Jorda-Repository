# Project Title: Digital Task Tracker using a Systemized Layout.

## Project Description
Many people, especially students, find it difficult to manage their tasks effectively. This is usually caused by busy schedules or frequent distractions, and this often causes them to forget responsibilities. Consequently, they experience stress and are needed to cram, often resulting in negative impacts in their productivity and well-being. 

## Project Objectives 
- To give students a means of effective task management.
- Allow students to easily organize and edit tasks.
- Make for a simple yet detailed orientation arrangement of tasks.
- Accesibility to daily or weekly tasks.

## Planned Features
- Task Name Edit
- Description
- Instructions or Steps 
- Timer 
- Option between Daily or Weekly Task
- Deadline

## Planned Inputs and Outputs
- Output: Shows the list of tasks the user has made, including finished and unfinished tasks

- Output: The code prints "Name of task: " 
  Input: The user inputs the name of the task, e.g. "Assignment in CS"
  
- Output: The code prints "Task Description: "
  Input: The user inputs the description, e.g. "This assignment is worth 10 points."
  
- Output: The code gives the user the choice between "Instructions" or "Steps" 
  Input: If the user chooses "Instuctions", the user then writes it in the paragraph form, e.g. "Make a flowchart that          calculates the time it takes for a car moving at 40km/h to reach from Manila to Cebu.". If "Steps", then the user writes      in the bullet form, e.g. 
  • Construct a flowchart
  • Calculate the time a car moves from Manila to Cebu moving at 40km/h

- Output: The code prints "Timer: "
  Input: The user inputs the "Timer", e.g. 1:30-2:00PM.
  
- Output: The option for task category to be "Daily" or "Weekly" is printed
  Input: If "Daily", the task is categorized as "Daily". If weekly, the task is categorized as weekly
  Option Outputs: "Daily": Daily Task || "Weekly": Weekly Task

- Output: The code prints "Deadline: "
  Input: The user inputs the "Deadline", e.g. 10/2/2025 at 4:00PM

- Output: Shows the entire description of the Task, e.g. 
  Task Name: Assignment in CS
  Task Description: This assignment is worth 10 points.
  a) Instructions: "Make a flowchart that calculates the time it takes for a car moving at 40km/h to reach from Manila to       Cebu."
  b) Steps:  
  • Construct a flowchart
  • Calculate the time a car moves from Manila to Cebu moving at 40km/h
  Timer: 1:30-2:00PM
  / Daily Task
  // Weekly Task
  Deadline: 10/2/2025 at 4:00PM
## Logic Plan
Pseudocode:
BEGIN
 Set ListOfTasks as an empty list
 
REPEAT
 Display "Task Name: "
 Input taskName then end line
 
 Display "Task Description: "
 Input taskDescription then end line
 
 Display "Would you like to provide Instructions or Steps?"
 Display "1. Instructions"
 Display "2. Steps"
 Input choice then end line

 if choice == "instructions" then
   Display "Enter Instruction(paragraph form): "
   Input instructions
  steps = None
else if choice == "steps" then 
   Display "Enter Steps(bullet form, type DONE if finished): "
  REPEAT
   if step != "DONE" then
   add step to steps
  endif
   steps == "DONE"
  instructions = None
endif

Display "Input Timer(e.g. 1:30-2:00PM): "
Input timer then end line

Display "Select Task Category"
Display "1. Daily"
Display "2. Weekly"
Input category then end line

if category == "Daily" then
  taskCategory == "Daily Task"
elseif
  taskCategory == "Weekly Task"
endif

Display "Deadline: "
Input deadline then end line
  
  ADD newTask TO taskList

CREATE newTask with:
          Name = taskName
          Description = taskDescription
          Instructions = instructions
          Steps = steps
          Timer = timer
          Category = category
          Deadline = deadline
          
Display "Do you want to add another task?"
Display "1. Yes"
Display "2. No"
Input moreTasks then end line
  add newTask to taskList
  until moreTasks == "no"

/Final Output
Display "||||| List of Tasks |||||"
for each task in taskList

Display "Task Name: " + taskName then end line
Display "Task Description: " + taskDescription then end line

if instruction != "None" then
  Display "Instructions: " + insructions then end line
elseif steps != "None" then
  Display "Steps: "  + steps then end line
endif

Display "Timer: " + timer then end line
Display "Task Category: " + taskCategory then end line
Display "Deadline: " + deadline then end line
Display "||||||||||||||||||||||||||"

END

## Contributors
- Jonash Miguel Aidan Cobico (encoder)
- Noah Jarelle L. Jorda (idea contributor)

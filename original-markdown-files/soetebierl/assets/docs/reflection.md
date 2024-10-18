# Procedure Assignment Reflection

Write a short analysis (~500 words) in which you explain what you did to meet the assignment's criteria. Use the criteria as headings to structure your reflection.

## How do your procedures address the needs of a "reading to learn to do audience"? Provide some specific examples that connect back to Redish's noted features of such an audience.
Reddish asserts that when "reading to learn to do", users value not only learning the steps, but understanding why they need to complete them (290). My first procedure, as a whole, is intended to fulfill this need. "Creating a New Save in Stardew Valley" provides context and meaning to the otherwise instruction-less character and farm creation interface. In my procedure "Planting and Harvesting Crops in Stardew Valley" under "Acquiring Seeds", I note that the reason the user needs to stay behind the counter is so that they open the shop interaction, rather than start the dialogue. Not only does this help them with this action, but also provides them with information to "transfer...to other situations that were not directly covered in the tutorial" (Redish 290).  Additionally, due to the complex nature of both of these procedures, I broke them down into sub-tasks so that the user was not overwhelmed by the volume of text and discouraged from reviewing the procedure from start to finish.


## How do your procedures follow the WTGA Staging, Coaching, and Alerting stylistic conventions? Provide some specific examples that connect back to the criteria from Hart-Davidson.

### Staging
Both of my procedures start with short blurbs that explain the goal to the user, and is followed by an in-depth list of pre-requisites. These combined actions mean that my procedures "orient readers to the task" and "adequately prepare the reader to complete the task" as Hart-Davidson specifies.

### Coaching
Each of my steps begin with "imperative verbal phrases" and in the case that a step is conditional or optional this is clearly indicated. Additionally, in cases where there is a specific expected result, such as tilling land in "Planting and Harvesting Crops in Stardew Valley", that outcome is specified. In cases where outcomes are variable based on user preference, like with the appearance selections in "Creating a New Save in Stardew Valley", an image was included to support the clarity of instruction without compromising the user's creative freedom.

### Alerting
All of my alerts are formatted consistently with block quotes to ensure that they are "visually distinctive" from the rest of the procedure. Additionally, the use of consistent formatting helps the user to mentally prepare for what the message will contain. One thing that varies is the introductory word. I use "Note:", "Tip" or no introduction in cases where a user needs to pay particular attention, but there aren't strongly negative consequences. I use "Warning:" to indicate when particular actions could have negative or regrettable consequences.

## How do your procedures follow your task orientation work? In other words, based on your audience and their goals, discuss how you oriented your SCA moves to the tasks.

### Creating a New Save in Stardew Valley
The scenario created for this procedure focuses on a user who is overwhelmed by choice. I have used my staging and coaching moves to provide structure to an otherwise freeform procedure. By dividing the process into three main moves (naming, farm selection, character creation) I have given the user concrete tasks to complete. I finish my coaching moves with a list of all the changes that need to be made as a way for the overwhelmed user to double check that they have completed the task correctly. My alerts help clarify to the reader which of their decisions will impact their game play permanently. Finally I included a supplementary section on how to make changes to elements of the game. While I reference this throughout the alerts, I include the bulk of the information at the end so as to not distract the user from the task at hand.

### Planting and Harvesting Crops in Stardew Valley
Because my target user is a prospective player, my pre-requisites detail both the pre-game and in-game requirements for being able to plant and harvest crops. Additionally, my coaching moves provide a detailed look at the mechanics that would have come naturally to a user that is familiar with the game. Additionally, because of my user's unique interest in RPGs I did my best to detail the, albeit limited, NPC interactions that happen in this procedure. My alerts are more focused on tips for best practice, rather than consequences both due to the nature of this task, but also to avoid dissuading prospective players from playing. While I found it important to include information on the optional steps, as it helped the prospective user understand the potential for expansion, I kept them until the end to ensure the user was not distracted from the tasks at hand. 


## How did you apply a basic docs-as-code editorial workflow to your assignment? Please provide specific cases with screenshots and/or links that can support your claims.
I began my use of docs-as-code by using different branches to complete the procedures for each task. Additionally, I made commits after each WTGA stage so that my work could be better legible for future reviews.

<img src="reflection screenshots\use-of-commits-task-1.png" alt="Screenshot from github showing commits for task 1" style="width: 700px">  <img src="reflection screenshots\use-of-commits-task-2.png" alt="Screenshot from github showing commits for task 2" style="width: 700px">

Once my procedures were at a stage where they were reviewable I submitted a pull request for each procedure.

<img src="reflection screenshots\pull-request-task-1.png" alt="Screenshot from github showing pull request for task 1" style="width: 700px">  <img src="reflection screenshots\pull-request-task-2.png" alt="Screenshot from github showing commits for task 2" style="width: 700px">

Once I had received feedback from my reviewers, I implemented those changes and summarized them in my commits.
<img src="reflection screenshots\summary-of-pr-changes-task-1.png" alt="Screenshot from github showing commit summary with pr changes for task 1" style="width: 700px"> 

<img src="reflection screenshots\summary-of-pr-changes-task-2.png" alt="Screenshot from github showing commit summary with pr changes for task 2" style="width: 700px">

One specific edit taken directly from the PR Feedback I made was to how I presented Steam in my pre-requisites.
<img src="reflection screenshots\steam-comment.png" alt="Screenshot from github comment on the confusion regarding steam" style="width: 700px"> 
<img src="reflection screenshots\steam-change-code.png" alt="Screenshot from github comment on the confusion regarding steam" style="width: 700px"> 

While I considered all the comments carefully, I did not blindly make the changes proposed by my teammates. For example, rather than delete the section on sprinklers and fertilizer that Camille suggested was taking away from the task orientation, I reorganized my information to include this blurb at the end of the procedure. I agreed that it took away from the user's task orientation, but I felt that this information was still vital for fulfilling the user's read to learn to do goal. 

<img src="reflection screenshots\optional-change-comment.png" alt="Screenshot from github of the comment on removing the sprinkler section." style="width: 700px"> 
<img src="reflection screenshots\optional-change-code.png" alt="Screenshot from github of the code moving the sprinkler section." style="width: 700px"> 

Once this reflection is complete, I will end my docs-as-code workflow by merging the pull requests with the main branch.

## How did you apply a consistent use of the Markdown language throughout your project? Please provide specific cases with screenshots and/or links that can support your claims.
I utilized Markdown to create a hierarchy of information. I did this first through my use of different heading levels to separate the WTGA moves, and nest tasks within each other where needed. For sections that were the same across both procedures, such as Pre-Requisites, I used the same level of headings.

<img src="reflection screenshots\use-of-subheadings.png" alt="Screenshot from code showing my use of headings and subheadings" style="width: 700px"> 

I also used both ordered and unordered lists to organize information. Unordered lists were use for non-sequential information such as pre-requisites, or the different farm types, while ordered lists were use to show the steps to complete each task.

<img src="reflection screenshots\lists.png" alt="Screenshot from code showing the different uses of unordered and ordered lists in my procedures." style="width: 700px"> 

All of my alerts were consistently formatted using the block quote style available through Markdown.

<img src="reflection screenshots\alerts.png" alt="Screenshot from code showing the consistent use of block quotes to format alerts." style="width: 700px"> 

I also made use of links to direct users to other pages where necessary.

<img src="reflection screenshots\links.png" alt="Screenshot from code showing use of links." style="width: 700px"> 

Finally, I utilized HTML in Markdown to reformat all of my pictures to ensure relatively consistent, and appropriate sizing for all my embeded images.
<img src="reflection screenshots\consistent-image-resizing-1.png" alt="Screenshot from code showing the different uses of unordered and ordered lists in my procedures." style="width: 1000px"> 



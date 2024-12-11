# **Plain Language Editing and Design Summary Report** 

Here is a link to our style guide: [https://docs.google.com/document/d/15c4obl2fMkcmaWNhAnnumP06cDu06EsDziN8KukJjDg/edit?usp=sharing](https://docs.google.com/document/d/15c4obl2fMkcmaWNhAnnumP06cDu06EsDziN8KukJjDg/edit?usp=sharing)

## **Revisions from Mini Topic Modeling**

After receiving the feedback from Dr. Lindgren, we made changes to our mini topic model in order to make it more usable for reuse, as well as making it more compatible with YAML when we began this project. 

### **Changes to Topic Model Structure**

We had  a few issues with the organization of our original topic model. The first was that we included the original markdown files that we were translating into DITA. While this was useful for us as we were drafting the initial model, the inclusion of these files could have potentially interfere with future reuse. Thus we removed these files from the final model (see this [pull request](https://github.com/ENG517/Topic-Model-3/pull/36))   
We also used a dense folder hierarchy to organise our initial topic model. We were advised that this level of organization posed an issue when thinking about re-use potential. Thus we decided to re-architect our topic model into a much simpler file structure. Files were grouped by topic, and all media was reallocated to the assets folder (see this [pull request](https://github.com/ENG517/Topic-Model-3/pull/37)).  

Finally we edited the topic references in the map to both reflect the new structure, and also to be easier to parse. For topic refs that were not parents, or did not have additional metadata were re-written to be self-closing we were able to make the maps much easier to parse. Additionally, we altered the indents and added in extra white space to emphasize the grouping and hierarchy of the topics (see this [pull request](https://github.com/ENG517/Topic-Model-3/pull/37) for the first map, and this [pull request](https://github.com/ENG517/Topic-Model-3/pull/40) for the other two).

### **Changes to Content**

One main issue we had was a concept topic that was better suited to be broken into multiple different kinds of topics. It was meant to set up for our task and references in our “intro to farming” section, about the differences between Joja Mart and Pierre’s General Store, but it ended up being too much information for one concept and would not be easily updatable. It was recommended to us by Dr. Lindgren that we break it into different concepts and references for each store, which was better suited to communicate the same information, but in a way that allows for reusability and better user comprehension. We ended up creating an introductory concept about store options, and then nested the references and concepts under this in the map. In doing so we were able to keep the information nested and organized, while making future edits and reuse easier (see this [pull request](https://github.com/ENG517/Topic-Model-3/pull/40)).

Another issue we had was with the “Intro to New Saves” concept. Our feedback suggested that the content was more task oriented than conceptual. While we initially attempted to revise the content to better fit the standards of a concept topic, we found that we needed to preserve the task oriented information. So, we created a new task topic that implemented the most important conceptual information in the form of prerequisites and context and utilized the main steps element to contain the task oriented information (see this [pull request](https://github.com/ENG517/Topic-Model-3/pull/43)). 

We also had an issue where our alerts for tasks were coded as “\<info\>” elements, which was not very useful for the addition of YAML to the project. We changed these alerts to “\<note type=”example”\>” in order to better categorize them, so they could be color coded using YAML and therefore be more eye catching to users (see this [pull request](https://github.com/ENG517/Topic-Model-3/issues?q=is%3Apr+author%3Ajckinsey01)). Additionally, we added “\<uicontrol\>” to any mention of buttons on screen to better communicate to users that these were actual buttons on the screen they could click (see this [pull request](https://github.com/ENG517/Topic-Model-3/pull/39)).

Other fixes were mainly small, organizational or aesthetic changes. Such as correcting the indentation for our short descriptions, deleting empty elements, fixing hierarchy issues with substeps, and fixing typos (see this [pull request](https://github.com/ENG517/Topic-Model-3/pull/41) and this [pull request](https://github.com/ENG517/Topic-Model-3/pull/44)).

## **Plain Language Editing**

When writing, we aimed to write in such a way that was straightforward, lacking in technical jargon and easy for users to understand, even if they were skimming our text quickly without reading in depth. To do this we kept sentences shorter, defined terms where needed, and kept titles concise and specific where needed. While there were minor  wording changes made here and there, we found that our existing information on the whole was well aligned with principles of plain language. Thus we focused a majority of efforts on improving the document design through YAML (see this [pull request](https://github.com/ENG517/Topic-Model-3/pull/44)).

## **Redesign with YAML**

For our YAML revision, we wanted the guide to feel like it had the same aesthetic as “Stardew Valley”. To us, this meant making the color scheme feel similar to the game and reminiscent of a farm, with yellows, greens, browns and blues. We went for more toned down, muted versions of these colors so they didn’t become overpowering. For our fonts, we wanted to prioritize readability while still feeling close to the game. We made our normal text dark brown so we could employ a softer feel to our text, and the headings were different colors to help them stand out. We also highlighted our alerts so that they stood out, and each color was chosen to reflect the purpose of the alert. Warnings were a light reddish brown, a lighter hue than the brown selected for the text, tips, used to show users tricks to enhance their gameplay, were green to emphasize improvement and growth, and notes about the general gameplay were blue, because it felt more neutral while still providing contrast to regular text.

We went with Swarabi Gothic (regular and bold) for our normal text, because it is readable. We selected more interesting fonts for our headers, with larger/higher ranking headers being larger and more pixelated (in order to be on theme with the pixel style present in Stardew Valley), and as they decrease in size and rank they become more similar to the plain text and less pixelated so as to be more readable. 

(See this [pull request](https://github.com/ENG517/Topic-Model-3/pull/45))

## **Final Note on Process**
A lot of this editing was done while both partners were together. Thus a lot of the back and forth on the PRs was done verbally rather than through GitHub. This is noted in the applicable pull requests.
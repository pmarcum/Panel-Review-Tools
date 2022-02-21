# Panel-Review-Tools
The below is a link to the Create Voting System spreadsheet on Google Drive: 

https://docs.google.com/spreadsheets/d/1kghxn7aBy22jxkettZE1ZcgyK_9PUyfzWmQnpr6Kojg/copy

If you hit the "Copy" button that appears when you follow the above link, a copy of the spreadsheet will appear on the "Shared With ME" folder in your Google Drive.  That copy, which will include the attached script that makes Create Voting System work, is yours to use as you prepare your review panels.  Note that you should move the spreadsheet down into a folder that you want to designate for the voting system files.  All of the voting system files will be generated UNDER the folder that you place Create Voting System into.

The script should work right out of the box.  You may have to "accept persmissions" when you first try running the buttons in the menu that allow you to configure the voting system format.  More specifically, to get through the authorizations (a one-time only task): 

"Authorization Required" --> click on the GREEN "Continue" 

"Choose an account" --> select the Google Account / email that you wish to use by clicking on it.

"Google hasn't verified this app":  

    --> scroll to the bottom and click on the small grey underlined "Advanced" in lower left corner.
    
    --> scroll down to bottom and click on small grey underlined "Go to createVotingSystem (unsafe)" at the very bottom.
    
"createVotingSystem wants to access your Google Account" --> scroll to the bottom and click the "Allow" button.

After the above steps, you will be able to run the scripts. 

Feel free to contect me if you run into permisison problems or if you notice any bugs as you use the code. 

-------------------------------------------------------

Create Voting System is a Google script-driven spreadsheet that generates voting management tools for proposal review panels.  Some files are generated for each panel, others are created to consolidate panel results. 

The files generated for each panel are:
* a voting ballot for each reviewer
* a scoresheet that provides statistics (mean/median/vote distribution/standard deviation) of votes for each proposal
* a dashboard that is a duplicate of the scoresheet but with an additional section that provides a view of each panelist's votes for each proposal.  This file is intended only  for use of the Panel Monitor, to allow monitoring of the panel (e.g., to make sure that each proposal receives all the votes expected, etc.).
* a "tracking sheet" that provides a list of the proposals under review by the panel and columns allowing the reviewers to indicate progress as they develop the final written evaluation for each proposal. 

-------------------------------------------------------------------------------------
UPDATES: 
02/21/2022 - I will be posting a YouTube video soon, describing how to use this tool

In addition to generating the panel-level files, a "consolidation" file is generated that is for the explicit use of the Program Officer who is overseeing the entire review.  This spreadsheet collects all of the final scores from each scoresheet in each panel, to faciliate an easy look-over of all proposals reviewed across all panels.  This file will also collect any special notes/comments made about proposals by the panelists. 

**Each file can be customized using Create Voting System to specify contents and whether to color-code the scores, whether to use adjectival or numerical scoring system, whether to display standard deviation, etc.**  The files can be made as simple or fancy as desired, with multiple review criteria and each criteria having several sub-criteria, or just a plain ballot with one evaluation criterion and no sub-criteria. You can choose the ballots and scoresheet to have scores and standard deviations color-coded, or just display as plain scores.  You can choose to have the ballots and scoresheet show only letter scores, or both letter and numerical scores.  
 
----------------------------------------------

Now we discuss each of these files in more detail: 

**Voting Ballot**:  This spreadsheet lists all of the proposals under review by the panel, and provides columns for the reviewer to type in their vote/score for each proposal.  Their vote may be one score for a single criterion (like scientific justification), or can be several "sub-criteria" that, when computed as a weighted sum, provide a "final" vote for that criterion.  There may also be more than 1 criteria to vote on (for example, in addition to scientific justification, which could itself have up to 10 subcriteria, one might have another criterion such as technical merit, which also could involve up to 10 subcriteria).  Up to 12 criteria can be included on the ballot, with each criteria including up to 10 subcriteria, if desired.   The weights involved in a weighted sum, in cases for which multiple sub-criteria are involved, are specified by the user when setting up the format for the voting ballot using the Create Voting System script.  The ballots also indicate if any of the proposals have "external reviews" (or "write-in" reviews, reviews by experts who are not full-time panelists).  The ballots also show the reviewer what role the reviewer plays on each of the proposals (e.g., Primary, Secondary reviewer or Conflict of Interest).  The ballot allows the role designation to be changed by the reviewer if the information is outdated and roles were changed just prior to the review meeting. 

**Scoresheet**:  This spreadsheet is linked to each reviewer ballot and records the mean or median (or both) of the votes for a proposal. The score distribution and standard deviation are also displayed, if set up to do so by Create Voting System.   The scoresheet can be set up to show the actual value of the standard deviation, or just a color-code (for example, red when a high standard devation and green if a low value). The spreadsheet is typically hidden from the reviewers until they have voted on all proposals in their panel, so as to not introduce biases in the voting.  During format specification, the scoresheet can be set up to show the scores with color-coding, or not.  Also, the scoresheet can be set up to only show letter (adjectival) scores, or also numerical scores.  The default format (which can be removed, if preferred) is to also include 3 columns that are filled out manually by the panels:  the final grade, the final rank number, and any comments about the proposal that might be a useful "prompt" for the Program Officer as a reminder why that proposal landed where it did in the overall list of proposals.  If any of these 3 columns are included in the format when setting up the files using Create Voting System, the information entered in those columns are copied into the consolidation file for use by the Program Officer overseeing the whole review. (see below)  The scoresheet also has a reviewer area in which the role of each reviewer is indicated, so that at a glance, one can determine who is the Primary, Secondary reviewers for a proposal. 

**Dashboard**:  This spreadsheet is identical to scoresheet, but also has columns revealing the individual scores of each reviewer, along with a column that shows a checkmark when the reviewer has completed his/her vote for that proposal.  The dashboard is a useful tool for the panel monitor to track progress of the review and to insure that all votes are received for each proposal.  This strategy allows the review to remain anonymous among the reviewers (the Panel Monitor is not a reviewer and does not vote), to prevent biases that may come with knowledge of the votes of colleagues.  The default format also provides a "lock" feature -- a check box that, when checked, will prevent that proposal's votes from being changed in the ballots.  Locking the proposal after completion of a vote is a good strategy, preventing accidental overwrites by the reviewer (as well as intentional attempts to change a vote after the voting period has closed). 

**Tracking Sheet**:  This spreadsheet is very simplistic and could probably benefit from improvements/bells & whistles, but for now it is just a plain spreadsheet with all the proposals listed, the Primary and Secondary reviewers listed for each proposal, and columns in which the panelists can use to indicate the progress of the development of the written evaluation for each proposal. 

**Consolidate Sheet**:  This spreadsheet is NOT meant for the panels, and not meant even for the panel monitors.  Only one file is created, and its purpose is to collect all of the typed-in final grades (and ranks and comments) from each scoresheet so that all the review information is consolidated into this single sheet, for use by the Program Officer(s) in charge of overseeing the entire review process.  The consolidation sheet is handy when performing "normalization" across the panels and reviewing the scores for proposal selection. 

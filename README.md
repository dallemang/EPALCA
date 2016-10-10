# EPALCA
Sharing Space for files for the LCA project for the EPA

# How to use the www.epa.gov project in TopBraid Composer

I have committed the entire project to github.  This means that when you check it out, you can just use the project as is in TopBraid.  Here's what you do (presuming you have already checked out the repository):

1. Open TopBraid Composer.  If you already have a project called www.epa.gov, either create a new workspace that doesn't have that, or ignore these instructions (for now; I'll see if I can figure out what is the most appropriate thing to do in this situation)

2. Right-click in the background of the Navigator pane.  Select New > Project ; General/Project . 

3. In the resulting window, put in the project name www.epa.gov

4. Un-click "Use default location", and browse for the folder www.epa.gov in the repository on your local drive. 

5. Click "Finish".  This creates a project in your workspace.  Verify that the contents of the www.epa.gov folder shows up in TopBraid.  If it doesn't, check the steps above and see what went wrong (mis-spelled directory names, etc.). 

6. Because the tool uses the FRS_XWALK TDB, which is made up of files too big for github, you'll have to get these files elsewhere, e.g., https://www.dropbox.com/sh/btqxfnplxrpx5xb/AADtp0U98O2D8C7r5Obnmp-Ra?dl=0

7. Copy the entire directory FRS_XWALK.tdb.data to your workspace, at the top level. Double-clickon FRS_XWALK.tdb to make sure TopBraid found it correctly. 

## Run the tool

8. Double-click on discoverytool.sms.ttl to open it. 

9. Under the menu "Scripts", select "Edit/View SPARQL Motion script".  The script should appear in graphical form.  Find the finale of the script (discoverytool:dt_Return).  Select it.  Click the "Run" button (a litle green triangle, leftmost icon in the SPARLMotion tab) to run the script. 

10. Navigate to owl:Thing / discoverytool:Demo, and select it.  There is one item in that class, which shows up on the right.  This is Acetic Acid (64197).  Double-click it to select.  The script will run on its own for a while. 

11. When it is done, you will be asked what to do with the results.  You'll probably want to infer them, so that you can browse and query them, so select "Infer result triples".  You can also Display them, but that probably isn't very useful. 


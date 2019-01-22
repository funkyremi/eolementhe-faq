# eolementhe-faq


1. [Error in the Workflow for European Parliament](#workflowEP)
1. [Two subtitles are displayed at the same time or in loop.](#dblesubtitles)
1. [File not found :( message when cliking on preview](#filenotfound)
1. [Speechmatics return a [object Object]](#object)


<a name="workflowEP"></a>
# Error in the Workflow for European Parliament

The workflow is organised in order to optimise the different steps / jobs and then a fast delivery.


* If something fails before the expand, it is worth to redo the workflow from start point, picking the file from the “server file”. 
* If a branch fails after the expand, it is worse to use a prepared reduced workflow that “retakes” the faulty branch. Select the correct output language and the pause addresses that has to be used for translation’s correction:
![](resources\reduced_wf.jpg)
 
If the platform is not accessible, use the [www.eolementhe.cloud](https://www.eolementhe.cloud)  where workflows should have been prepared : 

* If nothing has been made, load the workflow, change the person to be notified at each pause and launch all the workflow.

* If the English subtitle has already been made, drop it in the file lib to launch only translations and translastions’corrections on the following workflow : 

<a name="dblesubtitles"></a>
# Two subtitles are displayed at the same time or in loop.

It’s because of an overlap in time-codes : 

 

In this case, keep calm and rebuild correctly time-codes with no overlap. You can play the file, stop at a position and use TimeCode Icon to update it.

<a name="filenotfound"></a>

refresh the page (keys Control + F5)


<a name="object"></a>
# Speechmatics return a [object Object]
![Error message](resources\object.jpg)

This is because the volume /var/Eolementhe is not mounted on Speechmatics vm.

Connect to it and mount the volume ``sudo mount –a``

 

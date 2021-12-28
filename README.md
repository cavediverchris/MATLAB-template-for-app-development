# MATLAB Project Template For App Development
This repository contains the template files to set up a MATLAB Project for the purposes of building MATLAB Apps or Toolboxes (including blocksets). For further information on MathWorks, MATLAB and Simulink please check out the website (https://www.mathworks.com/company/aboutus.html).

# Why MATLAB Projects?
MATLABs Project are a feature within MATLAB that aims to provide a structed development environment both for solo development, but also for team working. This is achieved in collaboration with a revision control system such as Subversion or Git. At the time of writing, both Subversion (SVN) and Github are supported. In conjunction with the source control tool, MATLAB Project can be used to support both agile and robust development processes according to industry standards such as DO-178C, DO-254, DO-331 any many others.

A couple of the main reasons you want to use MATLAB Projects are:

- Easy integration with revision control systems
- Standardised development environment for all users

# How To Use This Template
To start using this template to support your workflow, you first need to initialise a new project:

  1. Start MATLAB
  2. On the Home Tab across the top of the screen, click "New", then choose "Project", then choose "From Simulink Template"
  3. From the window that appears, choose "Blank Project"
  4. In the pop-up window that appears, give your project a name (also update the Project Folder path with the name), and click "Create Project"
  5. Download this repository by clicking on the "Clone or Download" button then choose the option to "Download ZIP". Wait while the files are downloaded. 
  6. Extract the files from the compressed ZIP file in your downloads
  7. Copy the contents (excluded the high-level folder which contains all of the files) into the directory where you created your new project.
  8. Within Simulink Project, change your view to "All Files View".
  9. Highlight all of the files, right-click, and choose "Add to the project path (including child files)"
  10. Switch back to the "Project Files View".

The files are now included in Simulink Project for management (and adding to source-control). However there are some utility functions that need some more setup.

   1. Open the SLProjectFunctions folder
   2. Highlight "A_ProjectSetup.m", "B_ProjectCleanUp.m", "C_NewSubSystem.m", "D_InformReviewersAboutModels.m" and "E_ConfigurationSetup.m"
   3. Right-click and choose "Add Shortcut to ... General"
   4. Choose the Shortcut Manager node on the left hand side
   5. For "A_ProjectSetup", "D_InformReviewersAboutModels" and "E_ConfigurationSetup", right-click, choose Set Shortcut Action and choose Startup.
   6. For "B_ProjectCleanUp" use the same process, but choose Shutdown
  
 Close Simulink Project and re-open to ensure all utility functions are now called.
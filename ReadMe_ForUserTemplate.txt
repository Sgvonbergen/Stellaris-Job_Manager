##############################################
##############################################
######                                   #####
######    Job Manager                    #####
######                                   #####
######    The way to preset templates    #####
######                                   #####
##############################################
##############################################
#
# This is description of preset templates of Job Manager.
# 
# In the preset templates, you can modify only job priority templates, but not species right templates.
# The preset templates are applied on game start. So, they are NOT applied to saved game.
# 
# <Important!!>
#   The preset templates will be overwritten if a configuration set is saved as template in the game.
#   Once they are overwritten, there is no way to restore preset template in this save file.
#
######################
####  Way to Make  ###
######################
#	
#	1. Create empty mod.
#		- It can be created from 'Create Mod' in 'Mod tools' of Stellaris Launcher.
#		- Memorize the directory inputted here.
#		- Recommended to name your mod to be shown at close to Crisis Manager in the Stellaris Launcher.
#	
#	2. Copy all folders and files in "JobManager\ForUserTemplates"
#		- <folder of your mod>
#			- common
#				- scripted_variables
#					- Sdj36a_JobManagerTemplate1_scripted_variables.txt
#					- Sdj36a_JobManagerTemplate1_scripted_variables.txt
#					- Sdj36a_JobManagerTemplate1_scripted_variables.txt
#			- localisation
#				- replace
#					- CrisisManagerTemplate_l_<each language>.yml
#		* Never change names of files nor folders.
#		* Copy all files even if you do not edit all of 3 templates.
#	
#	3. Edit template files in "common\scripted_variables"
#		3.1. Select files to edit.
#		3.2. Change "@SdjConstTemplate*Enabled = no" to "@SdjConstTemplate*Enabled = yes"
#			- If it is "no", this template is ignored.
#		3.3. Edit each options
#			- All parameter is written as "@SdjConstTemplate1_job_<Job Name> = x".
#			  You can modify only the number in right side of equals.
#			  The meaning of the numbers are written in each template files.
#		3.4. Edit next files if you want.
#	
#	4. Edit localisation files.
#		3.1. Edit "Sdj_JobManager_Template_l_<language>.yml"
#	
#	5. Edit "<File Name>.mod" file
#		- <File Name> is the directory inputted at '1. Create empty mod.'
#		5.1. Add dependency list.
#			------------------------------------------------
#			dependencies={
#				"Job Manager"
#				"Job Manager."
#				"Job Manager [BETA]"
#				"Job Manager. [BETA]"
#			}
#			------------------------------------------------
#		5.2 Edit any other you want.
#			- Recommended tags: "Balance", "Economy"
#	
#	6. Test play and/or upload to Steam if you want.
#	7. That's all. Holistic goals clearly outweigh individual concerns.
#	
#	
#

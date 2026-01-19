# Groot2

Hi!

This repository contains updates about the release of [Groot2](https://www.behaviortree.dev/groot)
and (in the future) tutorials and learning material.

You can use submit issues here: https://github.com/BehaviorTree/Groot2/issues

## Changelog
  ### 1.8.1 (2026-01-18)  
  - [Bugfix]: license not initialized correctly
  - [Change]: disable port validation in Preferences
  - [Change]: add truncated link to "Recent project" button.
    
  ### 1.8.0 (2026-01-18)                                                                                                            
                                                                                                                                                                                                                                                                             
  - [New feature]: Tree Hierarchy Analysis. Groot2 now automatically detects problematic tree structures:                                                                         
       - Self-referencing trees - warns when a tree's SubTree node references itself (would cause infinite recursion)                        
       - Circular dependencies - detects cycles where Tree A → Tree B → Tree A                                                               
       - Warning banners appear directly in the graph view for affected trees                                                                
       - Trees with hierarchy errors are highlighted in red in the project tree                                                              
                                                                                                                                        
  - [New feature]:Keyboard Shortcuts Dialog (CTRL+H)                                                                                                             
       - Ctrl+S - Save current file in Editor mode (new!)                                                                                    
       - Ctrl+Z/Y - Undo/Redo                                                                                                                
       - And many more documented in the dialog                                                                                              
                                                                                                                                        
  - [New feature]: new "Darker" Theme and improved custom theme editor. See preferences.                                                                                                                
  - [New feature]: trees with only one tree now auto-open that tree correctly
                                                                                                                      
  - [Improved]: the welcome screens for Editor, Monitor, and Replay modes have been redesigned for better clarity and usability.
  - [Improved]: license status changes (expired, suspended, revoked) now show clear user dialogs.                                                        
  - [Improved]: the License tab in Preferences now shows the specific reason when a license becomes invalid.
  - [Improved]: ovable Model Editor. The Model Editor dialog can now be dragged and repositioned                    
                                                                                                                                        
  - [Bugfix]: fixed crash when viewing arrays in Blackboard - The Monitor's blackboard widget no longer crashes when displaying complex types like
   vectors or arrays (fixes #55, #77). Arrays now display properly with indexed keys.                                                                                                                                                                   
  - [Bugfix]: fixed thread safety issues in Monitor mode - The ZMQ communication manager no longer has race conditions that could cause sporadic crashes.                                                                                                                                                        - [Bugfix]: Fixed SubTree expansion failing to update the view state correctly                                                                  
  - [Bugfix]: Fixed port changes not updating the tree state properly (issue #251)                                                                
  - [Bugfix]: Fixed error tooltips stealing keyboard focus                                                                                        
  - [Bugfix]: Fixed opening files via --file command line when the previous mode was not Editor                                                   
  - [Bugfix]: Fixed license validation for floating licenses.
  - [Bugfix]: Opening a single XML file no longer prompts to save the previous project                                                                                     

  ### 1.7.1 (2026-01-04)

**New feature**
   
   A wrong port name is now displayed with red background, and the ToolTip is more visible

   <img width="500" alt="image" src="https://github.com/user-attachments/assets/75df5678-54b8-4737-b1b2-fe6b5af7de83" />


  - [Bugfix]: fix launch in Windows when another Qt version is installed in the system [issue 76](https://github.com/BehaviorTree/Groot2/issues/76) 
  - [Bugfix]: AppImage should be compatible again with Ubuntu 20.04. [issue 75](https://github.com/BehaviorTree/Groot2/issues/75)
  - [Bugfix]: When a licence is not activated, stop trying to reconnect and showing popup [issue 73](https://github.com/BehaviorTree/Groot2/issues/73)
  - [Bugfix]: adding node in Monitor View is not allowed [issue 71](https://github.com/BehaviorTree/Groot2/issues/71)
  - [Bugfix]: Do not reset viewpoint when changing tabs or program [issue 70](https://github.com/BehaviorTree/Groot2/issues/70)
  - [Bugfix]: workaround to real-time monitor and log viewer incorrectly displays subtree children with the same name [issue 56](https://github.com/BehaviorTree/Groot2/issues/56)
  - [Bugfix]: Minor UI icon bug [issue 41](https://github.com/BehaviorTree/Groot2/issues/41)

  ### 1.7.0 (2025-12-14)
 
 **Changes since version 1.6.1**.
 
 - [Editor]: Some users reported difficulties with empty ports creating attributes in the XML that were confused with empty strings. To prevent this issue, we added the following option in Settings

<img width="500" alt="image" src="https://github.com/user-attachments/assets/ba8736af-4d7f-4e46-8015-44f93054213d" />

- [Monitor]: some users reported that the "atio-zoom" when a breakpoint is reached is annoying, especially for large trees. For this reason, we added a check box to disable the autozoom and some convenient
  (intentionally redundant) buttons to select **Continue** / **SUCCESS** / **FAILURE** from the left panel.

<img width="1200" alt="image" src="https://github.com/user-attachments/assets/501c602d-af53-4289-99c9-6aba2cebe605" />
  

### 1.2.0 (2023-09-11)
- [Bugfix]: fixed crash when renaming a Subtree
- [Bugfix]: Prevent Model editor when double clicking a Subtree.
- [LogReplay]: add filter-in/filter-out to the Transitions table.
- [LogReplay]: add the ability to export the result of the query into a JSON file

### 1.1.1 (2023-08-12)

- [Bugfix]: fixed crash when inserting a node during the Creation of a Node connection
- [Bugfix]: fixed crash when pressing the button "Play" on an empty Log Replay
- [License]: when activating the PRO license, user is asket to agree with the EULA.

### 1.1.0 (2023-07-23)
- [Visualization]: improved layout for Pre/Post Conditions boxes.
- [Editor]: Adding the ability to save XML files using the same syntax used by Groot1 (disabled by default in Preferences).
- [Editor]: Added `ParallelAll` and `ScriptCondition` to the built-in nodes.
- [Editor]: allow files that only contain **include** tags, but not **BehaviorTree** to be loaded.
- [Monitor]: Breakpoints can now be saved/loaded from file.
- [Monitor]: Add compatibility with the Groo2Publisher in BT.CPP 3.8+. 
- [LogReplay/Monitor]: Log parsing will now use plugins. Users will be soon able to create their own plugins to save/load logs.
- [LogReplay]: the range of the log can be changed; in other words, you can zoom on a particular section of the timeline.
- [Licensing]: append license key to offline activation file.



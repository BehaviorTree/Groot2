# Groot2

Hi!

This repository contains updates about the release of [Groot2](https://www.behaviortree.dev/groot)
and (in the future) tutorials and learning material.

You can use submit issues here: https://github.com/BehaviorTree/Groot2/issues

## Changelog

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



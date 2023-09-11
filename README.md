# Groot2

Hi!

This repository contains updates about the release of [Groot2](https://www.behaviortree.dev/groot)
and (in the future) tutorials and learning material.

You can use submit issues here: https://github.com/BehaviorTree/Groot2/issues

## Changelog

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



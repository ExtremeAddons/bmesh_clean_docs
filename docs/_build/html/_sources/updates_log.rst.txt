.. _updates_log:

Updates Log
===========

1.1.203
-------

**Release date: 15-11-2024 (D/M/Y)**

- **Blender 4.3 Support - No Module Named toml**

    The Python module 'toml' is no longer included in Blender 4.3, it has been replaced by the tomllib module, this module is used to read the blender_manifest.toml file.

1.1.202
-------

**Release date: 13-10-2024 (D/M/Y)**

- **Bug Fix**

    When there was no object selected, an error occurred when pressing the 'Apply to selected' button, an additional condition has been added to prevent this error from happening again.

1.1.201
-------

**Release date: 14-06-2024 (D/M/Y)**

- **Compatibility with Blender 4.2**

    The new extensions/addons system uses a new blender_manifest.toml, which replaces the old bl_info, an update has been made to make Bmesh Clean compatible with Blender 4.2 while maintaining retro-compatibility with previous Blender versions

- **Save Preset custom addon path problems fixed**

    There was a problem, if the addon was not installed in the classic Blender addons path, in fact the save system was based only on that specific path, now instead, the addon will try to find the path to the ExtremeAddons folder, if it does not find it will attempt to create it at the path where the addon versions of Blender are contained 'Blender Foundation/Blender/ExtremeAddons', if this section does not exist, then the addon will create this folder in the custom addons path: 'addons_folder/ExtremeAddons'

1.1.200
-------

**Release date: 29-02-2024 (D/M/Y)**

- **Compatibility**

    This version has been made compatible with Blender 4.1, as some APIs have been modified in it, the addon is retro-compatible up to Blender 2.8

- **Online documentation Buttons**

    Bmesh Clean now has an online documentation system, with a button for each operator that will take you directly to the online documentation (Right click with mouse on the operator or properties)

- **Update Message System**

    The addon periodically checks for updates, and if there are any, it shows a message, the option can be disabled

- **Unofficial Version Alert**

    If the version of the Blender is in Alpha or Beta, the addon will show a message alerting, a button will be available to disable the alert

- **Interface Change Option**

    The addon now has an option to change the interface, the user can choose between 2 tipes of interface, the Classic and the Checkmark version

- **Ended support for Blender 2.79**

    The addon will no longer be compatible with Blender 2.79


# MauiApp2

Solution representation:

![image](https://github.com/user-attachments/assets/02958825-dddd-40e0-b827-af65116fa492)

When adding new page:
- need to insert this as first row: @page "/cats"
- add new page into `NavMenu.razor` -- location: `.\MauiApp2\Components\Layout\NavMenu.razor`
- - like this:
  -         <div class="nav-item px-3">
            <NavLink class="nav-link" href="cats or whatever new page is named">
                <span class="bi bi-plus-square-fill-nav-menu" aria-hidden="true"></span> Cats
            </NavLink>
        </div>
    
    

Testing some Android development using Visual Studio and Razor. 

Connecting an external Android device to Visual Studio 2022 for USB Debugging in App development (in Dec. 2023). The original info is from this Video

* open Visual Studio updater → Individual Components
* Install USB Device Connectivity
* In Visual Studio go to Tools → Android → Android SDK Manager
* open Tools Tab → Extras → Google USB Driver (install)
* Connect the device to the development machine, activate USB Debugging on the device
* open project
* select Debug configuration
* From the menu where you select the device (e.g. android emulator/Windows machine/etc.) select your connected device
* start

If in the process of debugging on local device get this error: `EmbedAssembliesIntoApk`
Follow these steps:
one is to double-click Android project Properties
select Android Options
disable `Use Fast Development(Debug mode only)`

# iOSApplicationAddons
Tweaks for jailed devices by loading it as an library on main app executable.

## Tweaks
List of tweaks.

### AppCake++ (Discontinued)
- Support AppCake v7.0.4 - v7.1.0 (Maybe even 7.1.1+)
- Removes Ads
- Removes AppSync Pop up
<br>
<a href="https://github.com/CrafterPika/Sideload-Apps/raw/master/AppCake/appcake_v0.5a.dylib">Download</a>

### ZipAppLite++ v0.1a (Discontinued)
- Most recent version patched it
- Removes Ads
<br>
<a href="https://github.com/CrafterPika/Sideload-Apps/raw/master/ZipAppLite/zipapplite_v0.1a.dylib">Download</a>

# How to use
- You need a [CydiaSubstrate.framework](http://crafterpika.ml/dl/libs/CydiaSubstrate.zip) and [libloader](http://crafterpika.ml/dl/libs/libloader.zip)
- Rename the <code>.ipa</code> extension too <code>.zip</code> and unzip it
- Open the main Executable (Example path: <code>/Payload/AppName.app/AppName</code>) in a Hex editor of your choice
- Replace all string with <code>/usr/lib/libSystem.B.dylib</code> to <code>@executable_path/Sys.dylib</code> and Save the changes.
- Copy from the <code>libloader.zip</code> the <code>Sys.dylib</code> in the directory of the App (Example path: <code>/Payload/AppName.app/</code>)
- Creat a new folder in the directory of the app called <code>libloader</code> (Example path: <code>/Payload/AppName.app/libloader/</code>)
- Copy the <code>[TweakName].dylib</code> you selected in the <code>libloader</code> folder
- Copy from the <code>CydiaSubstrate.zip</code> the <code>CydiaSubstrate.framework</code> in the <code>Frameworks</code> folder (Example path: <code>/Payload/AppName.app/Frameworks/</code>) if the folder does not exist creat it
- Compress the <code>Payload</code> folder back to an <code>.zip</code> and rename the zip extension to <code>.ipa</code>
- Use Sign tools like [AltStore](https://AltStore.io/), to install the application

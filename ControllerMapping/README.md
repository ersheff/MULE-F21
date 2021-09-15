# Controller Mapping

The Max patch in this folder has been created to automatically map and sort incoming data from various video game controllers. Still needs some testing and improvement.

<img src="img/controllerMappingScreenshot.png" alt="Controller Mapping Max patch screenshot" width="300"/>

It is intended to be used inside of a bpatcher. To create the bpatcher in your Max patch:
1. Make sure that the MULE21 folder has been added to your Max File Preferences under the Options menu
2. Open the patch that needs controller input and unlock (put in edit mode).
3. Create a blank new object (n key) and enter "bpatcher controllerMappingv2"
4. Expand the size of the resulting window so that you can see all of the controls.

Once in your patch and loaded, click "menu" to populate the menu with the available controllers, choose your controller from the dropdown list, click "poll 10" to start outputting data, then finally choose your controller type from the last menu to use the mapping/routing that works with your controller.
  
There are several outputs at the bottom of the bpatcher. Each will output values in the range 0-255. If you hover your cursor over the output, it will display a popup that tells you what the corresponding control is.

### Other Info

#### Playstation 4 Dual Shock 4 controllers
- Mac - works right out of the box over USB, most likely also bluetooth, easily recognized and mapped in Max
- Windows - not officially supported, but we should try this 3rd party utility https://github.com/Ryochan7/DS4Windows (Links to an external site.)

#### Xbox One controllers
- Mac - some compatibility, must be specific models that were released after the original console https://support.apple.com/en-us/HT211232 (Links to an external site.)
    - Xbox Wireless Controller with Bluetooth (Model 1708, model # found under battery cover)
    - Xbox Elite Wireless Controller Series 2
    - Xbox Adaptive Controller
    - Xbox Wireless Controller Series S and Series X
    - Likely only works over bluetooth (while getting power from USB)
- Windows - should work out of the box and be easily mapped in Max (can use this template patch Download can use this template patch )

#### Nintendo Switch controllers
- Mac - Appears that it will pair normally using bluetooth, just need to test mapping in Max https://osxdaily.com/2021/05/21/how-use-nintendo-switch-controller-mac/ (Links to an external site.)
- Windows - Individual Joy Cons should connect via bluetooth, but cannot easily be connected as a single unit (both joycons together)

#### PS3 controllers
- Mac - should pair normally via bluetooth
- Windows - unknown, probably won't work, but might pair via bluetooth

#### XBOX 360 controllers
- Mac - won't work, 3rd party drivers exist but are out of date
- Windows - should work automatically via a wired or wireless connection  (with separate USB receiver)

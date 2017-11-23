# SSP - a scalable size unit for texts
An android SDK that provides a new size unit - ssp (scalable sp). This size unit scales with the screen size based on the sp size unit (for texts). It can help Android developers with supporting multiple screens.

This is the sibling of the [sdp](https://github.com/intuit/sdp) size unit that should be used for non text views.

# Attention
Use it carefully! for example, in most cases you still need to design a different layout for tablets.

# Example
[Here](https://github.com/intuit/ssp/blob/master/ssp-android/src/main/res/layout/ssp_example.xml) is a single layout built using ssp:

![ssp example](https://github.com/intuit/ssp/blob/master/ssp_example.png)

And [here](https://github.com/intuit/ssp/blob/master/ssp-android/src/main/res/layout/sp_example.xml) is the same layout built using sp:

![sp example](https://github.com/intuit/ssp/blob/master/sp_example.png)

You can see that ssp scales with the screen size and the sp stays with the same size on all screen sizes.

# Getting Started

To add ssp to your Android Studio project:

  add compile 'com.intuit.ssp:ssp-android:1.0.5’ to your build.gradle dependencies block.
  
  for example:
  
  ```
  dependencies {
    compile 'com.intuit.ssp:ssp-android:1.0.5'
  }
  ```
  
See the [ssp_example.xml](https://github.com/intuit/ssp/blob/master/ssp-android/src/main/res/layout/ssp_example.xml) to see how to use to the ssp size unit.

For easy mapping of designs to ssp units, one can create designs with 300 pixels screen width - in this case each pixel in the design corresponds to 1 ssp.

# Note
The ssp size unit calculation includes some approximation due to some performance and usability constraints.

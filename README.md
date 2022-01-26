# A11yLabelForTest

Demonstrate the creation of an accessible name for an EditText field
using the android:labelFor attribute on a TextView.

This approach is improperly detected as a Critical failure of the "Accessible Name" rule by Evinced Mobile Flow Analyzer. 
TalkBack shows that it does work.

![Screenshot_20220126-085235 A11yLabelForTest](https://user-images.githubusercontent.com/85311885/151179128-378e84f4-d4f1-4243-96b5-222043cb35de.png)


It is detected as a failure of the "Item descriptions" rule by Android Accessibility Scanner:
"Multiple items have the same description. 
This clickable item's speakable text 'Field label' is identical to that of 1 other item(s)." 
Which is a fair statement of a minor issue, sometimes addressed by making the TextView 
invisible to accessibility services with android:importantForAccessibility="no".




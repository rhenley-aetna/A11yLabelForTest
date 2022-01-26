# A11yLabelForTest

Demonstrate the creation of an accessible name for an EditText field
using the android:labelFor attribute on a TextView.

This approach is improperly detected as a Critical failure of the Accessible Name rule by Evinced Mobile Flow Analyzer. 



It is detected as a failure of the "Item descriptions" rule by Android Accessibility Scanner:
"Multiple items have the same description. 
This clickable item's speakable text 'Field label' is identical to that of 1 other item(s)." 
Which is a fair statement of a minor issue, sometimes addressed by making the TextView 
invisible to accessibility services with android:importantForAccessibility="no".




# SlidingTabLayout-RightToLeft
Support Sliding Tab  In Right to Left language
 The Solution For Use Sliding Tab in Right to left Language;


for full support RTL, add this to your Pager Adapter class (FragmentStatePagerAdapter)

  if (Build.VERSION.SDK_INT >= Build.VERSION_CODES.JELLY_BEAN_MR1) {
     if(contecxt.getResources().getConfiguration().getLayoutDirection() == View.LAYOUT_DIRECTION_RTL){
        Collections.reverse(tabs);
     }
   }

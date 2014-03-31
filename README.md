SwipeRefreshLayout
==================

Modified android.support.v4.widget.SwipeRefreshLayout to make the animations more like Google Now.

### Changes:
* Added a 'mResistance' float variable to prevent the target layout from moving so quickly.
* Modified the 'REFRESH_TRIGGER_DISTANCE' from 120 to 190. (You can change that according to the resistance to fit the requirement, currently if you use a smaller number as mResistance, the distance trigger will also be smaller)

### Additional feature:
* Splite 'setColorScheme(int colorRes1, int colorRes2, int colorRes3, int colorRes4)' into two methods: 'setColorSchemeRes(int colorRes1, int colorRes2, int colorRes3, int colorRes4)', which can be used to pass color resource id to the progress bar; and 'setColorSchemeColor(int color1, int color2, int color3, int color4)', which can be used to pass the integer representation of colors to the progress bar.

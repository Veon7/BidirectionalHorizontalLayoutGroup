# BidirectionalHorizontalLayoutGroup
A Unity3D horizontal layout group that supports both left-to-right and right-to-left. Useful if you are building a UI for an RTL language such as Arabic, Persian, Hebrew, etc. or if you support multiple languages in your app.

The component works just like the default HorizontalLayoutGroup. The only difference is the addition of the "reverse" field. When "reverse" is checked, the layout is done from right to left.

![BidirectionalHorizontalLayoutGroup in action](https://raw.githubusercontent.com/hk1ll3r/ShowcaseOfBidirectionalHorizontalLayoutGroup/master/Resources/vid1.gif)

## Usage
### Git URLs
This is a standard Unity package you can add to your project using [Git URLs](https://docs.unity3d.com/Manual/upm-git.html).

Check out the showcase project to see a sample Unity project that uses this package. 
https://github.com/hk1ll3r/ShowcaseOfBidirectionalHorizontalLayoutGroup

### Unity Asset Store
This package is also available for free on [Unity Asset Store](https://assetstore.unity.com/packages/tools/gui/bidirectional-horizontal-layout-for-unity-ui-rtl-ltr-160659).

## Notes
The implementation is based on Unity's HorizontalLayoutGroup located below.
https://bitbucket.org/Unity-Technologies/ui/src/2019.1/UnityEngine.UI/UI/Core/Layout/LayoutGroup.cs

The Left and Right padding fields always refer to Left and Right respectively regardless of whether "reverse" is checked. However "children alignment" field gets reversed along with the children's order. Take the following examples.

### LTR mode
![BidirectionalHorizontalLayoutGroup in normal LTR mode](https://raw.githubusercontent.com/hk1ll3r/ShowcaseOfBidirectionalHorizontalLayoutGroup/master/Resources/vid2.gif)

### RTL mode
![BidirectionalHorizontalLayoutGroup in reverse mode](https://raw.githubusercontent.com/hk1ll3r/ShowcaseOfBidirectionalHorizontalLayoutGroup/master/Resources/vid3.gif)

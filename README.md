# ClaymorphicMobileNavMenu
Claymorphic Mobile Navigation Menu with animation for your Canvas Apps!

![ezgif-3-bb0863aeee](https://user-images.githubusercontent.com/86930618/181358227-a26a8700-b3b0-420f-94cb-0950870a2a4a.gif)



![image](https://user-images.githubusercontent.com/86930618/190909742-d0f29674-1906-4075-a2e6-7c4c1dc760b5.png)


This menu consists of a mixture of code and out-of-the-box controls.

To install the component, please follow these steps:

- Please download the .msapp from this repo,

- Import it into your application 

- Create 4 screens in your app - Screen1, Screen2, Screen3, Screen4. When you rename them, please make sure you rename the MenuScreenNavigate line in the Table function :)

- Change the MenuItems property to

Table(
   <br> {
     <br>   //this is the name of the screen
     <br>   MenuItem: "Home",
    <br>    // this is the screen you will navigate to when you select this item
    <br>    MenuScreenNavigate: Screen1,
    <br>    //if you are not comfortable with SVG's, you can use standard icons instead!  - just make sure you change the icon property of MenuIcon to              ThisItem.StandardIcon
    <br>    StandardIcon: Icon.Home,
    <br>    ID: 1
    },
   <br> {
    <br>    MenuItem: "Profile",
    <br>    MenuScreenNavigate: Screen2,
    <br>    StandardIcon: Icon.AddUser,
    <br>    ID: 2
   <br> },
  <br>  {
   <br>     MenuItem: "Settings",
   <br>     MenuScreenNavigate: Screen3,
    <br>    StandardIcon: Icon.Settings,
    <br>    ID: 3
   <br> },
   <br> {
    <br>    MenuItem: "Balance",
    <br>    MenuScreenNavigate: Screen4,
     <br>   StandardIcon: Icon.AddDocument,
     <br>   ID: 4
  <br>  }
<br>)

Change the StandardIcon to whatever out-of-the-box icon you'd like to use. 

<br> The component has five main properties:

![image](https://user-images.githubusercontent.com/86930618/190910148-087d22ae-4f6d-4305-b364-ed4880cd7178.png)

- MenuItems is the table of menu items pasted above,
- IconSVGorStandard - if you want your icons to be SVG's, set that to true. If you are not comfortable SVG's and want to use out-of-the-box icons instead, please set that to false.
- SVGActiveIconColour 1 & 2 - these are the two colours of our SVG which are making up the lineal gradient. If you'd like it to be single toned, please give both properties the same value
- StandardIconColour - if you choose to use standard icons instead of SVG's, this is how you will control the colour of your icon

I have added as many comments to the component itself to help you understand how it's built. However, if you have any questions, issues or comments - as always, please reach out to me on my socials and I'll be more than happy to help 😊

Kristine

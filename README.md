# ClaymorphicMobileNavMenu
Claymorphic Mobile Navigation Menu with animation for your Canvas Apps!

![ezgif-3-bb0863aeee](https://user-images.githubusercontent.com/86930618/181358227-a26a8700-b3b0-420f-94cb-0950870a2a4a.gif)



![image](https://user-images.githubusercontent.com/86930618/181357721-d4966ec4-9f76-4e88-b023-f2d4779969d1.png)


This menu consists of a mixture of code and out-of-the-box controls.

To install the component, please follow these steps:

- Please download the .msapp from this repo,

- Import it into your application 

- Change the MenuItems property to

Table( {
- //this is the name of the screen 
<br>  MenuItem: "Home", 
- // this is the screen you will navigate to when you select this item 
<br>  MenuScreenNavigate: Home, 
- //if you are not comfortable with SVG's, you can use standard icons instead! - just make sure you toggle the component property IconSVGorStandard to false :)  
<br> StandardIcon: Icon.Home},
<br> { MenuItem: "Add new", 
<br> MenuScreenNavigate: 'Add new', 
<br>  StandardIcon: Icon.Add },
<br> { MenuItem: "Profile", MenuScreenNavigate: Profile, 
<br> StandardIcon: Icon.AddUser }, 
<br> { MenuItem: "Settings",
<br> MenuScreenNavigate: Settings,
<br> StandardIcon: Icon.Settings },
<br> { MenuItem: "Documents",
<br> MenuScreenNavigate: Documents,
<br> StandardIcon: Icon.AddDocument } )

Change the StandardIcon to whatever out-of-the-box icon you'd like to use. 

- Create screens in your app to match the MenuItem name. 

- If you would like to use the animated SVG's, please note there are some additional steps to be carried out. 
The SVG code is contained within the MenuLogo image control - as we are changing the colour of the SVG's dynamically based on the active screen, we are using the Switch() function. I have recently blogged step by step how to achieve this - https://www.kristinekolodziejski.com/blog/building-a-beautiful-power-apps-mobile-navigation-menu-svgs-part-3


<br> The component has six main properties:

![image](https://user-images.githubusercontent.com/86930618/181357835-caf09661-1c7a-4f6e-9148-609713c40d92.png)

- MenuItems is the table of menu items pasted above,
- Animation - this is applicable to SVG's in this component only - if you want the active screen SVG to float, please set that to true, otherwise set it to fault.
- IconSVGorStandard - if you want your icons to be SVG's, set that to true. If you are not comfortable SVG's and want to use out-of-the-box icons instead, please set that to false.
- SVGActiveIconColour 1 & 2 - these are the two colours of our SVG which are making up the lineal gradient. If you'd like it to be single toned, please give both properties the same value
- StandardIconColour - if you choose to use standard icons instead of SVG's, this is how you will control the colour of your icon

I have added as many comments to the component itself to help you understand how it's built. However, if you have any questions, issues or comments - as always, please reach out to me on my socials and I'll be more than happy to help 😊

Kristine

# Fancy Flutter Alert Dialog

A flutter Package to show custom alert Dialog,you can choose between two themes 'Fancy' and 'Flat'

## Usage 

### Import the Package 
add this dependencies to your app
``` dependencies: fancy_dialog: ^0.0.1 ```
### Use the Package
add this import statement 
``` import 'package:fancy_dialog/fancy_dialog.dart';```
to show a Basic Dialog
``` showDialog(
              context: context,
              builder: (BuildContext context) => FancyDialog(
                title: "Fancy Gif Dialog",
                descreption: "This is descreption for fancy gif,you can load any image or gif to be displayed :), and you can choose between two themes Fancy and Flat",
                )
            ) 
         }, ```
 the ``` title ``` and ``` descreption ``` are required
 and the rest of the parameters are :
 * ``` okFun ``` : the function to be called when the user press Ok button (positive button)
 * ``` cancelFun ``` : the function to be called when the user press cancel button (negative button)
 * ``` cancelColor ``` : the color of the negative button, by default it's ``` Colors.grey ```
 * ``` oklColor ``` : the color of the positive button, by default it's ``` Colors.pink ```
 * ``` ok ``` : the text of the positive button, by default it's 'OK !'
 * ``` cancel ``` : the text of the negative button, by default it's 'cancel'
 * ``` animationType ``` : The type of the animation, there are 4 types,which are :

        * ``` FancyAnimation.LEFT_RIGHT ``` the default one
        * ``` FancyAnimation.RIGHT_LEFT ```
        * ``` FancyAnimation.TOP_BOTTOM ``` 
        * ``` FancyAnimation.BOTTOM_TOP ```  

 * ``` theme ``` : Fancy or Flat 

        * ``` FancyTheme.FANCY ```
        * ``` FancyTheme.FLAT ```

The dialog will be dissmised by default when the user click Ok or cancel, DON'T ADD 
```Navigator.of(context).pop()``` to  ``` okFun ``` or ``` cancelFun ```

## Contribution 
Feel free to contribute, to report a bug to suggest a feature, Thanl you :)
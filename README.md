# CUSTOM STYLE___Text / Button

### Screen Size

```
int MOBILE = 450;
int TABLET = 850;
int DESKTOP = 1024;
int LEARGE_SCREEN = 1280;
int FULL_SCREEN = 1980;

```


### TextStyle

#### Headline

```
TextStyle HEADLINE (context){

  var width = MediaQuery.of(context).size.width;

  if(width < MOBILE){
    return TextStyle(
      fontSize: 22,
      fontWeight: FontWeight.w600,
      height: 1.3,
      letterSpacing: 0.2,
    );
  } else if(width < TABLET){
    return TextStyle(
      fontSize: 28,
      fontWeight: FontWeight.w600,
      height: 1.35,
      letterSpacing: 0.3,
    );
  } else if(width < DESKTOP){
    return TextStyle(
      fontSize: 34,
      fontWeight: FontWeight.w600,
      height: 1.4,
      letterSpacing: 0.4,
    );
  } else if(width < LEARGE_SCREEN){
    return TextStyle(
      fontSize: 36,
      fontWeight: FontWeight.w600,
      height: 1.5,
      letterSpacing: 0.4,
    );
  } else{
    return TextStyle(
      fontSize: 40,
      fontWeight: FontWeight.w600,
      height: 1.6,
      letterSpacing: 0.4,
    );
  }

}

```

#### Sub Headling
```
TextStyle SUBHEADLINE (context){

  var width = MediaQuery.of(context).size.width;

  if(width < MOBILE){
    return TextStyle(
      fontSize: 16,
      fontWeight: FontWeight.w500,
      height: 1.4,
    );
  } else if(width < TABLET){
    return TextStyle(
      fontSize: 18,
      fontWeight: FontWeight.w500,
      height: 1.45,
    );
  } else if(width < DESKTOP){
    return TextStyle(
      fontSize: 20,
      fontWeight: FontWeight.w500,
      height: 1.5,
    );
  } else if(width < LEARGE_SCREEN){
    return TextStyle(
      fontSize: 22,
      fontWeight: FontWeight.w500,
      height: 1.55,
    );
  } else{
    return TextStyle(
      fontSize: 24,
      fontWeight: FontWeight.w500,
      height: 1.6,
    );
  }

}

```

#### Body Text

```
TextStyle BODYTEXT (context){

  var width = MediaQuery.of(context).size.width;

  if(width < MOBILE){
    return TextStyle(
      fontSize: 14,
      fontWeight: FontWeight.w400,
      height: 1.5,
    );
  } else if(width < TABLET){
    return TextStyle(
      fontSize: 15,
      fontWeight: FontWeight.w400,
      height: 1.55,
    );
  } else if(width < DESKTOP){
    return TextStyle(
      fontSize: 16,
      fontWeight: FontWeight.w400,
      height: 1.6,
    );
  } else if(width < LEARGE_SCREEN){
    return TextStyle(
      fontSize: 18,
      fontWeight: FontWeight.w400,
      height: 1.65,
    );
  } else{
    return TextStyle(
      fontSize: 22,
      fontWeight: FontWeight.w400,
      height: 1.7,
    );
  }

}
```

### Button Style
#### Primary Button

```
// Wrap on SizeBox and use SizeBox Width

double PRIMARY_BTN_WIDTH(BuildContext context) {
  final width = MediaQuery.of(context).size.width;

  if (width < MOBILE) {
    return 180;
  } else if (width < TABLET) {
    return 210;
  } else if (width < DESKTOP) {
    return 240;
  } else if (width < LEARGE_SCREEN) {
    return 270;
  } else {
    return 300;
  }
}



ButtonStyle PRIMARY_BTN(context){

  var width = MediaQuery.of(context).size.width;

  if(width < MOBILE){
    return ElevatedButton.styleFrom(
      padding: EdgeInsets.all(10),
      minimumSize: Size.fromHeight(44),
      shape: RoundedRectangleBorder(
        borderRadius: BorderRadius.all(Radius.circular(10)),
      ),
      textStyle: TextStyle(
        fontSize: 14,
        fontWeight: FontWeight.w600,
      ),
    );
  } else if(width < TABLET){
    return ElevatedButton.styleFrom(
      padding: EdgeInsets.all(10),
      minimumSize: Size.fromHeight(50),
      shape: RoundedRectangleBorder(
        borderRadius: BorderRadius.all(Radius.circular(10)),
      ),
      textStyle: TextStyle(
        fontSize: 15,
        fontWeight: FontWeight.w600,
      ),
    );
  } else if(width < DESKTOP){
    return ElevatedButton.styleFrom(
      padding: EdgeInsets.all(10),
      minimumSize: Size.fromHeight(56),
      shape: RoundedRectangleBorder(
        borderRadius: BorderRadius.all(Radius.circular(10)),
      ),
      textStyle: TextStyle(
        fontSize: 16,
        fontWeight: FontWeight.w600,
      ),
    );
  } else if(width < LEARGE_SCREEN){
    return ElevatedButton.styleFrom(
      padding: EdgeInsets.all(10),
      minimumSize: Size.fromHeight(62),
      shape: RoundedRectangleBorder(
        borderRadius: BorderRadius.all(Radius.circular(10)),
      ),
      textStyle: TextStyle(
        fontSize: 17,
        fontWeight: FontWeight.w600,
      ),
    );
  } else{
    return ElevatedButton.styleFrom(
      padding: EdgeInsets.all(10),
      minimumSize: Size.fromHeight(68),
      shape: RoundedRectangleBorder(
        borderRadius: BorderRadius.all(Radius.circular(10)),
      ),
      textStyle: TextStyle(
        fontSize: 18,
        fontWeight: FontWeight.w600,
      ),
    );
  }
}
```



###### © All right reserved by Faysal

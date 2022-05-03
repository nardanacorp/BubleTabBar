# BubleTabBar

# SetUp

Follow instruction in [TabBars](https://github.com/nardanacorp/TabBars)

# View Layout 

add below code on custom ( every view layout nameview.xml ) :

```
        <ir.nardana.bubletabbar.BubleTabBar
            android:id="@+id/BubleTabBar"
            android:layout_width="match_parent"
            android:layout_height="wrap_content" />
```

Added below custom item to top tag 

| Attributes | Value |
| ---------- | ----- |
| app:RadiusAll  | Integer |
| app:RadiusTopLeft  | Integer |
| app:RadiusTopRight  | Integer |
| app:RadiusBottomLeft  | Integer |
| app:RadiusBottomRight  | Integer |
| app:TitleSize  | Dimension ( dp,sp,.... ) |
| app:BoxShadowSize  | Integer |
| app:BoxShadowSizeX  | Integer |
| app:BoxShadowSizeY  | Integer |
| app:BoxShadowColor  | Color |
| app:BackgroundColor  | Color |
| app:BackgroundTapped  | Color |
| app:ColorTitleTapped  | Color |

# Coding Layout

After Casting to custom variable can access below function 

```
In Activity Main Body

val CustomVariableName = findViewById<BubleTabBar>(R.id.BubleTabBar)

In Custom View Or Fragment Or Inflate View

val CustomVariableName = viewname.findViewById<BubleTabBar>(R.id.BubleTabBar)
```

# Set List Flat Tab Bar mutableListOf

```

var mutablelisttoptabbar = mutableListOf<String>("First","Second")

CustomVariableName.setListTabBar(mutablelisttoptabbar)

```

# Set Listener Update Flat Tab Bar

```

CustomVariableName.setOnUpdaterListener(object: BubleTabBar.OnSelectedItem{
    override fun OnTapped(index: Int) {
               val index_Tapped = index
    }
})

```

# Set TypeFace ( Font )

For setting custom typeface , first create typeface and second set to function.

Create Directory Name ( Font ) under 'res' directory and put custom font into /res/font/customfontname.ttf

```

val typeface = ResourcesCompat.getFont(this.context,R.font.customfontname)
CustomVariableName.setTypeFace(typeface)

```

# Functions

# Gets

| Functions Name | Function Description |
| :-------------: | :------------------: |
| getRadiusAll | Get Radius all ( top left , top right , bottom right , bottom left ) corners |
| getRadiusTopRight | Get Radius of Top Right Corener |
| getRadiusTopLeft | Get Radius of Top Left Corener |
| getRadiusBottomRight | Get Radius of Bottom Right Corener |
| getRadiusBottomLeft | Get Radius of Bottom Left Corener |
| getTypeFace | Get Type Face of Title Text for added font |
| getLayoutWidth | Get Width of Layout |
| getLayoutHeight | Get Height of Layout |
| getBoxShadowColor | Get Shadow of Layout Color |
| getBoxShadowSize | Get Shadow of Layout Size |
| getBoxShadowSizeX | Get Shadow of Layout Size in DX |
| getBoxShadowSizeY | Get Shadow of Layout Size in DY |
| getTitleSize | Get Size of Title Text |
| getBackgroundColor | Get Background Color of Pre Tapped On Item |
| getBackgroundTapped |  Get Background Color of After Tapped On Item |
| getColorTitleTapped | Get Color of Title on Tapped |

# Sets

| Functions Name | Function Description |
| :-------------: | :------------------: |
| setRadiusAll | Set Radius all ( top left , top right , bottom right , bottom left ) corners |
| setRadiusTopRight | Set Radius of Top Right Corener |
| setRadiusTopLeft | Set Radius of Top Left Corener |
| setRadiusBottomRight | Set Radius of Bottom Right Corener |
| setRadiusBottomLeft | Set Radius of Bottom Left Corener |
| setTypeFace | Set Type Face of Title Text for added font |
| setLayoutWidth | Set Width of Layout |
| setLayoutHeight | Set Height of Layout |
| setBoxShadowColor | Set Shadow of Layout Color |
| setBoxShadowSize | Set Shadow of Layout Size |
| setBoxShadowSizeX | Set Shadow of Layout Size in DX |
| setBoxShadowSizeY | Set Shadow of Layout Size in DY |
| setTitleSize | Set Size of Title Text |
| setBackgroundColor | Set Background Color of Pre Tapped On Item |
| setBackgroundTapped |  Set Background Color of After Tapped On Item |
| setColorTitleTapped | Set Color of Title on Tapped |

# Contact Us

Website : [nardana](http://nardana.ir/)

Email : nardanacorp@gmail.com

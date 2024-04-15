# Rapport
Det första steget var, likt tidigare, att skapa en fork av projektet på LenaSYS Github. Först ut var att lägga till en ny layout och widget. Jag valde att börja med en vertikal _LinearLayout_ tillsammans med några horisontella linjer och en _RatingBar_. Dessa fick därefter några mindre ändringar i storlek, position och rotation genom att ändra i **activity_main.xml**. Senare uppdaterades antalet stjärnor också.

**activity_main.xml**
```
<RatingBar
            android:id="@+id/ratingBar"
            android:layout_width="match_parent"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_gravity="center"
            android:numStars="5"
            android:rotationX="30"
            android:scaleX="0.8"
            android:translationY="20dp" />
```

Härnäst var det en kalender som även fick lite annorlunda rotation och placering. 
**activity_main.xml**
```
<CalendarView
            android:id="@+id/calendarView2"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:rotationX="-5"
            android:translationY="30dp"
            android:visibility="visible"
            tools:visibility="visible" />
```

Slutligen lades en ny sektion till med en horisontell _LinearLayout_ som innehåller en _TextCView_ och en knapp som inte gör någonting. 
**activity_main.xml**
```
<TextView
            android:id="@+id/textView"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:gravity="center"
            android:text="Hello there!"
            android:textStyle="bold"
            android:translationY="10dp" />

<Button
            android:id="@+id/button3"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:scaleX="0.8"
            android:scaleY="0.8"
            android:text="Click me!"
            android:translationY="10dp" />
```

Därefter updaterades några marginaler samt positioner på objekten.

Ett skärmklipp från den färdiga applikationen:

![Screenshot_20240415_061311](https://github.com/a20gabpa/mobileapp-programming-widgets/assets/102604680/ef3522e9-2fa6-42a2-bb0b-1462217fdd69)

Practical No : 01

Practical Name : Create an Android application for printing ‘Hello World’.

activity_main.xml:-

<?xml version="1.0" encoding="utf-8"?>

<androidx.constraintlayout.widget.ConstraintLayoutxmlns:android="http://schemas.androi d.com/apk/res/android"

xmlns:app="http://schemas.android.com/apk/res-auto" xmlns:tools="http://schemas.android.com/tools" android:id="@+id/font" android:layout_width="match_parent" android:layout_height="match_parent" tools:context=".MainActivity">



<TextView android:id="@+id/textView3" android:layout_width="358dp" android:layout_height="92dp" android:text="Hello World!"

android:textAppearance="@style/TextAppearance.AppCompat.Body2" android:textColor="#E91E63"

android:textSize="60sp" android:textStyle="bold|italic" app:layout_constraintBottom_toBottomOf="parent" app:layout_constraintEnd_toEndOf="parent" app:layout_constraintHorizontal_bias="1.0" app:layout_constraintStart_toStartOf="parent" app:layout_constraintTop_toTopOf="parent" app:layout_constraintVertical_bias="0.387" />



<TextView android:id="@+id/textView2" android:layout_width="356dp" android:layout_height="104dp" android:layout_marginBottom="16dp" android:layout_marginEnd="96dp" android:layout_marginStart="16dp" android:layout_marginTop="16dp" android:text="Lokesh Chavan" android:textColor="#673AB7" android:textSize="50sp" android:textStyle="bold|italic"

app:layout_constraintBottom_toBottomOf="parent" app:layout_constraintEnd_toEndOf="parent" app:layout_constraintHorizontal_bias="0.0" app:layout_constraintStart_toStartOf="parent" app:layout_constraintTop_toTopOf="parent"

 

app:layout_constraintVertical_bias="0.0" />

</androidx.constraintlayout.widget.ConstraintLayout>



MainActivity.java:-

package com.imr.helloworld;



import androidx.appcompat.app.AppCompatActivity; import android.os.Bundle;

public class MainActivityextends AppCompatActivity{



@Override

protected void onCreate(Bundle savedInstanceState) { super.onCreate(savedInstanceState); setContentView(R.layout.activity_main);

}

}

 

Output :

 

 

Practical No : 02

Practical Name :Create an Android application for showing use of different resources.

 

MainActivity.java:-

package com.example.testtt;

import androidx.appcompat.app.AppCompatActivity; import android.os.Bundle;

import android.widget.TextView;



public class MainActivityextends AppCompatActivity{ TextViewt1,t2,t3;

@Override

protected void onCreate(Bundle savedInstanceState) { super.onCreate(savedInstanceState); setContentView(R.layout.activity_main); t1=(TextView) findViewById(R.id .textView); t2=(TextView) findViewById(R.id .textView2 ); t3=(TextView) findViewById(R.id .textView3 ); t1.setText("Jalgaon");

t2.setText("IMCA");

t3.setText("IMR");

}

}

activity_main.xml:-

<?xml version="1.0" encoding="utf-8"?>

<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android" xmlns:app="http://schemas.android.com/apk/res-auto" xmlns:tools="http://schemas.android.com/tools" android:layout_width="match_parent" android:layout_height="match_parent"

tools:context=".MainActivity">

<TextView android:id="@+id/textView" android:layout_width="wrap_content" android:layout_height="wrap_content" android:layout_weight="1" android:text="TextView"

android:background="@color/Lokesh" />

<TextView android:id="@+id/textView3" android:layout_width="wrap_content" android:layout_height="wrap_content" android:layout_weight="1" android:text="TextView" />

<TextView android:id="@+id/textView2" android:layout_width="wrap_content"

 

android:layout_height="296dp" android:layout_weight="1" android:text="@string/Lokesh" />

<ImageView android:id="@+id/imageView" android:layout_width="263dp" android:layout_height="315dp" android:layout_weight="1" app:srcCompat="@drawable/tp" />

</LinearLayout>

 



Output:-



 

Practical No : 03

Practical Name : . Create an Android application for showing use UI Layouts.

 

MainActivity.java

package com.example.rlayout;

import androidx.appcompat.app.AppCompatActivity; import android.os.Bundle;

public class MainActivity extends AppCompatActivity {



@Override

protected void onCreate(Bundle savedInstanceState) { super.onCreate(savedInstanceState);

setContentView(R.layout.activity_main);

}

}

activity_main.xml:-

<?xml version="1.0" encoding="utf-8"?>

<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android" xmlns:app="http://schemas.android.com/apk/res-auto" xmlns:tools="http://schemas.android.com/tools" android:layout_width="match_parent" android:layout_height="match_parent" tools:context=".MainActivity">

<LinearLayout android:layout_width="409dp" android:layout_height="729dp" android:orientation="horizontal"

app:layout_constraintBottom_toBottomOf="parent" app:layout_constraintEnd_toEndOf="parent" app:layout_constraintStart_toStartOf="parent" app:layout_constraintTop_toTopOf="parent">

<EditText android:id="@+id/editTextTextPersonName2" android:layout_width="131dp" android:layout_height="177dp" android:layout_weight="1"

android:ems="10" android:inputType="textPersonName" android:text="Name" />

<Button android:id="@+id/button2"

android:layout_width="wrap_content" android:layout_height="172dp" android:layout_weight="1"

 

android:text="Button" />



<Button android:id="@+id/button3"

android:layout_width="wrap_content" android:layout_height="171dp" android:layout_weight="1" android:text="Button" />

</LinearLayout>

</androidx.constraintlayout.widget.ConstraintLayout>

themes.xml:-

<resources xmlns:tools="http://schemas.android.com/tools">

<!-- Base application theme. -->

<style name="Theme.Rlayout" parent="Theme.MaterialComponents.DayNight.DarkActionBar">

<!-- Primary brand color. -->

<item name="colorPrimary">@color/purple_500</item>

<item name="colorPrimaryVariant">@color/purple_700</item>

<item name="colorOnPrimary">@color/white</item>

<!-- Secondary brand color. -->

<item name="colorSecondary">@color/teal_200</item>

<item name="colorSecondaryVariant">@color/teal_700</item>

<item name="colorOnSecondary">@color/black</item>

<!-- Status bar color. -->

<item name="android:statusBarColor">?attr/colorPrimaryVariant</item>

<!-- Customize your theme here. -->

</style>

</resources>

 

Design :

 

 

Practical No : 04

Practical Name :Create an Android application for event handling.



activity_main.xml :

<?xml version="1.0" encoding="utf-8"?>

<androidx.constraintlayout.widget.ConstraintLayoutxmlns:android="http://schemas.androi d.com/apk/res/android"

xmlns:app="http://schemas.android.com/apk/res-auto" xmlns:tools="http://schemas.android.com/tools" android:layout_width="match_parent" android:layout_height="match_parent" tools:context=".MainActivity">



<TextView android:id="@+id/textView2" android:layout_width="wrap_content" android:layout_height="wrap_content" android:layout_marginBottom="396dp" android:text="Hello World!"

app:layout_constraintBottom_toBottomOf="parent" app:layout_constraintEnd_toEndOf="parent" app:layout_constraintHorizontal_bias="0.473" app:layout_constraintStart_toStartOf="parent" />



<Button android:id="@+id/button"

android:layout_width="wrap_content" android:layout_height="wrap_content" android:text="click" app:layout_constraintBottom_toBottomOf="parent" app:layout_constraintEnd_toEndOf="parent" app:layout_constraintHorizontal_bias="0.455" app:layout_constraintStart_toStartOf="parent" app:layout_constraintTop_toBottomOf="@+id/textView2" app:layout_constraintVertical_bias="0.212" />



</androidx.constraintlayout.widget.ConstraintLayout>



MainActivity.java:-

package com.example.eventhandling;



import androidx.appcompat.app.AppCompatActivity;

 

import android.os.Bundle; import android.view.View; import android.widget.Button; import android.widget.TextView;



public class MainActivity extends AppCompatActivity { Button btn;

TextViewtview;



@Override

protected void onCreate(Bundle savedInstanceState) { super.onCreate(savedInstanceState); setContentView(R.layout.activity_main);

btn=(Button) findViewById(R. id.button); tview=findViewById(R.id.textView2 ); btn.setOnClickListener(new View.OnClickListener() {

@Override

public void onClick(View view) { tview.setText("You Have clicked");

}

}) ;

}

}

 

Output :





 

Practical No : 05

Practical Name : Create an Android application for showing use of style and theme.

 

MainActivity.java:-

package com.example.testtt;

import androidx.appcompat.app.AppCompatActivity; import android.os.Bundle;

import android.widget.TextView;



public class MainActivityextends AppCompatActivity{ TextViewt1,t2,t3;

@Override

protected void onCreate(Bundle savedInstanceState) { super.onCreate(savedInstanceState); setContentView(R.layout.activity_main); t1=(TextView) findViewById(R.id .textView); t2=(TextView) findViewById(R.id .textView2 ); t3=(TextView) findViewById(R.id .textView3 ); t1.setText("Jalgaon");

t2.setText("IMCA");

t3.setText("IMR");



}

}

activity_main.xml:-

<?xml version="1.0" encoding="utf-8"?>

<LinearLayoutxmlns:android="http://schemas.android.com/apk/res/android" xmlns:app="http://schemas.android.com/apk/res-auto" xmlns:tools="http://schemas.android.com/tools" android:layout_width="match_parent" android:layout_height="match_parent"

tools:context=".MainActivity">

<TextView android:id="@+id/textView" android:layout_width="wrap_content" android:layout_height="wrap_content" android:layout_weight="1" android:text="TextView"

android:background="@color/Lokesh" />

<TextView android:id="@+id/textView3" android:layout_width="wrap_content" android:layout_height="wrap_content" android:layout_weight="1"

 

android:text="TextView" />

<TextView android:id="@+id/textView2" android:layout_width="wrap_content" android:layout_height="296dp" android:layout_weight="1" android:text="@string/Lokesh" />

<ImageView android:id="@+id/imageView" android:layout_width="263dp" android:layout_height="315dp" android:layout_weight="1" app:srcCompat="@drawable/tp" />

</LinearLayout>

Colors.xml:-

<?xml version="1.0" encoding="utf-8"?>

<resources>

<colorname="purple_200">#FFBB86FC</color>

<colorname="purple_500">#FF6200EE</color>

<colorname="purple_700">#FF3700B3</color>

<colorname="teal_200">#FF03DAC5</color>

<colorname="teal_700">#FF018786</color>

<colorname="black">#FF9800</color>

<colorname="white">#FFFFFFFF</color>

<colorname="Lokesh">#8BC34A</color>

</resources>

strings.xml:-

<resources>

<string name="app_name">testtt</string>

<string name="Lokesh">Android Programming</string>

</resources>

themes.xml:-

<resources xmlns:tools="http://schemas.android.com/tools">

<!-- Base application theme. -->

<style name="Theme.Testtt" parent="Theme.MaterialComponents.DayNight.DarkActionBar">

<!-- Primary brand color. -->

<item name="colorPrimary">@color/Lokesh</item>

<item name="colorPrimaryVariant">@color/purple_700</item>

<item name="colorOnPrimary">@color/white</item>

<!-- Secondary brand color. -->

<item name="colorSecondary">@color/teal_200</item>

<item name="colorSecondaryVariant">@color/teal_700</item>

<item name="colorOnSecondary">@color/black</item>

<!-- Status bar color. -->

<item name="android:statusBarColor">?attr/colorPrimaryVariant</item>

<!-- Customize your theme here. -->

 

</style>

</resources>

 



Design :

 



Final Output :

 

Practical No : 06

Practical Name :Create an Android application for showing use of notification.

activity_main.xml:-

<?xml version="1.0" encoding="utf-8"?>

<androidx.constraintlayout.widget.ConstraintLayoutxmlns:android="http://schemas.androi d.com/apk/res/android"

xmlns:app="http://schemas.android.com/apk/res-auto" xmlns:tools="http://schemas.android.com/tools" android:layout_width="match_parent" android:layout_height="match_parent" tools:context=".MainActivity">

<TextView android:id="@+id/textView" android:layout_width="wrap_content" android:layout_height="wrap_content" android:text="Hello World!"

app:layout_constraintBottom_toBottomOf="parent" app:layout_constraintEnd_toEndOf="parent" app:layout_constraintStart_toStartOf="parent" app:layout_constraintTop_toTopOf="parent" />

<Button android:id="@+id/button3"

android:layout_width="wrap_content" android:layout_height="wrap_content" android:text="Button" app:layout_constraintBottom_toBottomOf="parent" app:layout_constraintEnd_toEndOf="parent" app:layout_constraintStart_toStartOf="parent" app:layout_constraintTop_toTopOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>

MainActivity.java:-

package com.example.notification;



import android.os.Bundle; import android.view.View; import android.widget.Button;

import androidx.appcompat.app.AppCompatActivity; import androidx.core.app.NotificationCompat;

import androidx.core.app.NotificationManagerCompat; public class MainActivityextends AppCompatActivity{ Button button;

@Override

protected void onCreate(Bundle savedInstanceState) { super.onCreate(savedInstanceState);

 

setContentView(R.layout.activity_main); button = findViewById(R.id.button3 );

button.setOnClickListener(new View.OnClickListener() { @Override

public void onClick(View view) {

NotificationCompat.Builder builder=new NotificationCompat.Builder(MainActivity.this ) ; builder.setContentTitle("Notification Example");

builder.setContentText("This is simple notification "); builder.setSmallIcon(R.drawable.ic_launcher_background); builder.setAutoCancel(true); NotificationManagerCompatmanagerCompat= NotificationManagerCompat.from(MainActivity.this); managerCompat.notify( 1,builder.build());



}

});



}

}

 

Output :

 

 

Practical No : 07

Practical Name : Create an Android application for Sending Email.

activity_main.xml:-

<?xml version="1.0" encoding="utf-8"?>

<androidx.constraintlayout.widget.ConstraintLayoutxmlns:android="http://schemas.androi d.com/apk/res/android"

xmlns:app="http://schemas.android.com/apk/res-auto" xmlns:tools="http://schemas.android.com/tools" android:layout_width="match_parent" android:layout_height="match_parent" tools:context=".MainActivity">

<EditText android:id="@+id/editText1" android:layout_width="wrap_content"

android:layout_height="wrap_content" android:ems="10" android:inputType="textPersonName" android:hint="To" app:layout_constraintBottom_toBottomOf="parent" app:layout_constraintEnd_toEndOf="parent" app:layout_constraintHorizontal_bias="0.497" app:layout_constraintStart_toStartOf="parent" app:layout_constraintTop_toTopOf="parent" app:layout_constraintVertical_bias="0.096" />

<EditText android:id="@+id/editText2" android:layout_width="wrap_content"

android:layout_height="wrap_content" android:ems="10" android:inputType="textPersonName" android:hint="Subject" app:layout_constraintBottom_toBottomOf="parent" app:layout_constraintEnd_toEndOf="parent" app:layout_constraintHorizontal_bias="0.497" app:layout_constraintStart_toStartOf="parent" app:layout_constraintTop_toTopOf="parent" app:layout_constraintVertical_bias="0.211" />

<EditText android:id="@+id/editText3" android:layout_width="wrap_content"

android:layout_height="wrap_content" android:ems="10" android:inputType="textPersonName" android:hint="Message" app:layout_constraintBottom_toBottomOf="parent"

 

app:layout_constraintEnd_toEndOf="parent" app:layout_constraintHorizontal_bias="0.497" app:layout_constraintStart_toStartOf="parent" app:layout_constraintTop_toTopOf="parent" app:layout_constraintVertical_bias="0.325" />

<Button android:id="@+id/button"

android:layout_width="wrap_content" android:layout_height="wrap_content" android:text="Send" app:layout_constraintBottom_toBottomOf="parent" app:layout_constraintEnd_toEndOf="parent" app:layout_constraintStart_toStartOf="parent" app:layout_constraintTop_toTopOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>

MainActivity.java:-

package com.example.email3;



import androidx.appcompat.app.AppCompatActivity; import android.content. Intent;

import android.os.Bundle; import android.view.View; import android.widget.Button; import android.widget.EditText;



public class MainActivityextends AppCompatActivity{ private EditTexteTo;

private EditTexteSubject; private EditTexteMsg; private Button btn;



@Override

protected void onCreate(Bundle savedInstanceState) { super.onCreate(savedInstanceState); setContentView(R.layout.activity_main);

eTo= (EditText)findViewById(R.id.editText1 ) ; eSubject= (EditText)findViewById(R.id.editText2 ) ; eMsg= (EditText)findViewById(R.id.editText3 ) ; btn= (Button)findViewById(R.id.button) ; btn.setOnClickListener(new View.OnClickListener() { @Override

public void onClick(View v) {

Intent it = new Intent(Intent.ACTION_SEND) ; it.putExtra(Intent.EXTRA_EMAIL, new String[]{eTo.getText().toString()}); it.putExtra( Intent. EXTRA_SUBJECT,eSubject.getText().toString()); it.putExtra( Intent. EXTRA_TEXT,eMsg.getText()); it.setType("message/rfc822");

 

startActivity(Intent.createChooser(it,"Choose Mail App"));

}

});

}

}

 

Output : Design

 

Final Output :

 

 

Practical No : 08

Practical Name :Create an Android application for sending SMS.

activity_main.xml:-

<?xml version="1.0" encoding="utf-8"?>

<LinearLayoutxmlns:android="http://schemas.android.com/apk/res/android" android:orientation="vertical" android:layout_width="match_parent" android:layout_height="match_parent">

<TextView android:id="@+id/fstTxt"

android:layout_width="wrap_content" android:layout_height="wrap_content" android:layout_marginLeft="100dp" android:layout_marginTop="150dp" android:text="Mobile No" />

<EditText android:id="@+id/mblTxt"

android:layout_width="wrap_content" android:layout_height="wrap_content" android:layout_marginLeft="100dp" android:ems="10"/>



<TextView android:id="@+id/secTxt"

android:layout_width="wrap_content" android:layout_height="wrap_content" android:text="Message" android:layout_marginLeft="100dp" />

<EditText android:id="@+id/msgTxt"

android:layout_width="wrap_content" android:layout_height="wrap_content" android:layout_marginLeft="100dp" android:ems="10" />



<Button android:id="@+id/btnSend"

android:layout_width="wrap_content" android:layout_height="wrap_content" android:layout_marginLeft="100dp" android:text="Send SMS" android:onClick="sendsms" />

</LinearLayout> MainActivity.java:- package com.example.sms;



import androidx.appcompat.app.AppCompatActivity;

 

import android.Manifest;

import android.content.pm.PackageManager; import android.os.Build;

import android.os.Bundle;

import android.telephony.SmsManager; import android.view.View;

import android.widget.Button; import android.widget.EditText; import android.widget.Toast;



public class MainActivityextends AppCompatActivity{ EditTextphonenumber, message;

Button send;



@Override

protected void onCreate(Bundle savedInstanceState) { super.onCreate(savedInstanceState); setContentView(R.layout.activity_main);

send = findViewById(R.id.btnSend); phonenumber= findViewById(R.id.mblTxt); message = findViewById(R.id.msgTxt);

send.setOnClickListener(new View.OnClickListener() {



public void onClick(View v) {

if (Build.VERSION.SDK_INT>= Build.VERSION_CODES.M) {

if (checkSelfPermission(Manifest.permission.SEND_SMS) == PackageManager.PERMISSION_GRANTED) {

sendsms();

} else {

requestPermissions(new String[]{Manifest.permission.SEND_SMS},1);



}



}

}

});

}

private void sendsms() {

String number = phonenumber.getText().toString().trim(); String msg= message.getText().toString().trim();

try {

SmsManagersmsManager= SmsManager.getDefault(); smsManager.sendTextMessage(number, null, msg, null, null); Toast.makeText(getApplicationContext(), "Message Sent", Toast.LENGTH_LONG).show();

} catch (Exception e) { e.printStackTrace();

 

Toast.makeText(getApplicationContext(), "Some fiedls is Empty", Toast.LENGTH_LONG).show();

}

}

}

AndroidMainfest.xml:-

<?xml version="1.0" encoding="utf-8"?>

<manifest xmlns:android="http://schemas.android.com/apk/res/android">

<uses-permission android:name="android.permission.SEND_SMS"/>

<application android:allowBackup="true" android

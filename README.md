Nama : Hilmy syaddad Ramzy Nurfauzan

NiM : 312210162

Kelas : TI22A1

Dosen Pengampu : Donny Maulana, S.kom, M.M.S.I

===============================================================================


Pengertian Fibonacci


Fibonacci adalah suatu barisan bilangan yang merupakan hasil penjumlahan dua bilangan sebelumnya.


Bilangan Fibonacci diperkenalkan pertama kali oleh Leonardo da Pisa atau yang lebih dikenal dengan Fibonacci pada abad ke 13.

Bilangan Fibonacci
Pada bagian sebelumnya telah dikemukakan bahwa bilangan Fibonacci merupakan penjumlahan dua bilangan sebelumnya.

Dua bilangan Fibonacci pertama yaitu bilangan 0 dan 1. Sehingga suku-suku berikutnya dari barisan bilangan Fibonacci yaitu sebagai berikut.

Bilangan pertama: 0

Bilangan kedua: 1

Bilangan ketiga: 0 + 1 = 1

Bilangan keempat: 1 + 1 = 2

Bilangan kelima: 1 + 2 = 3

Bilangan keenam: 2 + 3 = 5

Bilangan ketujuh: 3 + 5 = 8


Bilangan kedelapan: 5 + 8 = 13

dan seterusnya sehingga bilangan selanjutnya merupakan penjumlahan dari dua bilangan sebelumnya.

Selain itu, konsep Fibonacci juga digunakan digunakan untuk barisan bilangan yang lainnya. Perhatikan contoh di bawah ini.

4, 5, 9, 14, 23, . . .

Pada barisan di atas, suku pertama: 4 dan suku kedua: 5.

Suku ketiga: 4 + 5 = 9,

Suku keempat: 5 + 9 = 14,

Suku kelima: 9 + 14 = 23,

dan seterusnya.


Deret Fibonacci

Deret Fibonacci didefinisikan secara rekursif (berulang). Misalkan dalam beberapa pola barisan bilangan dengan dua suku pertama  F1 = 0 dan F2 = 1.

Suku selanjutnya dirumuskan secara rekursif sebagai berikut.

Fn + 1 = Fn – 1  + Fn

Berikut ini akan dijelaskan mengenai rumus Fibonacci.

Rumus Fibonacci
Untuk menentukan suku ke-n bilangan Fibonacci dapat dengan menggunakan rumus berikut ini.

fn = 1/√5 x ((1 + √5)/2)n – 1/√5 x ((1 – √5)/2)n


============================================================================================

Soalnya adalah dari project sebelumnya Toast number dan Buatlah Method Program java Toast Number, dengan menghasilkan Bilangan Fibonacci


Fibonacci Sequence (Deret angka Fibonacci) adalah deret angka yang diperoleh dengan menjumlahkan dua angka didepannya / sebelumnya:


1, 1, 2, ...

1 + 2 = 3 ( 1, 1, 2, 3, ... )

2 + 3 = 5 ( 1, 1, 2, 3, 5, ... )

3 + 5 = 8 ( 1, 1, 2, 3, 5, 8, ... )



Begitu seterusnya, dikerjakan pada lembar jawaban kertas atau di laptop masing-masing


Kemudian hasilnya diupload di ecampus, atau dikumpulkan lembar jawabannya

![Screenshot (270)](https://github.com/Hilmyramzy/lab6_mobile/assets/115677769/087f7c09-096c-42d3-bc45-8ce35cf5f913)
![Screenshot (271)](https://github.com/Hilmyramzy/lab6_mobile/assets/115677769/fe37f561-5080-482e-b591-1465f861dff2)
![Screenshot (272)](https://github.com/Hilmyramzy/lab6_mobile/assets/115677769/5f3ade31-c285-4bc0-9c19-5a0518ef480b)
![Screenshot (273)](https://github.com/Hilmyramzy/lab6_mobile/assets/115677769/0cee7ef1-17c6-4d57-a719-503792b9ff68)
![Screenshot (274)](https://github.com/Hilmyramzy/lab6_mobile/assets/115677769/3c36eb88-2774-4e6f-bd3d-4be88c19c904)
![Screenshot (275)](https://github.com/Hilmyramzy/lab6_mobile/assets/115677769/bfcb4c53-ff56-40aa-825e-d5a934f1cfd6)
![Screenshot (276)](https://github.com/Hilmyramzy/lab6_mobile/assets/115677769/09240f30-2bec-4c82-a4e7-e02dc160906b)
![Screenshot (277)](https://github.com/Hilmyramzy/lab6_mobile/assets/115677769/b95ea0bf-a19c-4982-8322-efd042667d8f)
![Screenshot (278)](https://github.com/Hilmyramzy/lab6_mobile/assets/115677769/b768869d-d234-4a3b-ae79-8a783a8e4d2e)
![Screenshot (280)](https://github.com/Hilmyramzy/lab6_mobile/assets/115677769/eeea122e-1ad8-40cf-a511-5fea5be8d7bd)


CODE :
#Actifity Main
==========================================
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <Button
        android:id="@+id/button_toast"
        android:layout_width="390dp"
        android:layout_height="49dp"
        android:layout_marginStart="4dp"
        android:layout_marginTop="4dp"
        android:background="@color/colorPrimary"
        android:onClick="setLimit"
        android:text="@string/button_label_toast"
        android:textColor="@android:color/white"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <Button
        android:id="@+id/button_count"
        android:layout_width="190dp"
        android:layout_height="48dp"
        android:layout_marginStart="8dp"
        android:layout_marginEnd="8dp"
        android:layout_marginBottom="8dp"
        android:background="@color/colorPrimary"
        android:onClick="countUp"
        android:text="@string/button_label_count"
        android:textColor="@android:color/white"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.0"
        app:layout_constraintStart_toStartOf="parent"
        tools:ignore="UsingOnClickInXml,VisualLintButtonSize" />

    <Button
        android:id="@+id/button_finish"
        android:layout_width="190dp"
        android:layout_height="48dp"
        android:layout_marginStart="8dp"
        android:layout_marginEnd="8dp"
        android:layout_marginBottom="8dp"
        android:background="@color/colorPrimary"
        android:onClick="back1"
        android:text="@string/button_label_finish"
        android:textColor="@android:color/white"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="1.0"
        app:layout_constraintStart_toStartOf="parent"
        tools:ignore="UsingOnClickInXml" />

    <TextView
        android:id="@+id/show_count"
        android:layout_width="0dp"
        android:layout_height="0dp"
        android:layout_marginStart="8dp"
        android:layout_marginTop="8dp"
        android:layout_marginEnd="8dp"
        android:layout_marginBottom="8dp"
        android:background="#80FF00"
        android:gravity="center_vertical"
        android:text="@string/count_initial_value"
        android:textAlignment="center"
        android:textColor="@color/colorPrimaryDark"
        android:textSize="160sp"
        android:textStyle="bold"
        app:layout_constraintBottom_toTopOf="@id/button_count"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@id/button_toast"
        tools:ignore="RtlCompat" />

</androidx.constraintlayout.widget.ConstraintLayout>

=========================================================
#MainActifityJava

package com.example.fibanocci;


import android.app.AlertDialog;
import android.content.DialogInterface;
import android.graphics.Color;
import android.os.Bundle;
import android.view.View;
import android.widget.EditText;
import android.widget.TextView;
import androidx.appcompat.app.AppCompatActivity;

public class MainActivity extends AppCompatActivity {
    private TextView showCount;
    private int count = 1;
    private long fibNMinus1 = 1;
    private long fibNMinus2 = 1;
    private int limit = -1; // Inisialisasi limit dengan nilai default

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        showCount = findViewById(R.id.show_count);
    }

    public void countUp(View view) {
        if (count == 0) {
            showCount.setText("0");
        } else if (count == 1) {
            showCount.setText("1");
        } else {
            if (limit != -1 && count > limit) {
                // Jika count melebihi limit, atur ulang perhitungan
                count = 0;
                fibNMinus1 = 1;
                fibNMinus2 = 0;
                showCount.setText(getString(R.string.count_initial_value));
            } else {
                long fibCurrent = fibNMinus1 + fibNMinus2;
                fibNMinus2 = fibNMinus1;
                fibNMinus1 = fibCurrent;

                // Mengubah warna teks menjadi warna RGB dengan warna yang berbeda setiap kali angka berubah
                int red = (int) (Math.random() * 256);
                int green = (int) (Math.random() * 256);
                int blue = (int) (Math.random() * 256);
                showCount.setTextColor(Color.rgb(red, green, blue));

                showCount.setText(String.valueOf(fibCurrent));
            }
        }

        count++;
    }

    public void back1(View view) {
        count = 1;
        fibNMinus1 = 1;
        fibNMinus2 = 0;
        showCount.setText(getString(R.string.count_initial_value));
    }

    public void setLimit(View view) {
        // Create and display a dialog to set the limit
        AlertDialog.Builder builder = new AlertDialog.Builder(this);
        builder.setTitle("Set Limit");

        final EditText input = new EditText(this);
        input.setInputType(android.text.InputType.TYPE_CLASS_NUMBER);
        builder.setView(input);

        builder.setPositiveButton("OK", new DialogInterface.OnClickListener() {
            @Override
            public void onClick(DialogInterface dialog, int which) {
                // Get the limit from the input and set it for calculations
                String limitStr = input.getText().toString();
                limit = Integer.parseInt(limitStr);
            }
        });

        builder.setNegativeButton("Cancel", new DialogInterface.OnClickListener() {
            @Override
            public void onClick(DialogInterface dialog, int which) {
                dialog.cancel();
            }
        });


        builder.show();
    }
}
=====================
#COLOR 

<?xml version="1.0" encoding="utf-8"?>
<resources>
    <color name="colorPrimary">#3F51B5</color>
    <color name="colorPrimaryDark">#2F3A78</color>
</resources>



=====================



#String


resources>
    <string name="app_name">fibanocci</string>
    <string name="Reset">Reset</string>
    <string name="button_label_finish">Toast</string>
    <string name="button_label_count">Count</string>
    <string name="toast_massage">Bilangan Fibonance</string>
    <string name="button_label_toast">angka limit Fibonacci?</string>
    <string name="count_initial_value">1</string>
</resources









================Hasil run=======================

![Gambar WhatsApp 2023-11-07 pukul 08 07 30_fe5eb96e](https://github.com/Hilmyramzy/lab6_mobile/assets/115677769/92c00873-da23-4972-bdcb-5feb4f79b7ad)


![Gambar WhatsApp 2023-11-07 pukul 07 36 11_d9df1d4e](https://github.com/Hilmyramzy/lab6_mobile/assets/115677769/66b4d665-8e1a-4dac-9547-f027bd02723c)

==========masukan limit===========
![Gambar WhatsApp 2023-11-07 pukul 07 43 42_ed238e07](https://github.com/Hilmyramzy/lab6_mobile/assets/115677769/515e9ada-38bf-4ef5-8399-0fc1768a5533)

























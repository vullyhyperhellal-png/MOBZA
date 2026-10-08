package com.example.accessoriesapp;

import android.app.Activity;
import android.os.Bundle;
import android.graphics.Color;
import android.view.Gravity;
import android.widget.*;

public class MainActivity extends Activity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);

        LinearLayout layout = new LinearLayout(this);
        layout.setOrientation(LinearLayout.VERTICAL);
        layout.setPadding(30, 50, 30, 30);
        layout.setBackgroundColor(Color.WHITE);

        TextView title = new TextView(this);
        title.setText("متجر إكسسوارات الهواتف");
        title.setTextSize(26);
        title.setTextColor(Color.rgb(20, 50, 120));
        title.setGravity(Gravity.CENTER);

        layout.addView(title);

        Button cases = new Button(this);
        cases.setText("📱 كوفرات الهواتف");
        layout.addView(cases);

        Button chargers = new Button(this);
        chargers.setText("🔌 شواحن");
        layout.addView(chargers);

        Button earphones = new Button(this);
        earphones.setText("🎧 سماعات");
        layout.addView(earphones);

        Button batteries = new Button(this);
        batteries.setText("🔋 بطاريات و Power Bank");
        layout.addView(batteries);

        Button screens = new Button(this);
        screens.setText("🛡️ شاشات و Vitres");
        layout.addView(screens);

        setContentView(layout);
    }
}

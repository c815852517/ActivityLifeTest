# 实验一——活动生命周期
This is the first Android test

## 实验目的
验证Activity的生命周期

## 实验重要代码
package com.example.myapplication;

import android.support.v7.app.AppCompatActivity;
import android.os.Bundle;
import android.util.Log;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_LinearLayout);
        Log.d("MainActivity","调用onCreate()");
    }
    @Override
    protected void onStart(){
        super.onStart();
        Log.d("MainActivity","调用onStart()");
    }
    @Override
    protected void onResume(){
        super.onResume();
        Log.d("MainActivity","调用onResume()");
    }

    @Override
    protected void onPause(){
        super.onPause();
        Log.d("MainActivity","调用onPause()");
    }

    @Override
    protected void onStop(){
        super.onStop();
        Log.d("MainActivity","调用onStop()");
    }

    @Override
    protected void onDestroy(){
        super.onDestroy();
        Log.d("MainActivity","调用onDestroy()");
    }
}

## 实验内容及步骤
### 一、启动Activity生命周期
![](https://github.com/c815852517/ActivityLifeTest/blob/master/myapplication/src/111.png)

### 二、返回前台（未关闭Activity）
![](https://github.com/c815852517/ActivityLifeTest/blob/master/myapplication/src/222.png)

### 三、返回Activity
![](https://github.com/c815852517/ActivityLifeTest/blob/master/myapplication/src/%7BB%24DJ%25NI_%25CWZM_UAA88%5DA7.png)

### 四、关闭Activity生命周期
![](https://github.com/c815852517/ActivityLifeTest/blob/master/myapplication/src/I%5B%5DG%5DZOY5K%7D%5B5%24%40HUMG%25OFW.png)

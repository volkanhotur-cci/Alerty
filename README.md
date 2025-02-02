# Alerty 

Alerty is a simple Alert Dialog Library for Android.

# Latest Release

The latest release is available on Jitpack with 1.0.0-alfa.

    repositories {
		maven { url 'https://jitpack.io' }
	}

    implementation 'com.github.volkanhotur-cci:Alerty:1.0.0-alfa'
    
This repo has a sample project. And you can see sample codes below:

```java
new Alerty.Builder(this)
                .setTitle("Test Title")
                .setMessage("Test Message Dialog")
                .setCancellable(false)
                .setPositiveButtonText("DONE")
                .setNegativeButtonText("CANCEL")
                .setHeaderImage(R.drawable.ic_message_red)
                .setPositiveButtonColor(0XFF0EC432)
                .setNegativeButtonColor(0XFF828282)
                .setButtonRadius(16f)
                .setDialogRadius(16f)
                .setTextAppearance(Alerty.MEDIUM_TEXT)
                .setTitleTextColor(0xFF000000)
                .setPositiveListener(new AlertyListener() {
                    @Override
                    public void onDialogClick(Dialog dialog) {
                        Toast.makeText(MainActivity.this, "DONE!", Toast.LENGTH_SHORT).show();
                    }
                })
                .build();
```

# Screenshot

![ScreenShot](https://github.com/volkanhotur-cci/Alerty/blob/master/Screenshot_1574755161.png)

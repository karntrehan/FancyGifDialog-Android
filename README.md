# FancyAlertDialog-Android
[![platform](https://img.shields.io/badge/platform-Android-yellow.svg)](https://www.android.com)
[![API](https://img.shields.io/badge/API-19%2B-brightgreen.svg?style=plastic)](https://android-arsenal.com/api?level=19)
[![License](https://img.shields.io/badge/license-Apache%202-4EB1BA.svg?style=flat-square)](https://www.apache.org/licenses/LICENSE-2.0.html)
[![](https://jitpack.io/v/Shashank02051997/FancyGifDialog-Android.svg)](https://jitpack.io/#Shashank02051997/FancyGifDialog-Android)
[![Android Arsenal](https://img.shields.io/badge/Android%20Arsenal-FancyGifDialog-brightgreen.svg?style=flat)](https://android-arsenal.com/details/1/6652)
## Prerequisites

Add this in your root `build.gradle` file (**not** your module `build.gradle` file):

```gradle
allprojects {
	repositories {
		...
		maven { url "https://jitpack.io" }
	}
}
```

## Dependency

Add this to your module's `build.gradle` file (make sure the version matches the JitPack badge above):

```gradle
dependencies {
	...
	compile 'com.github.Shashank02051997:FancyGifDialog-Android:1.1'
}
```
<h2> Fancy Gif Dialog</h2>

```java
new FancyGifDialog.Builder(this)
                    .setTitle(R.string.from_resources)
                    .setMessage(R.string.description_from_resources)
                    .setNegativeBtnText(android.R.string.cancel)
                    .setPositiveBtnBackground(R.color.positiveButton)
                    .setPositiveBtnText(android.R.string.ok)
                    .setNegativeBtnBackground(R.color.negativeButton)
                    .setGifResource(R.drawable.gif1)
                    .isCancellable(true)
                    .setOnCancelListener(new DialogInterface.OnCancelListener() {
                        @Override
                        public void onCancel(DialogInterface dialogInterface) {
                            toaster("Cancelled");
                        }
                    })
                    .OnPositiveClicked(new FancyGifDialogListener() {
                        @Override
                        public void OnClick() {
                            toaster("Ok");
                        }
                    })
                    .OnNegativeClicked(new FancyGifDialogListener() {
                        @Override
                        public void OnClick() {
                            toaster("Cancel");
                        }
                    })
                    .build();
```

## Screenshots

**Please click the image below to enlarge.**


<img src="https://github.com/Shashank02051997/FancyGifDialog-Android/blob/master/Screenshot/20180106_215855.gif" height="420" width="240" hspace="20"><img src="https://github.com/Shashank02051997/FancyGifDialog-Android/blob/master/Screenshot/20180106_220303.gif" height="420" width="240" hspace="20"><img src="https://github.com/Shashank02051997/FancyGifDialog-Android/blob/master/Screenshot/20180106_220829.gif" height="420" width="240">

<img src="https://github.com/Shashank02051997/FancyGifDialog-Android/blob/master/Screenshot/20180106_221054.gif" height="420" width="240" hspace="20"><img src="https://github.com/Shashank02051997/FancyGifDialog-Android/blob/master/Screenshot/20180106_221227.gif" height="420" width="240" hspace="20"><img src="https://github.com/Shashank02051997/FancyGifDialog-Android/blob/master/Screenshot/20180106_221357.gif" height="420" width="240">

<img src="https://github.com/Shashank02051997/FancyGifDialog-Android/blob/master/Screenshot/Screenshot_2018-01-07-10-24-37.png" height="420" width="240" hspace="20"><img src="https://github.com/Shashank02051997/FancyGifDialog-Android/blob/master/Screenshot/Screenshot_2018-01-07-10-25-07.png" height="420" width="240" hspace="20"><img src="https://github.com/Shashank02051997/FancyGifDialog-Android/blob/master/Screenshot/Screenshot_2018-01-07-10-25-26.png" height="420" width="240">

## Dependencies

This project use this libraries ~ Thanks to them.

  [android-gif-drawable](https://github.com/koral--/android-gif-drawable)
  
## Contributing

Please fork this repository and contribute back using
[pull requests](https://github.com/Shashank02051997/FancyGifDialog-Android/pulls).

Any contributions, large or small, major features, bug fixes, are welcomed and appreciated
but will be thoroughly reviewed .

### Contact - Let's become friend
- [Twitter](https://twitter.com/shashank020597)
- [Github](https://github.com/Shashank02051997)
- [Linkedin](https://www.linkedin.com/in/shashank-singhal-a87729b5/)
- [Facebook](https://www.facebook.com/shashanksinghal02)

## License

* [Apache Version 2.0](http://www.apache.org/licenses/LICENSE-2.0.html)

```
Copyright 2018 Shashank Singhal

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

 http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

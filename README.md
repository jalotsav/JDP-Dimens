## Introduction

You can use this library for reduce your design work. Using this library you need to create only one default layout file and it's support in most of different resolutions.

## How to Use?

Here is example for set Width and Height for ImageView
```
<ImageView
    android:layout_width="@dimen/_50jdp"
    android:layout_height="@dimen/_50jdp"
    android:contentDescription="Launcher image"
    android:src="@mipmap/ic_launcher" />
```

## How to Apply?

**Include AAR file to project**

- Download `jdpdimens-1.0.0.aar` AAR file from
<a href='http://jcenter.bintray.com/com/jalotsav/design/jdpdimens/1.0.0/jdpdimens-1.0.0.aar'><img src='https://api.bintray.com/packages/jalotsav/maven/jdpdimens/images/download.svg?version=1.0.0'></a>

- Add downloded AAR file under app(module)-->libs directory of your project.
- Add below code in to app/build.gradle
```
android {
  ...
}

repositories {
    flatDir {
        dirs 'libs'
    }
}

dependencies {
  ...
  compile(group: 'com.jalotsav.design', name: 'jdpdimens', version: '1.0.0', ext: 'aar', classifier: '')
}
```

**Add dependency in Gradle**
```
compile 'com.jalotsav.design:jdpdimens:1.0.0'
```

# Note
The jdp size calculation includes some approximation due to some performance and usability constraints.

### Inspired by [sdp](https://github.com/intuit/sdp)

## License
```
Copyright (c) 2017 Jalotsav

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
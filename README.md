
# AnimationRatingBar
Just like a Android RatingBar with 16 animations.  
And more features than Android RatingBar.  
You can use custom icon and set animation for it.  

<img src="https://github.com/WillysFish/AnimationRatingBar/blob/main/sample.gif" height="20%" width="20%" > <img src="https://github.com/WillysFish/AnimationRatingBar/blob/main/animation_damo.gif" height="20%" width="20%" >

# Download
### Gradle:  
Add it in your root build.gradle at the end of repositories:
```gradle
allprojects {
  repositories {
    ...
    maven { url 'https://jitpack.io' }
  }
}
```
Add the dependency
```gradle
dependencies {
	 implementation 'com.github.WillysFish:AnimationRatingBar:1.0.0'
}
```
### Maven:
Add the JitPack repository to your build file
```xml
<repositories>
  <repository>
      <id>jitpack.io</id>
      <url>https://jitpack.io</url>
  </repository>
</repositories>
```
Add the dependency
```xml
<dependency>
  <groupId>com.github.WillysFish</groupId>
  <artifactId>AnimationRatingBar</artifactId>
  <version>1.0.0</version>
</dependency>
```

# How to use? 
  - Attribute Introduction
	  - Setting the number of icon.
	  ```xml
	  <attr format="integer" name="numStars"/>
	  ``` 
	  
	  - Setting the score of AnimationRatingBar.  
	    __If your score is from api or other data, set it be zero.__
	  ```xml
	  <attr format="float" name="rating"/>
	  ```
	  
	  - IndicatorBar means not clickable.
	  ```xml
	  <attr format="boolean" name="isIndicatorBar"/>
	  ```
	  

	  - Setting icons which you like.  
	  __If you don't need the halfIcon, set icon which is same to emptyIcon or filledIcon.__
	  ```xml
	  <attr format="reference" name="emptyIcon"/>
	  <attr format="reference" name="filledIcon"/>
	  <attr format="reference" name="halfIcon"/>
	  ```
	  
	  - Adjusting spacing of icon.
	  ```xml
	  <attr format="dimension" name="iconSpacingEnd"/>
	  <attr format="dimension" name="iconSpacingStart"/>
	  <attr format="dimension" name="iconSpacingTop"/>
	  <attr format="dimension" name="iconSpacingBottom"/>
	  ```
	  
	  - Adjusted the speed of animation.  
	  0.5 => Half of original speed.  
	  3 => Original speed of 3 times.
	  ```xml
	  <attr format="float" name="iconAnimationSpeed"/>
	  ```
	  
	  - Selecting none animation or any animation which you like.
	  ```xml
	  <attr format="enum" name="iconAnimationMode">
	  ```

    - The animation list
    ```xml
    <enum name="none" value="0"/>  
    <enum name="rotation" value="1"/>  
    <enum name="rotationJumpUp" value="2"/>  
    <enum name="rotationDownUp" value="3"/>  
    <enum name="zoom" value="4"/>  
    <enum name="zoomJumpUp" value="5"/>  
    <enum name="zoomDownUp" value="6"/>  
    <enum name="shake" value="7"/>  
    <enum name="shakeJumpUp" value="8"/>  
    <enum name="shakeDownUp" value="9"/>  
    <enum name="shakeZoom" value="10"/>  
    <enum name="shakeZoomJumpUp" value="11"/>  
    <enum name="shakeZoomDownUp" value="12"/>  
    <enum name="turnRound" value="13"/>  
    <enum name="turnRoundJumpUp" value="14"/>  
    <enum name="turnRoundZoom" value="15"/>  
    <enum name="turnRoundZoomJumpUp" value="16"/>
    ```
&nbsp;

- Method Introduction
	- Programmatically set rating
	```kotlin
	fun setRating(score: Float) {}
	```
	- Getting current rating
	```kotlin
	fun getRating() {}
	```
		  

  

# License
```
Copyright 2020 zewei yan

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



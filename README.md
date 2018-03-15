# SwipeButton
A very simple Android Swipe Button

![SwipeButton](https://github.com/rrishabhj/SwipeButton/blob/master/ezgif.com-video-to-gif.gif)

## How to use

```
swipeButtonSettings
        .setButtonPressText(">> NEW TEXT! >>")
        .setGradientColor1(0xFF888888)
        .setGradientColor2(0xFF666666)
        .setGradientColor2Width(60)
        .setGradientColor3(0xFF333333)
        .setPostConfirmationColor(0xFF888888)
        .setActionConfirmDistanceFraction(0.7)
        .setActionConfirmText("Action Confirmed");

```
Adding callback listner
```
 if (mSwipeButton != null) {
      mSwipeButton.setSwipeButtonCustomItems(swipeButtonSettings);
    }
SwipeButtonCustomItems swipeButtonSettings = new SwipeButtonCustomItems() {
      @Override
      public void onSwipeConfirm() {
        Log.d("NEW_STUFF", "New swipe confirm callback");
      }
    };
```

In XML--

```
<com.rishabh.swipebutton.SwipeButton
      android:id="@+id/my_swipe_button"
      android:layout_width="400dp"
      android:layout_height="50dp"
      android:text="Button"
      android:background="#888888"
      android:textColor="#ffffff"
      />
```

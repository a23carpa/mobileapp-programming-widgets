
# Rapport
I detta arbete har jag innuti startlayouten ConstraintLayout lagt till yttigare layouts. En LinearLayout(Vertical) som innuti sig har 3 andra layouts, 2 linear layout (Horizontal) och en ConstraintLayout. I den första inre LinearLayouten skapas en ImageView som centrers i mitten, genom ```android:gravity="center"```.
I linearLayout nr 2 skapas det en knapp som läggs top/center genom ```android:gravity="top|center"```
I den inre ConstraintLayout skapas det en TextView och en EditText view. Dessa Constrainas och plaseras i mitten genom skystering av dp marain.
Dessa två är även constrainade till varandra bottom-top och top-bottom.
```
                app:layout_constraintBottom_toBottomOf="parent"
                app:layout_constraintEnd_toEndOf="parent"
                app:layout_constraintStart_toStartOf="parent"
                app:layout_constraintTop_toBottomOf="@id/text1" 
```
Koden ovan är ifrån viewn EditText som är en textfält som användaren kan skiva in egen text. I koden visas de constraints som den använder sig av. Att till höger, vänster och nedåt så constrainar den sig emot parent, vilket är skärmens storlek. Consteint uppåt sker genom att constraina EditTexts top emot viewn med id "text1" som ligger ovanför.


<img src="Screenshot.png" width="300" height="600"> 




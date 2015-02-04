# jquery-map-trifecta
Combines RWD Image Maps, Maphilight, and Zoom into 1 solution. Optional table integration.

---

## Usage:
Simply pass in the Image for the Responsive, Hilight, and Zoom features<br>
  <pre>• Double-click Image Map to Zoom<br>
• Hold down Ctrl key to select multiple</pre>

``` html
<link href="css/map-trifecta.css" rel="stylesheet" /> <!--Needed for Zoom and img-->
<script src="js/jquery.map-trifecta.min.js"></script>

<img src="images/shapes.png" usemap="#shapesMap">
<map name="shapesMap">
  <area coords="5,136,80,9" alt="Triangle" href="#" shape="poly" />
  <area coords="177,134,179..." alt="Square" href="#" shape="poly" />
  <area coords="358,123,353..." alt="Circle" href="#" shape="poly" />
</map>
```

```js
$("img[usemap]").mapTrifecta();
```

## With Table:
You can have a table (shown in index.html) respond with the Image Map Hilight.<br>
To do this just have the `<tr>` of the table and the `<area>` of the map include a **data-mapid** parameter.
Matching id's with Hilight.

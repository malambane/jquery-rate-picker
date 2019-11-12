# jquery-rate-picker
An easy to use rate picker built on top of jquery and font awesome.  

<h2> Example 1 [default]:</h2>

<p> <pre>No callback, data will posted as &lt;input type="hidden" name="rating-1" /&gt;</pre> </p>

<b>html:</b>
<p>
<code>
&lt;span id="rating-1" data-stars="3"&gt;&lt;/span&gt;
</code></p>

<b>javascript:</b>
<p>
<code>
$.ratePicker("#rating-1");
</code>
</p>

<h2> Example 2 [custom]: </h2>

<p> <pre>Callback function, colors, maximum starts and pointer given, <br/>
 data will still be posted as &lt;input type="hidden" name="rating-2" /&gt;</pre>
 </p>


<b>html:</b>
<p>
<code>
&lt;span id="rating-2" data-stars="6"&gt;&lt;/span&gt;
</code></p>

<b>javascript:</b>
<p>
<code>
 $.ratePicker("#rating-2", {
        max :10,
        rgbOn:"#e74c3c",
        rgbOff:"#ecf0f1",
        rgbSelection:"#e74c3c",
        cursor:"crosshair",
        rate : function (stars){
            alert('Sample 2 Rate is ' + stars);
        }
    });
</code>
</p>

<h2> Example 3 [custom]: </h2>

<p> <pre>Custom font awesome indicator</pre>
 </p>


<b>html:</b>
<p>
<code>
&lt;span id="rating-3" data-stars="3"&gt;&lt;/span&gt;
</code></p>

<b>javascript:</b>
<p>
<code>
  $.ratePicker("#rating-3", {
         max :5,
         rgbOn:"#2ecc71",
         rgbOff:"#bdc3c7",
         rgbSelection:"#2ecc71",
         indicator:"fa-thumbs-up"
     });
</code>
</p>


Click for <a href="http://helton.malambane.com/js/jquery-rate-picker" target="_blank">live demo</a>
<p>Helton MALAMBANE</p>



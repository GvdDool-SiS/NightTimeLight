ref: https://www.markdownguide.org/basic-syntax/

note: reorder the locations, from blast site (1) to Airport (6) - ports first, residential second.


<br><br>
<h1> Night-Time Light Investigation into the Beirut Explosion (2020-08-04) </h1>
 
Gijs van den Dool <sup id="a1">[1](#f1)</sup>
@ Space-ins.-Solutions <sup id="a2">[2](#f1)</sup>
 

 
<h2> Introduction </h2>
<p>

</p>
<br>

<h2> Area of Interest </h2>
<p>

</p>
<br>

![Map of the Area of Interest](Figures/F1_map1.png?raw=true "Title") <br>
Figure 1: Area of Intrest (Lebanon/Beirut)<br>
<br>

<h3> Local View </h3>
<p>Six locations are selected to test the change in NTL before and afer the explosion. The location position is randon, but the location type is prediterment. To compare the Blast Area (as a port location), two other port locations are selected, and the main intest of the study is to see if it is possible to detect recovery rates, so two residential areas are added to the selection, and finally the Airport is included in the test locations because of the presumed stability in NTL intensity.</p>
<br>

![Map of the Area of Interest](Figures/F2_zoom1.png?raw=true "Title") <br>
Figure 2: Six pilot locations (Greater Beirut Area)<br>
<br>


<h2>Data</h2>
<p>

</p>
<br>

<h2>Exploratory Data Analysis (EDA)</h2>
<p>

</p>
<br>

<h3> EDA 1 </h3>
<p>

</p>
<br>

![Map of the Area of Interest](Figures/F3_EDA1.png?raw=true "Title") <br>
Figure 3: XXXX<br>
<br>

<h3> EDA 2 </h3>
<p>

</p>
<br>

![Map of the Area of Interest](Figures/F3_EDA2.png?raw=true "Title") <br>
Figure 4: XXXX<br>
<br>

<h3> EDA 3 </h3>
<p>

</p>
<br>

![Map of the Area of Interest](Figures/F3_EDA3.png?raw=true "Title") <br>
Figure 5: XXXX<br>
<br>

<h3> EDA 4 </h3>
<p>

</p>
<br>

![Map of the Area of Interest](Figures/F3_EDA4.png?raw=true "Title") <br>
Figure 6: XXXX<br>
<br>

<h3> EDA 5 </h3>
<p>

</p>
<br>

![Map of the Area of Interest](Figures/F3_EDA5.png?raw=true "Title") <br>
Figure 7: XXXX<br>
<br>


<h2>Statistics</h2>
<p>

</p>
<br>

<h3> Method 1: T-Test </h3>
<p>

</p>
<br>

<h3> Method 2: Causual Impact  </h3>
<p>

</p>
<br>


Table 1: Causal Imapact Results; method adapted from CausalImpact <sup id="a5">[5](#f1)</sup>   
<table>
    <tr>
        <td>Event date: 2020-08-04</td>
        <td>Event date: 2020-06-20</td>
    </tr>
    <tr>
        <td valign="top"><img src="Figures/F4_CausalImpact1.png"></td>
        <td valign="top"><img src="Figures/F4_CausalImpact2.png"></td>
    </tr>
    <tr>
        <td valign="top"> The probability of obtaining this effect by chance is p = 21.78%.<br> <br>
        This means that, although the intervention appears to have caused a <strong>positive</strong> effect, the effect may be spurious and would generally not be considered statistically significant, when considering the entire post-intervention period as a whole. 
        </td> 
        <td valign="top"> The probability of obtaining this effect by chance is p = 9.59%. <br> <br>
        Although it may look as though the intervention has exerted a <strong>negative</strong> effect on the response variable when considering the intervention period as a whole, this effect may be spurious and would generally not be considered statistically significant.
        </td>
    </tr>
    <tr>
        <td> Method adapted from CausalImpact <sup id="a5">[5](#f1)</sup>                          
        </td>
    </tr>
</table>
<br>
<br>

<h2>Conclusion</h2>
<p>

</p>
<br>


---
<br>

<b id="f1">1</b> https://www.linkedin.com/in/gvddool/ [↩](#a1)<br>
<b id="f1">2</b> https://www.spaceinssolutions.com/ [↩](#a2)<br>

<h2>References</h2>
<p>

Example 3 <sup id="a3">[3](#f1)</sup><br>
Example 4 <sup id="a4">[4](#f1)</sup><br>

<b id="f1">3</b> https://www.linkedin.com/in/gvddool/ [↩](#a3)<br>
<b id="f1">4</b> https://www.spaceinssolutions.com/ [↩](#a4)<br>

<b id="f1">5</b> CausalImpact GitHub repro https://github.com/dafiti/ [↩](#a5)<br>

</p>



ref: https://www.markdownguide.org/basic-syntax/

note: reorder the locations, from blast site (1) to Airport (6) - ports first, residential second.


<br><br>
<h1> Night-Time Light Investigation into the Beirut Explosion (2020-08-04) </h1>
 
Gijs van den Dool <sup id="aa">[a](#f1)</sup>
@ Space-ins.-Solutions <sup id="ab">[b](#f1)</sup>
 

 
<h2> Motivation </h2>
<p> Night-Time Light satellite products often mentioned as an input parameter for sociological studies, for example, in this study from the Universities of Wageningen, Utrecht and Nanjing: “Detecting Inequality from Space.” (2021)[1], or “Spatially explicit global gross domestic product (GDP) data set consistent with the Shared Socioeconomic Pathways” by Wang and Sun (2021)[2], to give two examples out of many scientific publications, and from personal experience, I participated in two projects with Omdena, WRI, ACET and DSSG in which we used NTL to compute an index for either well-being or access to electricity [3, 4].
</p>
<br>
<p> My first encounter with NTL was, however, in a NASA-ARSET training: Introduction to NASA’s “Black Marble” Night Lights Data [5], and while going through the training exercise to Monitoring the Disaster Impacts in Puerto Rico – After the Jan-2020 6.4 Earthquakes, I thought that looking at the Beirut explosion, and exploring the possibility to detect the effect of the blast (at ground zero) and the potential recovery, would be a good self-test for after the training.</p>
<br>
<p> This article will follow the steps in the training exercise, and most of the data handling scripts are modified from the training material to fit this case study; the notebooks I used for the analysis are part of a GitHub repository, and I placed a link in the reference section. <sup id="ac">[c](#f1)</sup> [c]. 
</p>

1. Data acquisition: the linked ARSET training material has an excellent tutorial on getting the data; I will briefly describe the data, and the features, and refer to this tutorial for the practical steps.

2. Data transformation: again using the scripts from the ARSET training material, but now used to convert the native format of the data to GeoTiff, other file formats are possible too (like xarray), but GeoTiff raster files were easy to implement and flexible enough.
3. Exploratory Data Analysis (EDA): The purpose of the analysis is to see if it is possible to detect the explosion in the NTL data, therefor six locations are selected, and in this section, the differences between the locations are explored to determine if it is possible to detect a trend in NTL, not only at the Blast Site but also in the surrounding areas.
4. Statistical Analysis: EDA is a general term to visualise the data by summary statistics and graphical representations, and to look at data before making any assumptions, as well as to discover patterns, spot anomalies, and test hypothesis.
5. In the concluding section, I will highlight my observations and  provide an outlook on the possible next steps.

<p> Working through the excersise, applying it to a real-world problem, and seeing how the data changed during the EDA process, and the Statistical Analysis, was a nice expirience. I am happy to share the NoteBook(s), and related material, and hope that the code and this text has helped you in your project, and that it gave you some ideas on how to use NTL data; I am looking forward to the reactions and feedback in the comments.

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


Table 1: Causal Imapact Results, method adapted from CausalImpact
            <sup id="a5">[5](#f1)</sup>
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
</table>
<br>
<br>

<h2>Conclusion</h2>
<p>

</p>
<br>


---
<br>

<b id="f1">a</b> https://www.linkedin.com/in/gvddool/ [↩](#aa)<br>
<b id="f1">b</b> https://www.spaceinssolutions.com/ [↩](#ab)<br>
<b id="f1">c</b> https://www.spaceinssolutions.com/ [↩](#ac)<br>

<h2>References</h2>
<p>

Example 3 <sup id="a3">[3](#f1)</sup><br>
Example 4 <sup id="a4">[4](#f1)</sup><br>

<b id="f1">3</b> https://www.linkedin.com/in/gvddool/ [↩](#a3)<br>
<b id="f1">4</b> https://www.spaceinssolutions.com/ [↩](#a4)<br>

<b id="f1">5</b> CausalImpact GitHub repro https://github.com/dafiti/ [↩](#a5)<br>

</p>



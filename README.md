Download Link: https://assignmentchef.com/product/solved-csc370-assignment-4
<br>
Some of the queries in this assignment involve floating point data. In the expected output shown below, there might be slight differences in floating point values due to rounding and formatting issues. You may assume that floating point values in your query results match the expected output if they are equivalent to four decimal places (e.g. if the expected output is written as ‘0.1234’, the values ‘0.123398’ and ‘0.1234567’ would both be considered correct, but the value ‘0.123’ would not).

<strong>Question 1</strong>: IMDB Queries

Create queries for each of the data retrieval problems below, using the imdb database. In the questions below, any reference to ‘films’ refers to titles with title_type = ‘movie’.

<ul>

 <li>For each year between 2000 and 2017 (inclusive), list the primary name, production year, rating and number of votes of the film or films which attained the highest rating among all movies produced in that year which received at least 10000 votes. Both the rating and number of votes are stored in the ratings</li>

</ul>

<table width="510">

 <tbody>

  <tr>

   <td colspan="4" width="510">Expected Query Result</td>

  </tr>

  <tr>

   <td width="340">primary name</td>

   <td width="46">year</td>

   <td width="57">rating</td>

   <td width="67">votes</td>

  </tr>

  <tr>

   <td width="340">Memento</td>

   <td width="46">2000</td>

   <td width="57">8.5000</td>

   <td width="67">942432</td>

  </tr>

  <tr>

   <td width="340">Gladiator</td>

   <td width="46">2000</td>

   <td width="57">8.5000</td>

   <td width="67">1095891</td>

  </tr>

  <tr>

   <td width="340">The Lord of the Rings: The Fellowship of the Ring</td>

   <td width="46">2001</td>

   <td width="57">8.8000</td>

   <td width="67">1370113</td>

  </tr>

  <tr>

   <td width="340">The Lord of the Rings: The Two Towers</td>

   <td width="46">2002</td>

   <td width="57">8.7000</td>

   <td width="67">1221886</td>

  </tr>

  <tr>

   <td width="340">The Lord of the Rings: The Return of the King</td>

   <td width="46">2003</td>

   <td width="57">8.9000</td>

   <td width="67">1349934</td>

  </tr>

  <tr>

   <td width="340">Anbe Sivam</td>

   <td width="46">2003</td>

   <td width="57">8.9000</td>

   <td width="67">10116</td>

  </tr>

  <tr>

   <td width="340">Black Friday</td>

   <td width="46">2004</td>

   <td width="57">8.6000</td>

   <td width="67">13513</td>

  </tr>

  <tr>

   <td width="340">Earthlings</td>

   <td width="46">2005</td>

   <td width="57">8.7000</td>

   <td width="67">14649</td>

  </tr>

  <tr>

   <td width="340">The Prestige</td>

   <td width="46">2006</td>

   <td width="57">8.5000</td>

   <td width="67">959259</td>

  </tr>

  <tr>

   <td width="340">The Lives of Others</td>

   <td width="46">2006</td>

   <td width="57">8.5000</td>

   <td width="67">290278</td>

  </tr>

  <tr>

   <td width="340">The Departed</td>

   <td width="46">2006</td>

   <td width="57">8.5000</td>

   <td width="67">975612</td>

  </tr>

  <tr>

   <td width="340">Like Stars on Earth</td>

   <td width="46">2007</td>

   <td width="57">8.5000</td>

   <td width="67">113421</td>

  </tr>

  <tr>

   <td width="340">The Dark Knight</td>

   <td width="46">2008</td>

   <td width="57">9.0000</td>

   <td width="67">1864795</td>

  </tr>

  <tr>

   <td width="340">Home</td>

   <td width="46">2009</td>

   <td width="57">8.6000</td>

   <td width="67">19621</td>

  </tr>

  <tr>

   <td width="340">Inception</td>

   <td width="46">2010</td>

   <td width="57">8.8000</td>

   <td width="67">1653611</td>

  </tr>

  <tr>

   <td width="340">The Intouchables</td>

   <td width="46">2011</td>

   <td width="57">8.6000</td>

   <td width="67">591006</td>

  </tr>

  <tr>

   <td width="340">The Dark Knight Rises</td>

   <td width="46">2012</td>

   <td width="57">8.4000</td>

   <td width="67">1269644</td>

  </tr>

  <tr>

   <td width="340">Django Unchained</td>

   <td width="46">2012</td>

   <td width="57">8.4000</td>

   <td width="67">1087769</td>

  </tr>

  <tr>

   <td width="340">CM101MMXI Fundamentals</td>

   <td width="46">2013</td>

   <td width="57">9.3000</td>

   <td width="67">38106</td>

  </tr>

  <tr>

   <td width="340">Interstellar</td>

   <td width="46">2014</td>

   <td width="57">8.6000</td>

   <td width="67">1120400</td>

  </tr>

  <tr>

   <td width="340">RangiTaranga</td>

   <td width="46">2015</td>

   <td width="57">8.7000</td>

   <td width="67">10286</td>

  </tr>

  <tr>

   <td width="340">The Mountain II</td>

   <td width="46">2016</td>

   <td width="57">9.6000</td>

   <td width="67">93071</td>

  </tr>

  <tr>

   <td width="340">Ayla: The Daughter of War</td>

   <td width="46">2017</td>

   <td width="57">9.1000</td>

   <td width="67">15807</td>

  </tr>

 </tbody>

</table>

<ul>

 <li>Select the primary name and episode count of each TV series (contained in the tv_series table) for which at least 6000 episodes have been produced.</li>

</ul>

<table width="380">

 <tbody>

  <tr>

   <td width="291">Expected Query Result</td>

   <td width="88"> </td>

  </tr>

  <tr>

   <td width="291">series name</td>

   <td width="88">episode count</td>

  </tr>

  <tr>

   <td width="291">Days of Our Lives</td>

   <td width="88">10240</td>

  </tr>

  <tr>

   <td width="291">Ohayou Tokushima</td>

   <td width="88">9502</td>

  </tr>

  <tr>

   <td width="291">Coronation Street</td>

   <td width="88">9316</td>

  </tr>

  <tr>

   <td width="291">Neighbours</td>

   <td width="88">8911</td>

  </tr>

  <tr>

   <td width="291">Six O’Clock News</td>

   <td width="88">8646</td>

  </tr>

  <tr>

   <td width="291">The Price Is Right</td>

   <td width="88">8461</td>

  </tr>

  <tr>

   <td width="291">One O’Clock News</td>

   <td width="88">8100</td>

  </tr>

  <tr>

   <td width="291">Jeopardy!</td>

   <td width="88">7599</td>

  </tr>

  <tr>

   <td width="291">EastEnders</td>

   <td width="88">7393</td>

  </tr>

  <tr>

   <td width="291">The Bold and the Beautiful</td>

   <td width="88">7236</td>

  </tr>

  <tr>

   <td width="291">Home and Away</td>

   <td width="88">7081</td>

  </tr>

  <tr>

   <td width="291">Wheel of Fortune</td>

   <td width="88">6564</td>

  </tr>

  <tr>

   <td width="291">Gute Zeiten, schlechte Zeiten</td>

   <td width="88">6413</td>

  </tr>

  <tr>

   <td width="291">The Tonight Show Starring Johnny Carson</td>

   <td width="88">6037</td>

  </tr>

  <tr>

   <td width="291">The Young and the Restless</td>

   <td width="88">6024</td>

  </tr>

 </tbody>

</table>

<strong>Question 2</strong>: BC Ferries Queries [14 marks]

The queries you write below should work correctly on any of the BC Ferries databases (ferries_1month, ferries_3months, ferries_6months, ferries_9months, ferries_1year or ferries_3years). For comparison, sample output is shown for both ferries_1month and ferries_3years.

The following definitions apply to all of the parts below unless otherwise stated.

<ul>

 <li>The ‘duration’ of a sailing is defined to be the number of minutes between the scheduled departure (not the actual departure) and the arrival of that sailing.</li>

 <li>Any reference to the ‘day of a sailing’ refers to the calendar day of the scheduled departure (not the actual departure) of that sailing.</li>

</ul>

<ul>

 <li>For many routes, there are simultaneous sailings in both directions at the same time. For example, on a typical day at 9:00am, a ferry leaves Tsawwassen for Swartz Bay and a different ferry leaves Swartz Bay for Tsawwassen. Not all routes or sailings have this property. We will define two vessels as ‘paired up’ if they have both served the same route number at the same (scheduled) departure time/date. Construct a query to count the number of times each distinct pair of ferries have been paired up. Your result must not contain counts for pairs of vessels which have never been paired up. Each distinct pair of ferries should appear only once in your result, and in the result rows, the vessel names of each pair must be ordered alphabetically (so the alphabetically lowest vessel name will be listed first).</li>

</ul>

<table width="449">

 <tbody>

  <tr>

   <td width="7"> </td>

   <td colspan="2" width="366">Expected Query Result (ferries 1month)</td>

   <td colspan="2" width="83"> </td>

   <td width="7"> </td>

  </tr>

  <tr>

   <td width="7"> </td>

   <td width="183">vessel1</td>

   <td width="183">vessel2</td>

   <td colspan="2" width="83">num pairings</td>

   <td width="7"> </td>

  </tr>

  <tr>

   <td width="7"> </td>

   <td width="183">Coastal Inspiration</td>

   <td width="183">Queen of Alberni</td>

   <td colspan="2" width="83">158</td>

   <td width="7"> </td>

  </tr>

  <tr>

   <td width="7"> </td>

   <td width="183">Spirit of British Columbia</td>

   <td width="183">Spirit of Vancouver Island</td>

   <td colspan="2" width="83">10</td>

   <td width="7"> </td>

  </tr>

  <tr>

   <td colspan="6" width="463">Expected Query Result (ferries 3years)</td>

  </tr>

  <tr>

   <td colspan="2" width="190">vessel1</td>

   <td colspan="2" width="190">vessel2</td>

   <td colspan="2" width="83">num pairings</td>

  </tr>

  <tr>

   <td colspan="2" width="190">Coastal Inspiration</td>

   <td colspan="2" width="190">Queen of Alberni</td>

   <td colspan="2" width="83">5449</td>

  </tr>

  <tr>

   <td colspan="2" width="190">Spirit of British Columbia</td>

   <td colspan="2" width="190">Spirit of Vancouver Island</td>

   <td colspan="2" width="83">3552</td>

  </tr>

  <tr>

   <td colspan="2" width="190">Queen of Cowichan</td>

   <td colspan="2" width="190">Queen of Oak Bay</td>

   <td colspan="2" width="83">3048</td>

  </tr>

  <tr>

   <td colspan="2" width="190">Coastal Celebration</td>

   <td colspan="2" width="190">Queen of New Westminster</td>

   <td colspan="2" width="83">2261</td>

  </tr>

  <tr>

   <td colspan="2" width="190">Coastal Renaissance</td>

   <td colspan="2" width="190">Queen of Oak Bay</td>

   <td colspan="2" width="83">1825</td>

  </tr>

  <tr>

   <td colspan="2" width="190">Coastal Celebration</td>

   <td colspan="2" width="190">Spirit of British Columbia</td>

   <td colspan="2" width="83">1653</td>

  </tr>

  <tr>

   <td colspan="2" width="190">Coastal Celebration</td>

   <td colspan="2" width="190">Spirit of Vancouver Island</td>

   <td colspan="2" width="83">1247</td>

  </tr>

  <tr>

   <td colspan="2" width="190">Coastal Renaissance</td>

   <td colspan="2" width="190">Spirit of Vancouver Island</td>

   <td colspan="2" width="83">847</td>

  </tr>

  <tr>

   <td colspan="2" width="190">Coastal Renaissance</td>

   <td colspan="2" width="190">Queen of Alberni</td>

   <td colspan="2" width="83">814</td>

  </tr>

  <tr>

   <td colspan="2" width="190">Coastal Celebration</td>

   <td colspan="2" width="190">Coastal Renaissance</td>

   <td colspan="2" width="83">622</td>

  </tr>

  <tr>

   <td colspan="2" width="190">Coastal Renaissance</td>

   <td colspan="2" width="190">Queen of New Westminster</td>

   <td colspan="2" width="83">594</td>

  </tr>

  <tr>

   <td colspan="2" width="190">Coastal Inspiration</td>

   <td colspan="2" width="190">Queen of New Westminster</td>

   <td colspan="2" width="83">592</td>

  </tr>

  <tr>

   <td colspan="2" width="190">Queen of Coquitlam</td>

   <td colspan="2" width="190">Queen of Cowichan</td>

   <td colspan="2" width="83">548</td>

  </tr>

  <tr>

   <td colspan="2" width="190">Queen of Coquitlam</td>

   <td colspan="2" width="190">Queen of Oak Bay</td>

   <td colspan="2" width="83">481</td>

  </tr>

  <tr>

   <td colspan="2" width="190">Queen of Alberni</td>

   <td colspan="2" width="190">Queen of Coquitlam</td>

   <td colspan="2" width="83">400</td>

  </tr>

  <tr>

   <td colspan="2" width="190">Queen of Coquitlam</td>

   <td colspan="2" width="190">Queen of New Westminster</td>

   <td colspan="2" width="83">152</td>

  </tr>

  <tr>

   <td colspan="2" width="190">Coastal Renaissance</td>

   <td colspan="2" width="190">Spirit of British Columbia</td>

   <td colspan="2" width="83">53</td>

  </tr>

  <tr>

   <td colspan="2" width="190">Coastal Celebration</td>

   <td colspan="2" width="190">Coastal Inspiration</td>

   <td colspan="2" width="83">24</td>

  </tr>

  <tr>

   <td colspan="2" width="190">Queen of New Westminster</td>

   <td colspan="2" width="190">Spirit of Vancouver Island</td>

   <td colspan="2" width="83">17</td>

  </tr>

  <tr>

   <td colspan="2" width="190">Coastal Inspiration</td>

   <td colspan="2" width="190">Spirit of British Columbia</td>

   <td colspan="2" width="83">8</td>

  </tr>

  <tr>

   <td colspan="2" width="190">Queen of Coquitlam</td>

   <td colspan="2" width="190">Queen of Surrey</td>

   <td colspan="2" width="83">3</td>

  </tr>

  <tr>

   <td colspan="2" width="190">Coastal Renaissance</td>

   <td colspan="2" width="190">Queen of Cowichan</td>

   <td colspan="2" width="83">1</td>

  </tr>

  <tr>

   <td width="7"></td>

   <td width="177"></td>

   <td width="177"></td>

   <td width="7"></td>

   <td width="74"></td>

   <td width="7"></td>

  </tr>

 </tbody>

</table>

<ul>

 <li>The routes table contains the ‘nominal duration’ of each route, which is the expected crossing time. The nominal duration is determined by BC Ferries based on the average marine and traffic conditions, along with information like loading times and the speed of the vessels. We can test the accuracy of this calculation by computing the average time of each crossing. Construct a query to find, for each route number, the nominal duration (in minutes) and the average duration (in minutes) of a crossing based on all available data for that route. For this question, assume that the ‘duration’ of a particular sailing is the time between its scheduled departure and its arrival.</li>

</ul>

<table width="286">

 <tbody>

  <tr>

   <td colspan="3" width="286">Expected Query Result (ferries 1month)</td>

  </tr>

  <tr>

   <td width="83">route number</td>

   <td width="105">nominal duration</td>

   <td width="98">avg duration</td>

  </tr>

  <tr>

   <td width="83">1</td>

   <td width="105">95</td>

   <td width="98">101.2424</td>

  </tr>

  <tr>

   <td width="83">3</td>

   <td width="105">40</td>

   <td width="98">44.9415</td>

  </tr>

  <tr>

   <td width="83">4</td>

   <td width="105">35</td>

   <td width="98">33.2479</td>

  </tr>

  <tr>

   <td width="83">8</td>

   <td width="105">20</td>

   <td width="98">20.5182</td>

  </tr>

  <tr>

   <td width="83">30</td>

   <td width="105">120</td>

   <td width="98">129.0709</td>

  </tr>

  <tr>

   <td colspan="3" width="286">Expected Query Result (ferries 3years)</td>

  </tr>

  <tr>

   <td width="83">route number</td>

   <td width="105">nominal duration</td>

   <td width="98">avg duration</td>

  </tr>

  <tr>

   <td width="83">1</td>

   <td width="105">95</td>

   <td width="98">92.8867</td>

  </tr>

  <tr>

   <td width="83">2</td>

   <td width="105">100</td>

   <td width="98">106.8488</td>

  </tr>

  <tr>

   <td width="83">3</td>

   <td width="105">40</td>

   <td width="98">45.1520</td>

  </tr>

  <tr>

   <td width="83">4</td>

   <td width="105">35</td>

   <td width="98">31.8939</td>

  </tr>

  <tr>

   <td width="83">8</td>

   <td width="105">20</td>

   <td width="98">21.9507</td>

  </tr>

  <tr>

   <td width="83">30</td>

   <td width="105">120</td>

   <td width="98">123.0126</td>

  </tr>

 </tbody>

</table>

<ul>

 <li>Suppose we define a sailing to be ‘late’ if the duration is at least five minutes longer<a href="#_ftn1" name="_ftnref1"><sup>[1]</sup></a> than the nominal duration in the routes Construct a query to find, for each month, the number of days for which at least one sailing occurred on Route 1 but no late sailings occurred on route number 1.</li>

</ul>

<table width="286">

 <tbody>

  <tr>

   <td colspan="2" width="286">Expected Query Result (ferries 1month)</td>

  </tr>

  <tr>

   <td width="45">month</td>

   <td width="242">count</td>

  </tr>

  <tr>

   <td width="45">4</td>

   <td width="242">1</td>

  </tr>

  <tr>

   <td colspan="2" width="286">Expected Query Result (ferries 3years)</td>

  </tr>

  <tr>

   <td width="45">month</td>

   <td width="242">count</td>

  </tr>

  <tr>

   <td width="45">1</td>

   <td width="242">65</td>

  </tr>

  <tr>

   <td width="45">2</td>

   <td width="242">53</td>

  </tr>

  <tr>

   <td width="45">3</td>

   <td width="242">58</td>

  </tr>

  <tr>

   <td width="45">4</td>

   <td width="242">29</td>

  </tr>

  <tr>

   <td width="45">5</td>

   <td width="242">19</td>

  </tr>

  <tr>

   <td width="45">6</td>

   <td width="242">23</td>

  </tr>

  <tr>

   <td width="45">7</td>

   <td width="242">22</td>

  </tr>

  <tr>

   <td width="45">8</td>

   <td width="242">18</td>

  </tr>

  <tr>

   <td width="45">9</td>

   <td width="242">43</td>

  </tr>

  <tr>

   <td width="45">10</td>

   <td width="242">45</td>

  </tr>

  <tr>

   <td width="45">11</td>

   <td width="242">51</td>

  </tr>

  <tr>

   <td width="45">12</td>

   <td width="242">60</td>

  </tr>

 </tbody>

</table>

<ul>

 <li>Construct a query to find, for each vessel with any sailings, the total number of sailings it has made, the number of late sailings it has made (which may be zero) and the fraction of its sailings that were late (that is, the number of late sailings divided by the total number of sailings). You should be careful with this query: a vessel may be involved in multiple routes, each with a different nominal duration.</li>

</ul>

<table width="454">

 <tbody>

  <tr>

   <td width="4"> </td>

   <td colspan="5" width="365">Expected Query Result (ferries 1month)</td>

   <td colspan="2" width="88"> </td>

   <td width="4"> </td>

  </tr>

  <tr>

   <td width="4"> </td>

   <td width="183">vessel name</td>

   <td colspan="2" width="94">total sailings</td>

   <td colspan="2" width="88">late sailings</td>

   <td colspan="2" width="88">late fraction</td>

   <td width="4"> </td>

  </tr>

  <tr>

   <td width="4"> </td>

   <td width="183">Coastal Inspiration</td>

   <td colspan="2" width="94">232</td>

   <td colspan="2" width="88">166</td>

   <td colspan="2" width="88">0.7155</td>

   <td width="4"> </td>

  </tr>

  <tr>

   <td width="4"> </td>

   <td width="183">Coastal Renaissance</td>

   <td colspan="2" width="94">39</td>

   <td colspan="2" width="88">14</td>

   <td colspan="2" width="88">0.3590</td>

   <td width="4"> </td>

  </tr>

  <tr>

   <td width="4"> </td>

   <td width="183">Queen of Alberni</td>

   <td colspan="2" width="94">163</td>

   <td colspan="2" width="88">43</td>

   <td colspan="2" width="88">0.2638</td>

   <td width="4"> </td>

  </tr>

  <tr>

   <td width="4"> </td>

   <td width="183">Queen of Capilano</td>

   <td colspan="2" width="94">440</td>

   <td colspan="2" width="88">30</td>

   <td colspan="2" width="88">0.0682</td>

   <td width="4"> </td>

  </tr>

  <tr>

   <td width="4"> </td>

   <td width="183">Queen of Coquitlam</td>

   <td colspan="2" width="94">68</td>

   <td colspan="2" width="88">16</td>

   <td colspan="2" width="88">0.2353</td>

   <td width="4"> </td>

  </tr>

  <tr>

   <td width="4"> </td>

   <td width="183">Queen of Surrey</td>

   <td colspan="2" width="94">274</td>

   <td colspan="2" width="88">100</td>

   <td colspan="2" width="88">0.3650</td>

   <td width="4"> </td>

  </tr>

  <tr>

   <td width="4"> </td>

   <td width="183">Skeena Queen</td>

   <td colspan="2" width="94">234</td>

   <td colspan="2" width="88">22</td>

   <td colspan="2" width="88">0.0940</td>

   <td width="4"> </td>

  </tr>

  <tr>

   <td width="4"> </td>

   <td width="183">Spirit of British Columbia</td>

   <td colspan="2" width="94">164</td>

   <td colspan="2" width="88">98</td>

   <td colspan="2" width="88">0.5976</td>

   <td width="4"> </td>

  </tr>

  <tr>

   <td width="4"> </td>

   <td width="183">Spirit of Vancouver Island</td>

   <td colspan="2" width="94">94</td>

   <td colspan="2" width="88">23</td>

   <td colspan="2" width="88">0.2447</td>

   <td width="4"> </td>

  </tr>

  <tr>

   <td colspan="7" width="373">Expected Query Result (ferries 3years)</td>

   <td colspan="2" width="88"> </td>

  </tr>

  <tr>

   <td colspan="3" width="190">vessel name</td>

   <td colspan="2" width="94">total sailings</td>

   <td colspan="2" width="88">late sailings</td>

   <td colspan="2" width="88">late fraction</td>

  </tr>

  <tr>

   <td colspan="3" width="190">Bowen Queen</td>

   <td colspan="2" width="94">1268</td>

   <td colspan="2" width="88">83</td>

   <td colspan="2" width="88">0.0655</td>

  </tr>

  <tr>

   <td colspan="3" width="190">Coastal Celebration</td>

   <td colspan="2" width="94">6506</td>

   <td colspan="2" width="88">406</td>

   <td colspan="2" width="88">0.0624</td>

  </tr>

  <tr>

   <td colspan="3" width="190">Coastal Inspiration</td>

   <td colspan="2" width="94">6545</td>

   <td colspan="2" width="88">2502</td>

   <td colspan="2" width="88">0.3823</td>

  </tr>

  <tr>

   <td colspan="3" width="190">Coastal Renaissance</td>

   <td colspan="2" width="94">5637</td>

   <td colspan="2" width="88">1220</td>

   <td colspan="2" width="88">0.2164</td>

  </tr>

  <tr>

   <td colspan="3" width="190">Mayne Queen</td>

   <td colspan="2" width="94">1</td>

   <td colspan="2" width="88">0</td>

   <td colspan="2" width="88">0.0000</td>

  </tr>

  <tr>

   <td colspan="3" width="190">Queen of Alberni</td>

   <td colspan="2" width="94">6903</td>

   <td colspan="2" width="88">1164</td>

   <td colspan="2" width="88">0.1686</td>

  </tr>

  <tr>

   <td colspan="3" width="190">Queen of Capilano</td>

   <td colspan="2" width="94">14277</td>

   <td colspan="2" width="88">2806</td>

   <td colspan="2" width="88">0.1965</td>

  </tr>

  <tr>

   <td colspan="3" width="190">Queen of Coquitlam</td>

   <td colspan="2" width="94">6650</td>

   <td colspan="2" width="88">2230</td>

   <td colspan="2" width="88">0.3353</td>

  </tr>

  <tr>

   <td colspan="3" width="190">Queen of Cowichan</td>

   <td colspan="2" width="94">7071</td>

   <td colspan="2" width="88">2946</td>

   <td colspan="2" width="88">0.4166</td>

  </tr>

  <tr>

   <td colspan="3" width="190">Queen of Cumberland</td>

   <td colspan="2" width="94">974</td>

   <td colspan="2" width="88">113</td>

   <td colspan="2" width="88">0.1160</td>

  </tr>

  <tr>

   <td colspan="3" width="190">Queen of New Westminster</td>

   <td colspan="2" width="94">3966</td>

   <td colspan="2" width="88">439</td>

   <td colspan="2" width="88">0.1107</td>

  </tr>

  <tr>

   <td colspan="3" width="190">Queen of Oak Bay</td>

   <td colspan="2" width="94">6609</td>

   <td colspan="2" width="88">4592</td>

   <td colspan="2" width="88">0.6948</td>

  </tr>

  <tr>

   <td colspan="3" width="190">Queen of Surrey</td>

   <td colspan="2" width="94">12759</td>

   <td colspan="2" width="88">4555</td>

   <td colspan="2" width="88">0.3570</td>

  </tr>

  <tr>

   <td colspan="3" width="190">Quinitsa</td>

   <td colspan="2" width="94">8</td>

   <td colspan="2" width="88">8</td>

   <td colspan="2" width="88">1.0000</td>

  </tr>

  <tr>

   <td colspan="3" width="190">Skeena Queen</td>

   <td colspan="2" width="94">7312</td>

   <td colspan="2" width="88">378</td>

   <td colspan="2" width="88">0.0517</td>

  </tr>

  <tr>

   <td colspan="3" width="190">Spirit of British Columbia</td>

   <td colspan="2" width="94">5539</td>

   <td colspan="2" width="88">1013</td>

   <td colspan="2" width="88">0.1829</td>

  </tr>

  <tr>

   <td colspan="3" width="190">Spirit of Vancouver Island</td>

   <td colspan="2" width="94">5916</td>

   <td colspan="2" width="88">791</td>

   <td colspan="2" width="88">0.1337</td>

  </tr>

  <tr>

   <td width="4"></td>

   <td width="180"></td>

   <td width="4"></td>

   <td width="89"></td>

   <td width="4"></td>

   <td width="83"></td>

   <td width="4"></td>

   <td width="84"></td>

   <td width="4"></td>

  </tr>

 </tbody>

</table>

<ul>

 <li>Usually, you would expect that when the beginning of a sailing is delayed (that is, when actual_departure is much later than scheduled_departure), the arrival is also delayed and the sailing is late. However, in some cases, a vessel that departs late may still arrive on time. Define a ‘made up sailing’ to be any sailing which leaves at least 15 minutes after its scheduled departure but arrives less than (or equal to) five minutes late. Write a query to list the number of made up sailings in the dataset for each vessel. Only vessels with at least one made up sailing should be listed.</li>

</ul>

<table width="287">

 <tbody>

  <tr>

   <td width="4"> </td>

   <td colspan="3" width="287">Expected Query Result (ferries 1month)</td>

   <td width="4"> </td>

  </tr>

  <tr>

   <td width="4"> </td>

   <td width="183">vessel name</td>

   <td colspan="2" width="104">made up sailings</td>

   <td width="4"> </td>

  </tr>

  <tr>

   <td width="4"> </td>

   <td width="183">Coastal Inspiration</td>

   <td colspan="2" width="104">4</td>

   <td width="4"> </td>

  </tr>

  <tr>

   <td width="4"> </td>

   <td width="183">Coastal Renaissance</td>

   <td colspan="2" width="104">2</td>

   <td width="4"> </td>

  </tr>

  <tr>

   <td width="4"> </td>

   <td width="183">Spirit of British Columbia</td>

   <td colspan="2" width="104">3</td>

   <td width="4"> </td>

  </tr>

  <tr>

   <td colspan="5" width="294">Expected Query Result (ferries 3years)</td>

  </tr>

  <tr>

   <td colspan="3" width="190">vessel name</td>

   <td colspan="2" width="104">made up sailings</td>

  </tr>

  <tr>

   <td colspan="3" width="190">Coastal Celebration</td>

   <td colspan="2" width="104">109</td>

  </tr>

  <tr>

   <td colspan="3" width="190">Coastal Inspiration</td>

   <td colspan="2" width="104">70</td>

  </tr>

  <tr>

   <td colspan="3" width="190">Coastal Renaissance</td>

   <td colspan="2" width="104">53</td>

  </tr>

  <tr>

   <td colspan="3" width="190">Queen of Alberni</td>

   <td colspan="2" width="104">11</td>

  </tr>

  <tr>

   <td colspan="3" width="190">Queen of Coquitlam</td>

   <td colspan="2" width="104">7</td>

  </tr>

  <tr>

   <td colspan="3" width="190">Queen of Cowichan</td>

   <td colspan="2" width="104">1</td>

  </tr>

  <tr>

   <td colspan="3" width="190">Queen of New Westminster</td>

   <td colspan="2" width="104">28</td>

  </tr>

  <tr>

   <td colspan="3" width="190">Queen of Oak Bay</td>

   <td colspan="2" width="104">1</td>

  </tr>

  <tr>

   <td colspan="3" width="190">Skeena Queen</td>

   <td colspan="2" width="104">2</td>

  </tr>

  <tr>

   <td colspan="3" width="190">Spirit of British Columbia</td>

   <td colspan="2" width="104">57</td>

  </tr>

  <tr>

   <td colspan="3" width="190">Spirit of Vancouver Island</td>

   <td colspan="2" width="104">75</td>

  </tr>

  <tr>

   <td width="4"></td>

   <td width="178"></td>

   <td width="4"></td>

   <td width="97"></td>

   <td width="4"></td>

  </tr>

 </tbody>

</table>

<ul>

 <li>Define a ‘good day’ for a particular route number to be a day where at least one sailing occurred and no late sailings occurred. For each route, find the maximum number of <em>good days </em>in a row over the entire dataset.</li>

</ul>

Note that the rather unimpressive results for the ferries_1month dataset compared to the other datasets seem to be the result of COVID-19 related service reductions and extra precautions (which may be increasing the number of late sailings).

Hint: This is probably easiest when you use a large number of CTE expressions (that is, subqueries in the WITH clause).

<table width="286">

 <tbody>

  <tr>

   <td colspan="2" width="286">Expected Query Result (ferries 1month)</td>

  </tr>

  <tr>

   <td width="83">route number</td>

   <td width="204">max consecutive good days</td>

  </tr>

  <tr>

   <td width="83">1</td>

   <td width="204">1</td>

  </tr>

  <tr>

   <td width="83">2</td>

   <td width="204">0</td>

  </tr>

  <tr>

   <td width="83">3</td>

   <td width="204">1</td>

  </tr>

  <tr>

   <td width="83">4</td>

   <td width="204">3</td>

  </tr>

  <tr>

   <td width="83">8</td>

   <td width="204">4</td>

  </tr>

  <tr>

   <td width="83">30</td>

   <td width="204">0</td>

  </tr>

  <tr>

   <td colspan="2" width="286">Expected Query Result (ferries 3years)</td>

  </tr>

  <tr>

   <td width="83">route number</td>

   <td width="204">max consecutive good days</td>

  </tr>

  <tr>

   <td width="83">1</td>

   <td width="204">15</td>

  </tr>

  <tr>

   <td width="83">2</td>

   <td width="204">2</td>

  </tr>

  <tr>

   <td width="83">3</td>

   <td width="204">4</td>

  </tr>

  <tr>

   <td width="83">4</td>

   <td width="204">27</td>

  </tr>

  <tr>

   <td width="83">8</td>

   <td width="204">8</td>

  </tr>

  <tr>

   <td width="83">30</td>

   <td width="204">6</td>

  </tr>

 </tbody>

</table>

<ul>

 <li>For each route, output all date ranges where the maximum number of consecutive <em>good days </em>(as defined in part (f) above) was achieved. For some routes, only one date range will meet this criteria, but for others (e.g. route 2 in the ferries_3years dataset) there may be multiple date ranges of the same size. The columns containing the start and end dates should contain values of type DATE (created, for example, by the make_date function).</li>

</ul>

<table width="404">

 <tbody>

  <tr>

   <td colspan="4" width="404">Expected Query Result (ferries 1month)</td>

  </tr>

  <tr>

   <td width="83">route number</td>

   <td width="84">start date</td>

   <td width="84">end date</td>

   <td width="153">max consecutive good days</td>

  </tr>

  <tr>

   <td width="83">1</td>

   <td width="84">2020-04-26</td>

   <td width="84">2020-04-26</td>

   <td width="153">1</td>

  </tr>

  <tr>

   <td width="83">3</td>

   <td width="84">2020-04-15</td>

   <td width="84">2020-04-15</td>

   <td width="153">1</td>

  </tr>

  <tr>

   <td width="83">4</td>

   <td width="84">2020-04-19</td>

   <td width="84">2020-04-21</td>

   <td width="153">3</td>

  </tr>

  <tr>

   <td width="83">8</td>

   <td width="84">2020-04-29</td>

   <td width="84">2020-05-02</td>

   <td width="153">4</td>

  </tr>

  <tr>

   <td colspan="4" width="404">Expected Query Result (ferries 3years)</td>

  </tr>

  <tr>

   <td width="83">route number</td>

   <td width="84">start date</td>

   <td width="84">end date</td>

   <td width="153">max consecutive good days</td>

  </tr>

  <tr>

   <td width="83">1</td>

   <td width="84">2017-12-21</td>

   <td width="84">2018-01-04</td>

   <td width="153">15</td>

  </tr>

  <tr>

   <td width="83">2</td>

   <td width="84">2017-05-20</td>

   <td width="84">2017-05-21</td>

   <td width="153">2</td>

  </tr>

  <tr>

   <td width="83">2</td>

   <td width="84">2017-09-26</td>

   <td width="84">2017-09-27</td>

   <td width="153">2</td>

  </tr>

  <tr>

   <td width="83">3</td>

   <td width="84">2018-02-24</td>

   <td width="84">2018-02-27</td>

   <td width="153">4</td>

  </tr>

  <tr>

   <td width="83">4</td>

   <td width="84">2018-09-02</td>

   <td width="84">2018-09-28</td>

   <td width="153">27</td>

  </tr>

  <tr>

   <td width="83">8</td>

   <td width="84">2019-03-06</td>

   <td width="84">2019-03-13</td>

   <td width="153">8</td>

  </tr>

  <tr>

   <td width="83">30</td>

   <td width="84">2017-09-23</td>

   <td width="84">2017-09-28</td>

   <td width="153">6</td>

  </tr>

 </tbody>

</table>

<strong>Question 3</strong>: VWSN Queries [10 marks]

Create queries for each of the data retrieval problems below, using the vwsn 1year database.

<ul>

 <li>Find the highest observed temperature in the dataset, along with the station number, station name and observation time of all cases where that temperature was reported.</li>

</ul>

Note: The expected output below is correct (that is, the observation shown is actually in the dataset, even though it appears to be unseasonably warm).

<table width="602">

 <tbody>

  <tr>

   <td width="71"> </td>

   <td width="311">Expected Query Result</td>

   <td width="79"> </td>

   <td width="141"> </td>

  </tr>

  <tr>

   <td width="71">station id</td>

   <td width="311">name</td>

   <td width="79">temperature</td>

   <td width="141">observation time</td>

  </tr>

  <tr>

   <td width="71">180</td>

   <td width="311">Captain Meares Elementary Secondary School</td>

   <td width="79">42.6000</td>

   <td width="141">2019-10-05 15:11:00</td>

  </tr>

 </tbody>

</table>

<ul>

 <li>For each station with station ID between 1 and 10 (inclusive), list the station ID, station name, maximum temperature observed at that station and observation time of <strong>all </strong>observations in the dataset in which the maximum temperature was attained at that station. Only include stations which actually have recorded observations in the dataset.</li>

</ul>

<table width="659">

 <tbody>

  <tr>

   <td colspan="4" width="659">Expected Query Result</td>

  </tr>

  <tr>

   <td width="71">station id</td>

   <td width="347">name</td>

   <td width="100">max temperature</td>

   <td width="141">observation time</td>

  </tr>

  <tr>

   <td width="71">1</td>

   <td width="347">Ian Stewart Complex/Mt. Douglas High School</td>

   <td width="100">29.8000</td>

   <td width="141">2019-08-05 16:31:00</td>

  </tr>

  <tr>

   <td width="71">3</td>

   <td width="347">Strawberry Vale Elementary School</td>

   <td width="100">30.2000</td>

   <td width="141">2019-06-12 15:15:00</td>

  </tr>

  <tr>

   <td width="71">3</td>

   <td width="347">Strawberry Vale Elementary School</td>

   <td width="100">30.2000</td>

   <td width="141">2019-06-12 15:21:00</td>

  </tr>

  <tr>

   <td width="71">4</td>

   <td width="347">Oaklands Elementary School</td>

   <td width="100">30.3000</td>

   <td width="141">2019-06-12 14:46:00</td>

  </tr>

  <tr>

   <td width="71">4</td>

   <td width="347">Oaklands Elementary School</td>

   <td width="100">30.3000</td>

   <td width="141">2019-06-12 14:52:00</td>

  </tr>

  <tr>

   <td width="71">5</td>

   <td width="347">Cedar Hill Middle School</td>

   <td width="100">30.2000</td>

   <td width="141">2019-06-12 17:12:00</td>

  </tr>

  <tr>

   <td width="71">6</td>

   <td width="347">Marigold Elementary School/Spectrum High School</td>

   <td width="100">29.8000</td>

   <td width="141">2019-06-12 14:41:00</td>

  </tr>

  <tr>

   <td width="71">7</td>

   <td width="347">Campus View Elementary</td>

   <td width="100">29.6000</td>

   <td width="141">2019-06-12 17:22:00</td>

  </tr>

  <tr>

   <td width="71">8</td>

   <td width="347">Victoria High School</td>

   <td width="100">29.7000</td>

   <td width="141">2019-06-12 14:41:00</td>

  </tr>

  <tr>

   <td width="71">9</td>

   <td width="347">Frank Hobbs Elementary School</td>

   <td width="100">29.2000</td>

   <td width="141">2019-08-05 17:27:00</td>

  </tr>

  <tr>

   <td width="71">10</td>

   <td width="347">Macaulay Elementary School</td>

   <td width="100">27.3000</td>

   <td width="141">2019-06-12 12:26:00</td>

  </tr>

 </tbody>

</table>

<ul>

 <li>Find the IDs and names of all stations which have reported at least one observation at some point, but which did not report <strong>any </strong>observations in January 2020.</li>

</ul>

<table width="403">

 <tbody>

  <tr>

   <td colspan="2" width="403">Expected Query Result</td>

  </tr>

  <tr>

   <td width="71">station id</td>

   <td width="332">name</td>

  </tr>

  <tr>

   <td width="71">13</td>

   <td width="332">Shoreline Middle School</td>

  </tr>

  <tr>

   <td width="71">16</td>

   <td width="332">Tillicum Elementary School</td>

  </tr>

  <tr>

   <td width="71">31</td>

   <td width="332">Sangster Elementary School</td>

  </tr>

  <tr>

   <td width="71">32</td>

   <td width="332">Colwood Elementary School</td>

  </tr>

  <tr>

   <td width="71">36</td>

   <td width="332">Hans Helgesen Elementary School</td>

  </tr>

  <tr>

   <td width="71">57</td>

   <td width="332">Wishart Elementary School</td>

  </tr>

  <tr>

   <td width="71">62</td>

   <td width="332">Deep Cove Elementary School</td>

  </tr>

  <tr>

   <td width="71">70</td>

   <td width="332">Parkland Secondary School</td>

  </tr>

  <tr>

   <td width="71">81</td>

   <td width="332">Braefoot Elementary School</td>

  </tr>

  <tr>

   <td width="71">94</td>

   <td width="332">Pender Islands Elementary and Secondary School</td>

  </tr>

  <tr>

   <td width="71">103</td>

   <td width="332">Frances Kelsey Secondary School</td>

  </tr>

  <tr>

   <td width="71">105</td>

   <td width="332">Port Renfrew Elementary School</td>

  </tr>

  <tr>

   <td width="71">108</td>

   <td width="332">Alberni Weather</td>

  </tr>

  <tr>

   <td width="71">109</td>

   <td width="332">Brentwood Elementary School</td>

  </tr>

  <tr>

   <td width="71">112</td>

   <td width="332">Saturna Elementary School</td>

  </tr>

  <tr>

   <td width="71">113</td>

   <td width="332">Mayne Island School</td>

  </tr>

  <tr>

   <td width="71">117</td>

   <td width="332">Saltspring Elementary and Middle Schools</td>

  </tr>

  <tr>

   <td width="71">124</td>

   <td width="332">Seaview Elementary School</td>

  </tr>

  <tr>

   <td width="71">131</td>

   <td width="332">Glenlyon Norfolk Junior School</td>

  </tr>

  <tr>

   <td width="71">133</td>

   <td width="332">Discovery Elementary School</td>

  </tr>

  <tr>

   <td width="71">136</td>

   <td width="332">Pleasant Valley Elementary School</td>

  </tr>

  <tr>

   <td width="71">160</td>

   <td width="332">Shawnigan Lake School</td>

  </tr>

  <tr>

   <td width="71">161</td>

   <td width="332">Bamfield Marine Sciences Centre</td>

  </tr>

  <tr>

   <td width="71">166</td>

   <td width="332">Maquinna Elementary School</td>

  </tr>

  <tr>

   <td width="71">180</td>

   <td width="332">Captain Meares Elementary Secondary School</td>

  </tr>

  <tr>

   <td width="71">195</td>

   <td width="332">North Island Distance Education School</td>

  </tr>

  <tr>

   <td width="71">196</td>

   <td width="332">Valley View Elementary School</td>

  </tr>

  <tr>

   <td width="71">226</td>

   <td width="332">Ditidaht Community School</td>

  </tr>

 </tbody>

</table>

<ul>

 <li>In this question (and the next question), define the ‘daily average temperature’ for a particular day to be the average of all observations from all stations on that day. Furthermore, for each month, define the ‘10 hottest days’ to be the top 10 days (by daily average temperature) and define the ‘10 coolest days’ to be the bottom 10 days (by daily average temperature). For each month/year pair in the dataset, compute the average daily average temperature across the ten hottest days and the average daily average temperature across the ten coolest days. Notice that you are computing an average of averages (first, find the average daily temperatures of each of the ten hottest days, then average those temperatures to produce the result). Hint:</li>

</ul>

Use the rank() function with an appropriate over() clause (maybe in multiple places)

<table width="312">

 <tbody>

  <tr>

   <td colspan="4" width="312">Expected Query Result</td>

  </tr>

  <tr>

   <td width="46">year</td>

   <td width="45">month</td>

   <td width="111">hottest10 average</td>

   <td width="111">coolest10 average</td>

  </tr>

  <tr>

   <td width="46">2019</td>

   <td width="45">5</td>

   <td width="111">16.8834</td>

   <td width="111">12.0071</td>

  </tr>

  <tr>

   <td width="46">2019</td>

   <td width="45">6</td>

   <td width="111">17.8665</td>

   <td width="111">13.8339</td>

  </tr>

  <tr>

   <td width="46">2019</td>

   <td width="45">7</td>

   <td width="111">19.0044</td>

   <td width="111">15.9400</td>

  </tr>

  <tr>

   <td width="46">2019</td>

   <td width="45">8</td>

   <td width="111">19.7309</td>

   <td width="111">16.5326</td>

  </tr>

  <tr>

   <td width="46">2019</td>

   <td width="45">9</td>

   <td width="111">17.0929</td>

   <td width="111">12.3717</td>

  </tr>

  <tr>

   <td width="46">2019</td>

   <td width="45">10</td>

   <td width="111">10.8171</td>

   <td width="111">6.5475</td>

  </tr>

  <tr>

   <td width="46">2019</td>

   <td width="45">11</td>

   <td width="111">9.2537</td>

   <td width="111">3.6983</td>

  </tr>

  <tr>

   <td width="46">2019</td>

   <td width="45">12</td>

   <td width="111">7.3156</td>

   <td width="111">4.1378</td>

  </tr>

  <tr>

   <td width="46">2020</td>

   <td width="45">1</td>

   <td width="111">7.8368</td>

   <td width="111">0.9990</td>

  </tr>

  <tr>

   <td width="46">2020</td>

   <td width="45">2</td>

   <td width="111">6.3289</td>

   <td width="111">3.1054</td>

  </tr>

  <tr>

   <td width="46">2020</td>

   <td width="45">3</td>

   <td width="111">7.3842</td>

   <td width="111">3.7168</td>

  </tr>

  <tr>

   <td width="46">2020</td>

   <td width="45">4</td>

   <td width="111">11.5621</td>

   <td width="111">7.1426</td>

  </tr>

 </tbody>

</table>

<ul>

 <li>List the day, month and year (in separate columns) of all days whose daily average temperature (see previous question) was lower than the daily average temperature of <strong>each </strong>of the previous 28 days in the dataset. The result should not list any of the first 28 days in the dataset, since the metric cannot be computed for those days, but the data for those days should be used to compute the rest of the result. Hint: You may want to use both the min() and count() aggregation functions in combination with an over() clause that includes both partitioning and windowing.</li>

</ul>

<table width="165">

 <tbody>

  <tr>

   <td colspan="3" width="165">Expected Query Result</td>

  </tr>

  <tr>

   <td width="46">year</td>

   <td width="45">month</td>

   <td width="75">day</td>

  </tr>

  <tr>

   <td width="46">2019</td>

   <td width="45">8</td>

   <td width="75">21</td>

  </tr>

  <tr>

   <td width="46">2019</td>

   <td width="45">8</td>

   <td width="75">23</td>

  </tr>

  <tr>

   <td width="46">2019</td>

   <td width="45">9</td>

   <td width="75">12</td>

  </tr>

  <tr>

   <td width="46">2019</td>

   <td width="45">9</td>

   <td width="75">14</td>

  </tr>

  <tr>

   <td width="46">2019</td>

   <td width="45">9</td>

   <td width="75">15</td>

  </tr>

  <tr>

   <td width="46">2019</td>

   <td width="45">9</td>

   <td width="75">16</td>

  </tr>

  <tr>

   <td width="46">2019</td>

   <td width="45">9</td>

   <td width="75">17</td>

  </tr>

  <tr>

   <td width="46">2019</td>

   <td width="45">9</td>

   <td width="75">23</td>

  </tr>

  <tr>

   <td width="46">2019</td>

   <td width="45">9</td>

   <td width="75">27</td>

  </tr>

  <tr>

   <td width="46">2019</td>

   <td width="45">9</td>

   <td width="75">30</td>

  </tr>

  <tr>

   <td width="46">2019</td>

   <td width="45">10</td>

   <td width="75">1</td>

  </tr>

  <tr>

   <td width="46">2019</td>

   <td width="45">10</td>

   <td width="75">8</td>

  </tr>

  <tr>

   <td width="46">2019</td>

   <td width="45">10</td>

   <td width="75">9</td>

  </tr>

  <tr>

   <td width="46">2019</td>

   <td width="45">10</td>

   <td width="75">10</td>

  </tr>

  <tr>

   <td width="46">2019</td>

   <td width="45">10</td>

   <td width="75">28</td>

  </tr>

  <tr>

   <td width="46">2019</td>

   <td width="45">10</td>

   <td width="75">29</td>

  </tr>

  <tr>

   <td width="46">2019</td>

   <td width="45">10</td>

   <td width="75">30</td>

  </tr>

  <tr>

   <td width="46">2019</td>

   <td width="45">11</td>

   <td width="75">26</td>

  </tr>

  <tr>

   <td width="46">2019</td>

   <td width="45">11</td>

   <td width="75">28</td>

  </tr>

  <tr>

   <td width="46">2019</td>

   <td width="45">11</td>

   <td width="75">29</td>

  </tr>

  <tr>

   <td width="46">2020</td>

   <td width="45">1</td>

   <td width="75">9</td>

  </tr>

  <tr>

   <td width="46">2020</td>

   <td width="45">1</td>

   <td width="75">12</td>

  </tr>

  <tr>

   <td width="46">2020</td>

   <td width="45">1</td>

   <td width="75">13</td>

  </tr>

  <tr>

   <td width="46">2020</td>

   <td width="45">1</td>

   <td width="75">14</td>

  </tr>

  <tr>

   <td width="46">2020</td>

   <td width="45">3</td>

   <td width="75">14</td>

  </tr>

 </tbody>

</table>

<a href="#_ftnref1" name="_ftn1">[1]</a> . A duration which is exactly five minutes longer is still considered late.
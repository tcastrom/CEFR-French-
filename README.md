# CEFR-French-
This repository contains a ML model to recognise the difficulty of a french text or sentence based on the CEFR benchmark. (i.e from A1 to C2)
<style type="text/css">
#T_f4a83 thead th {
  background-color: grey;
  color: black;
  font-weight: bold;
}
#T_f4a83 tbody tr:nth-child(even) {
  background-color: #f2f2f2;
  color: black;
  font-weight: bold;
}
#T_f4a83 tbody tr:nth-child(odd) {
  background-color: white;
  color: black;
  font-weight: bold;
}
#T_f4a83_row0_col0, #T_f4a83_row0_col1, #T_f4a83_row0_col2, #T_f4a83_row0_col3, #T_f4a83_row0_col4, #T_f4a83_row1_col0, #T_f4a83_row1_col1, #T_f4a83_row1_col2, #T_f4a83_row1_col3, #T_f4a83_row1_col4, #T_f4a83_row2_col0, #T_f4a83_row2_col1, #T_f4a83_row2_col2, #T_f4a83_row2_col3, #T_f4a83_row2_col4, #T_f4a83_row3_col0, #T_f4a83_row3_col1, #T_f4a83_row3_col2, #T_f4a83_row3_col3, #T_f4a83_row3_col4, #T_f4a83_row4_col0, #T_f4a83_row4_col1, #T_f4a83_row4_col2, #T_f4a83_row4_col3, #T_f4a83_row4_col4, #T_f4a83_row5_col0, #T_f4a83_row5_col1, #T_f4a83_row5_col2, #T_f4a83_row5_col3, #T_f4a83_row5_col4, #T_f4a83_row6_col0, #T_f4a83_row6_col1, #T_f4a83_row6_col2, #T_f4a83_row6_col3, #T_f4a83_row6_col4, #T_f4a83_row7_col0, #T_f4a83_row7_col1, #T_f4a83_row7_col2, #T_f4a83_row7_col3, #T_f4a83_row7_col4, #T_f4a83_row8_col0, #T_f4a83_row8_col1, #T_f4a83_row8_col2, #T_f4a83_row8_col3, #T_f4a83_row8_col4, #T_f4a83_row9_col0, #T_f4a83_row9_col1, #T_f4a83_row9_col2, #T_f4a83_row9_col3, #T_f4a83_row9_col4, #T_f4a83_row10_col0, #T_f4a83_row10_col1, #T_f4a83_row10_col2, #T_f4a83_row10_col3, #T_f4a83_row10_col4 {
  text-align: center;
}
</style>
<table id="T_f4a83">
  <caption>Model Performance Comparison</caption>
  <thead>
    <tr>
      <th class="blank level0" >&nbsp;</th>
      <th id="T_f4a83_level0_col0" class="col_heading level0 col0" >Model</th>
      <th id="T_f4a83_level0_col1" class="col_heading level0 col1" >Accuracy</th>
      <th id="T_f4a83_level0_col2" class="col_heading level0 col2" >Precision</th>
      <th id="T_f4a83_level0_col3" class="col_heading level0 col3" >Recall</th>
      <th id="T_f4a83_level0_col4" class="col_heading level0 col4" >F1 Score</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th id="T_f4a83_level0_row0" class="row_heading level0 row0" >0</th>
      <td id="T_f4a83_row0_col0" class="data row0 col0" >Linear Regression</td>
      <td id="T_f4a83_row0_col1" class="data row0 col1" >0.26</td>
      <td id="T_f4a83_row0_col2" class="data row0 col2" >0.25</td>
      <td id="T_f4a83_row0_col3" class="data row0 col3" >0.26</td>
      <td id="T_f4a83_row0_col4" class="data row0 col4" >0.25</td>
    </tr>
    <tr>
      <th id="T_f4a83_level0_row1" class="row_heading level0 row1" >1</th>
      <td id="T_f4a83_row1_col0" class="data row1 col0" >Logistic Regression</td>
      <td id="T_f4a83_row1_col1" class="data row1 col1" >0.47</td>
      <td id="T_f4a83_row1_col2" class="data row1 col2" >0.47</td>
      <td id="T_f4a83_row1_col3" class="data row1 col3" >0.47</td>
      <td id="T_f4a83_row1_col4" class="data row1 col4" >0.47</td>
    </tr>
    <tr>
      <th id="T_f4a83_level0_row2" class="row_heading level0 row2" >2</th>
      <td id="T_f4a83_row2_col0" class="data row2 col0" >K-Nearest Neighbors</td>
      <td id="T_f4a83_row2_col1" class="data row2 col1" >0.36</td>
      <td id="T_f4a83_row2_col2" class="data row2 col2" >0.4</td>
      <td id="T_f4a83_row2_col3" class="data row2 col3" >0.36</td>
      <td id="T_f4a83_row2_col4" class="data row2 col4" >0.35</td>
    </tr>
    <tr>
      <th id="T_f4a83_level0_row3" class="row_heading level0 row3" >3</th>
      <td id="T_f4a83_row3_col0" class="data row3 col0" >Decision Tree</td>
      <td id="T_f4a83_row3_col1" class="data row3 col1" >0.22</td>
      <td id="T_f4a83_row3_col2" class="data row3 col2" >0.24</td>
      <td id="T_f4a83_row3_col3" class="data row3 col3" >0.22</td>
      <td id="T_f4a83_row3_col4" class="data row3 col4" >0.16</td>
    </tr>
    <tr>
      <th id="T_f4a83_level0_row4" class="row_heading level0 row4" >4</th>
      <td id="T_f4a83_row4_col0" class="data row4 col0" >Random Forest</td>
      <td id="T_f4a83_row4_col1" class="data row4 col1" >0.38</td>
      <td id="T_f4a83_row4_col2" class="data row4 col2" >0.37</td>
      <td id="T_f4a83_row4_col3" class="data row4 col3" >0.38</td>
      <td id="T_f4a83_row4_col4" class="data row4 col4" >0.34</td>
    </tr>
    <tr>
      <th id="T_f4a83_level0_row5" class="row_heading level0 row5" >5</th>
      <td id="T_f4a83_row5_col0" class="data row5 col0" >Support Vector Machine</td>
      <td id="T_f4a83_row5_col1" class="data row5 col1" >0.48</td>
      <td id="T_f4a83_row5_col2" class="data row5 col2" >0.48</td>
      <td id="T_f4a83_row5_col3" class="data row5 col3" >0.48</td>
      <td id="T_f4a83_row5_col4" class="data row5 col4" >0.48</td>
    </tr>
    <tr>
      <th id="T_f4a83_level0_row6" class="row_heading level0 row6" >6</th>
      <td id="T_f4a83_row6_col0" class="data row6 col0" >Naive Bayes</td>
      <td id="T_f4a83_row6_col1" class="data row6 col1" >0.45</td>
      <td id="T_f4a83_row6_col2" class="data row6 col2" >0.47</td>
      <td id="T_f4a83_row6_col3" class="data row6 col3" >0.45</td>
      <td id="T_f4a83_row6_col4" class="data row6 col4" >0.45</td>
    </tr>
    <tr>
      <th id="T_f4a83_level0_row7" class="row_heading level0 row7" >7</th>
      <td id="T_f4a83_row7_col0" class="data row7 col0" >Stochastic Gradient Descent</td>
      <td id="T_f4a83_row7_col1" class="data row7 col1" >0.46</td>
      <td id="T_f4a83_row7_col2" class="data row7 col2" >0.46</td>
      <td id="T_f4a83_row7_col3" class="data row7 col3" >0.46</td>
      <td id="T_f4a83_row7_col4" class="data row7 col4" >0.45</td>
    </tr>
    <tr>
      <th id="T_f4a83_level0_row8" class="row_heading level0 row8" >8</th>
      <td id="T_f4a83_row8_col0" class="data row8 col0" >Gradient Boosting</td>
      <td id="T_f4a83_row8_col1" class="data row8 col1" >0.44</td>
      <td id="T_f4a83_row8_col2" class="data row8 col2" >0.44</td>
      <td id="T_f4a83_row8_col3" class="data row8 col3" >0.44</td>
      <td id="T_f4a83_row8_col4" class="data row8 col4" >0.43</td>
    </tr>
    <tr>
      <th id="T_f4a83_level0_row9" class="row_heading level0 row9" >9</th>
      <td id="T_f4a83_row9_col0" class="data row9 col0" >AdaBoost</td>
      <td id="T_f4a83_row9_col1" class="data row9 col1" >0.35</td>
      <td id="T_f4a83_row9_col2" class="data row9 col2" >0.36</td>
      <td id="T_f4a83_row9_col3" class="data row9 col3" >0.35</td>
      <td id="T_f4a83_row9_col4" class="data row9 col4" >0.35</td>
    </tr>
    <tr>
      <th id="T_f4a83_level0_row10" class="row_heading level0 row10" >10</th>
      <td id="T_f4a83_row10_col0" class="data row10 col0" >Quadratic Discriminant Analysis</td>
      <td id="T_f4a83_row10_col1" class="data row10 col1" >0.17</td>
      <td id="T_f4a83_row10_col2" class="data row10 col2" >0.2</td>
      <td id="T_f4a83_row10_col3" class="data row10 col3" >0.17</td>
      <td id="T_f4a83_row10_col4" class="data row10 col4" >0.15</td>
    </tr>
  </tbody>
</table>

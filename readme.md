# Covid-19 Time-Series Analysis
#### Study By
#### JD Kim - Muriel Kosaka -  Gabe Arnold



<h3> Understanding Our Data </h3>
<center> ===================================================== </center>

<center> ![COVID-19 Cases](./assets/graphs/overall_cases.png) </center>

<p> Our dataset was collected from *[JHU GitHub](https://github.com/CSSEGISandData/COVID-19/tree/master/csse_covid_19_data)*. It contains up to date information regarding the latest COVID-19 counts. Data includes international locations, as well as updated data from the United States.
</p>


<p>
Since the beginnning of the year COVID-19 has spread across America. The first case in the United States was recorded in January 2020. As of July 30, millions have been infected, and over 150,000 people have died from the virus.
</p>

<p>
Our goal is to build a model to project death rates for cities in America. After and see if certain actions can be made to decrease the rate of the curve.
</p>


<h3>Models Used</h3>
<center> ===================================================== <center>
    
<ul>
    <li>ARMA</li>    
    <li>ARIMA</li>
    <li>SARIMAX</li>
</ul>

<h6>Final Model</h6>

<p>The final model selected was SARIMAX model. The RMSE Score for the National Cases Confirmed model was 15,325. The RMSE Score for the National Death Model was 487.</p>


<h3>Findings</h3>

<h6>Confirmed Cases </h6>
<p>We are seeing that highly populated areas were hit extremely hard. We believe that it is a result of the dense population and high transmission rate. </p>

<p>New York City and Cook County (Chicago), had large jumps in the number of people that were initially infected, during the lockdown phase however data shows a smoothing in the recent rate of cases after reopening. It should also be noted that both of these cities instituted a lockdown relatively early and longer in the US.</p>

![New York City Confirmed Cases](./assets/graphs/nyc_confirmed.png)


![Cook County Chicago Confirmed Cases](./assets/graphs/chicago_confimed.png)
    
<p>Recently, the cities of Los Angeles, Harris County Texas (Dallas), and Maricopa (Phoenix), have seen large increases in the number of people that have recently contracted the disease. Los Angeles, even though they instituted a longer lockdown, has faced a rapid increase in the number of confirmed cases. We noticed that Harris County Texas and Maricopa had shorter lockdown periods and a rapid increase in cases after reopening.</p>


<p>Additionally, we noticed in median populated (~12000 People) regions, that had shorter lockdown periods are experiencing high rates of contact.</p>

<p>In areas with small populations (U+003C1000 People) face small amounts of Contamination Cases.</p>

<p>In large (>4000000) and median populated regions generally saw a spike after the Fourth of July.</p>

<h6>Death Cases</h6>
<p>Death cases were similar to confirmed cases. Large metropolitans that were hit early experienced very high death rates. As we transition to overall state data, we can see New York, California, and Massachusetts are all leading the nation in COVID-19 deaths. 
    
![US Death Count](./assets/graphs/top_10_states.png)
<a href="https://covid19dataproject.org/">
    <img src="https://covid19dataproject.org/wp-content/uploads/2020/04/LOGO-Broadstreet-covid19.svg" alt="Broadstreet logo" title="BroadStreet" align="right" height="80" />
</a>

Broadstreet COVID-19 Data Project
=================================

## Daily Numbers

We created the [Covid-19 Data Project](https://covid19dataproject.org/data/) in March to satisfy the driving need for accessible data tracking the spread of the coronavirus across the United States. In response to this public health emergency, BroadStreet is releasing data files with cumulative counts of coronavirus cases and mortalities in the United States and their territories, at the county level, from January 20th, 2020 to present. Over 120 interns and volunteers were recruited via the BroadStreet website, and through institutional reference for interested undergraduate or graduate students. The project quickly grew as the virus spread, leading to a large data set involving historical and present data collection, input, and analysis. The data team tracked daily numbers of deaths and cases throughout the entire United States at the county level. 

The BroadStreet COVID-19 Data Project data is unique in that data is updated/corrected by quality assurance reviews in days, weeks and months following initial entry. We feel this will provide an alternate method of collecting COVID-19 data and an alternate historical snapshot.  This data allows individuals to visualize the pandemic impact on counties, states and the United States. This data, including daily case totals from the first known case of the virus, gives the public access to knowledge regarding the rate of transmission and spread of the virus. We will be releasing monthly updates to this dataset.
  
## Structure of the Dataset  
  
The data is structured in wide form. This is how the first case in the United States would be represented at the county level for January 20, 2020: 05000US53061, Snohomish County Washington, WA, 1, 0, 0, 0. This is how the first case would be represented at the state level: 04000US53, Washington (state), WA, 1, 0. Both the county and state data begins with the state identification number/county identification number, followed by the state/county. At the county level, the data recorded are first confirmed positive cases, followed by the number of probable positive cases, the number of confirmed deaths, then the number of probable deaths. At the state level, the data recorded are total number of cases, followed by the total number of deaths.

Variables used in our data include:  
<ul>
<li>tstpos_ : The number of confirmed cases</li>  
<li>pbpos_ : The number of probable cases</li>  
<li>mort_ : The number of confirmed deaths</li>  
<li>pbmort_ : The number of probable deaths</li>  
<li>Unknown: Cases and deaths within each state that do not neatly fit into a geographic code. These are most often cases which are still being investigated to determine their county of residence</li>  
</ul>

## Methodology

All data prior to March 9th was entered from Johns Hopkins University. Data between March 9th to March 16th was entered historically from various county health departments, state health departments, and local news sources obtaining information from health departments or local officials.. 

Beginning on March 16, 2020, the BroadStreet team (consisting of approximately 120 volunteers) began tracking confirmed cumulative case and death totals. Volunteers were organized into regional groups consisting of a data entry team, and a quality assurance team. Each team was supervised by a designated lead who ensured data was entered completely and in a timely manner.

Data entry team members enter data from state or county health departments each day onto a shared google sheet. Team leads would then do a first check to ensure data was filled in completely, and matched reported state totals. Quality assurance team members then compared what was entered into our dataset with the totals reported by our comparison sets: Johns Hopkins University, the New York Times, and USAFacts. These were used to identify potential errors. If the value entered in any county was inconsistent with what these comparison sets reported, quality assurance team members would research the case or death totals in that county to determine which value was correct, then leave a comment on the relevant cell with the results of their research.
Cumulative totals should, by definition, be constantly trending upwards. In any instance where the case or death totals decreased from the previous day we investigated the cause of the revision and corrected historic data accordingly. Health departments frequently do not report the information needed to correct these “trend breaks.”

## Changes in Process

During early months, we found that there were often multiple reliable sources reporting conflicting case totals in many counties. The most frequent source of disagreement was between county health departments and state health departments. There are several potential causes for this: they may be using different criteria to report cases, such as one source including probable cases or prisoners where the other does not. The difference between the two is most commonly affected by the path that information surrounding a case takes in that particular state. If the state is being notified of cases by each individual county health department, there may be a delay in the state’s ability to report these cases as it processes new reports.

Quality assurance team members would regularly check multiple reliable sources and use the highest case total reported for that day. As the virus spread and more counties began reporting cases, checking multiple sources for each county became an untenable strategy. In late June, we began choosing designated sources to enter data from in each county to simplify this process. [More details on specific sources can be found here](https://docs.google.com/spreadsheets/d/14Id9avOoss4fLMr8YjrBAUShOtycvovxWAinq4wxSuA/edit?usp=sharing).

On 4/16/20, we began including probable cases in our data wherever they are reported. [This is consistent with CDC interim guidelines published on 4/5/20](https://wwwn.cdc.gov/nndss/conditions/coronavirus-disease-2019-covid-19/case-definition/2020/08/05/).

On 7/27/20, we began separating probable cases and deaths from confirmed cases and deaths in our data. Prior to this, we had been including them in the same figure. In some states, these cases are not possible to separate due to the health department reporting only the total cases.

On 9/4/20, the [CDC published a guideline](https://www.cdc.gov/coronavirus/2019-ncov/lab/resources/antigen-tests-guidelines.html) for use of rapid antigen test, stating they are a valuable tool for screening for the presence of COVID-19 and can be useful as a diagnostic tool if properly interpreted by clinicians. Some states have since begun including individuals testing positive via rapid antigen tests in either their confirmed or probable case totals. These are included in our data where reported.

## Date of Case Inclusion

Case and death totals are typically included in our data on the date they were reported. This does not always result in an accurate picture of how the virus is spreading as a function of time. It may take days or longer for a case to be reflected in reported totals,  due to the time it may take someone to be tested after they become ill or delays in processing test results. Several states include the date of symptom onset or date of death in their reports; where possible, we include cases and deaths based on these criteria to provide a more accurate epidemiologic curve.

<ul>
<li>Georgia: Reports cases by date of symptom onset, and deaths by date of death. Both are used in our data.</li>
<li>Tennessee: Reports total cases by date of symptom onset. This is used in our data.</li>
<li>Ohio: Reports cases by date of symptom onset, and deaths by date of death. Both is used in our data.</li>
<li>Indiana: Reports cases by date of symptom onset, and deaths by date of death. Both are used in our data.</li>
<li>Michigan: Reports cases by date of symptom onset, and deaths by date of death. Both are used in our data.</li>
<li>Wisconsin: Reports cases by date of symptom onset, and deaths by date of death. Both are used in our data.</li>
<li>Oklahoma: Reports cases by date of symptom onset. This is used in our data.</li>
<li>Kansas: Reports cases by date of diagnosis. This is used in our data.</li>
<li>Oregon: Reports deaths by date of death. Reports statewide case totals by date of symptom onset. Both are used in our data.</li>
<li>Washington: Reports cases by date of symptom onset, and deaths by date of death. Both are used in our data.</li>
</ul>

## Geographic Exceptions

<ul>
<li>Massachusetts: Duke and Nantucket county totals were included together until 8/19</li>
<li>New Hampshire: Manchester and Nashua county totals are included in Hillsborough county</li>
<li>New York: We do not record data for the individual boroughs of New York CIty, and instead record all data in the New York City totals</li>
<li>Michigan: Detroit City is included within Wayne County totals</li>
<li>Missouri: Joplin City totals are included within Jasper County totals</li>
<li>Missouri: Kansas City totals are included within Jackson County totals</li>
<li>Utah: Cases from the Ute tribe are entered into the unknown row</li>
<li>Nevada: Cases from the Shoshone tribe are entered into the unknown row</li>
<li>Puerto Rico: All deaths are entered into the unknown row</li>
</ul>

## Attributions

All data in California after 3/16/20 was gathered from reports in the Los Angeles Times. Their organization has been diligently tracking the spread of COVID-19 by accessing every county health department in the state. 
https://www.latimes.com/projects/california-coronavirus-cases-tracking-outbreak/

## Suggested Citation
When using data images, downloaded data, or shared document formats, please attribute BroadStreet as well as the original source, when applicable. For examples and more information, review this article which answers the question ["How do I cite BroadStreet?"](https://help.broadstreet.io/article/citations/)



## Contributors
Tom Schmitt, PhD, Tracy Flood, MD PhD, Zach Sturgeon, Samin Charepoo, April Miller, Cedonia Thomas, Grace Gibbon.
A full list of the Broadstreet Covid-19 Data Project volunteers can be found here: https://covid19dataproject.org/team-2/



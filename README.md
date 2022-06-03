# bank
<img src='img/bank.png' width='100'>
# Information
<div style="background-color:lightgrey;">
The data is related with direct marketing campaigns of a Portuguese banking institution. 
The marketing campaigns were based on phone calls. Often, more than one contact to the same client was required, 
in order to access if the product (bank term deposit) would be (or not) subscribed.
</div>
<p></p>
<div style='background-color:lightgreen;'>Goal: Given certain user data, we can predict if it would subscribe to the bank term deposit and create a graphical interface to ease prediction.</div>

Input variables:
## bank client data:
   <div>
    <ol>
       <li><strong>age (numeric)</strong> </li>
       <li><strong>job</strong> : type of job(categorical:"admin.","unknown","unemployed","management","housemaid","entrepreneur","student",
                                       "blue-collar","self-employed","retired","technician","services")</li> 
       <li><strong>marital</strong> : marital status (categorical: "married","divorced","single"; note: "divorced" means divorced or widowed)
       <li><strong>education</strong> (categorical: "unknown","secondary","primary","tertiary")</li>
       <li><strong>default</strong>: has credit in default? (binary: "yes","no")</li>
       <li><strong>balance</strong>: average yearly balance, in euros (numeric) </li>
       <li><strong>housing</strong>: has housing loan? (binary: "yes","no")</li>
       <li><strong>loan</strong>: has personal loan? (binary: "yes","no")</li>
    </ol>
   </div>
   
   ## related with the last contact of the current campaign:
   <ol>
      <li><strong>contact</strong>: contact communication type (categorical: "unknown","telephone","cellular")</li> 
      <li><strong>day</strong>: last contact day of the month (numeric)</li>
      <li><strong>month</strong>: last contact month of year (categorical: "jan", "feb", "mar", ..., "nov", "dec")</li>
      <li><strong>duration</strong>: last contact duration, in seconds (numeric)</li>
    </ol>
    
   ## other attributes:
   
   <ol>
      <li><strong>campaign</strong>: number of contacts performed during this campaign and for this client (numeric, includes last contact)</li>
      <li><strong>pdays</strong>: number of days that passed by after the client was last contacted from a previous campaign (numeric, -1 means client was not previously contacted)</li>
      <li><strong>previous</strong>: number of contacts performed before this campaign and for this client (numeric)</li>
      <li><strong>poutcome</strong>: outcome of the previous marketing campaign (categorical: "unknown","other","failure","success")</li>
</ol>
  Output variable (desired target):
  <ol>
      <li><strong>y</strong> - has the client subscribed a term deposit? (binary: "yes","no")</li>
  </ol>

  <div>Prediction sample:</div>
  <img src='img/prediction example.png' width='500'>
  

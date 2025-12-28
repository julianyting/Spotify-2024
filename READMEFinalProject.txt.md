### Personal Info

* Eric Villanueva, Jamie Ann Visconde, Julian Ting, Kristen Ng  
* [krng@chapman.edu](mailto:krng@chapman.edu), [jting@chapman.edu](mailto:jting@chapman.edu), [ervillanueva@chapman.edu](mailto:ervillanueva@chapman.edu), [visconde@chapman.edu](mailto:visconde@chapman.edu)  
* CPSC392-03  
* Final Project Part 3 Perform Analysis

### A description of any known compile or runtime errors, code limitations, or deviations from the assignment specifications

N/A

### A list of all references used to complete the assignment, including peers

AI: What prompt did you ask?

* how to fix value error with the commas in the numbers  
    
* how to model the different metrics MSE, MAE, and R2 on the same line chart

What output from the LLM did you use?

* for column in continuous: x\[column\] \= x\[column\].astype(str).str.replace(',', '').astype(float)

y \= pd.to\_numeric(y.astype(str).str.replace(',', '', regex=True))

* metrics \= { 'R²': { 'Train': \[ r2\_score(y\_train, y\_pred\_train\_p2), r2\_score(y\_train, y\_pred\_train\_p3), r2\_score(y\_train, y\_pred\_train\_p4) \], 'Test': \[ r2\_score(y\_test, y\_pred\_p2), r2\_score(y\_test, y\_pred\_p3), r2\_score(y\_test, y\_pred\_p4) \] }, 'MSE': { 'Train': \[ mean\_squared\_error(y\_train, y\_pred\_train\_p2), mean\_squared\_error(y\_train, y\_pred\_train\_p3), mean\_squared\_error(y\_train, y\_pred\_train\_p4) \], 'Test': \[ mean\_squared\_error(y\_test, y\_pred\_p2), mean\_squared\_error(y\_test, y\_pred\_p3), mean\_squared\_error(y\_test, y\_pred\_p4) \] }, 'MAE': { 'Train': \[ mean\_absolute\_error(y\_train, y\_pred\_train\_p2), mean\_absolute\_error(y\_train, y\_pred\_train\_p3), mean\_absolute\_error(y\_train, y\_pred\_train\_p4) \], 'Test': \[ mean\_absolute\_error(y\_test, y\_pred\_p2), mean\_absolute\_error(y\_test, y\_pred\_p3), mean\_absolute\_error(y\_test, y\_pred\_p4)\]}}


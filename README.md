##Data Science Challenge

We've randomly sampled click stream data from 10,000 sessions from a major client. The data set contains a record for each of the page views that correspond to the sessions.

When the sessions started they were assigned to the test or the control group. This is given as parameter "G" in the page views. G=0 indicates that the session is a *test group* session, while G=1 corresponds to the *control group*.

Regardless of the assigned group, a prediction model was used ad-hoc to decide at each of the pageviews whether or not to display incentives. If the decision was taken to show an incentive, the page view has a flag "md" (e. g. session 53844cf830fde21446e1757b). However, the incentive was only actually shown if the session was initially assigned to the test group.

If the visitor bought anything, there is a page view with the "C" parameter set to "checkout" in the session and the "o" specifies the order total.

The corresponding session ID is stored in the field "S" in each record. The timestamp is specified by the "t" parameter (in ms since 1970-01-01). The parameter "I" corresponds to the cookie ID, while "K" is the shop token (constant in this dataset).

You can confirm you read the dataset correctly with this information: the test group revenue is r_t = 32211.62 and the control group revenue is r_c = 9362.55.

##Task

Create a prediction model that will lead to an increase in shop revenue by deciding whether or not to display an incentive to the shop visitor on a page view basis.

1. read the data with your programming language of choice and write code that will train a prediction model that will decide on a page view basis (with knowledge of the previous page views) when to display an incentive to the visitor. (~3 hrs)

 Note: in your choice of algorithms, you may of course assume that your dataset doesn't contain just 10,000 but 1,000,000+ sessions

2. Describe how you would evaluate the performance of it. (~ 0.5hrs)

3. Imagine your prediction model went live to actually target online-shop visitors of our customers. How can you make sure you will continuously improve the prediction model? (~ 0.5hrs)

##Data

JSON file, each line represents a single page view.

##Answers

Please solve the first task using your programming language of choice and include the source code in your solution. Put remarks and explanation in comments.


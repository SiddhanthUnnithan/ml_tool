# ml_tool
Web application used to conduct preliminary regression or classification on
arbitrary data set.

## Inspiration:
After going through Kaggle competitions, I noticed that there was
a similar set of preprocessing, feature extraction/selection, and estimation
steps taken to get to a first round of regression or classification.

I wanted to create a simple tool that allows the user to pass a training set, 
and receive an analysis of the set (e.g. strongly correlated features, best 
performing estimators, important categorical and continuous features).

The first version of the tool should allow users to upload a csv file
containing training data. Users can either segment features based on whether
they're categorical or continuous, or allow the tool to auto-segment
(assuming feature types are specified correctly). The only mandatory
specifications are the unique identifier and target columns.

The user should also be able to input a test set for which the newly 
learn model would provide a prediction. If users are handled properly by
the application they should be allowed to re-run their model against new
test sets (i.e. through the use of local pickles); this re-running makes most
sense with document-classification models.

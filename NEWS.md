# AccelStab 2.1.0

This is a major release adding new functionality, adjusting the data sets and documentation.

## New features

-   `step1_down_basic()` This new function allows for rapid testing of the fit without 
    all of the features.

-   `antigenicity` Changed example data and added a validation column.

-   `step1_down()` Adjusted the help page and added validation options to the examples.
    The function will now also return sampled parameters, reducing the need for the 
    step1_sample_mvt function.

-   `step1_plot_diagnostic()` Added argument to use either classic, standardized or 
    studentized residuals.


# AccelStab 2.0.2

This release has a minor bug fix and additional descriptions added.

## Bug fixes

-   `step1_sample_mvt()` Fixed issue when no values at time point zero

-   `potency.rda` File data adjusted slightly

-   `step1_down()` Added to some arguments' description and new print 
    when any of the k3 draws are below zero.


# AccelStab 2.0.0

This is a major release adding a few new functions and fixing a bug.

## New features

-   `step1_down_rmse()` added which allows the user to calculate the
    root mean squared error for their data and chosen parameters

-   `step1_down_diagnostic()` added which allows the user to plot
    residual diagnostic plots after fitting the model

-   `step1_sample_mvt()` added which allows the user to draw a chosen
    number of sample parameters from the multivariate t distribution for
    their own analyses
    
-   `step1_down()` now accepts an extra argument `validation` which
    sidelines some of the data allowing the user to save it for testing
    purposes

-   `step1_plot_desc()` now accepts an extra argument `validation` which
    sidelines some of the data allowing the user to save it for testing
    purposes

## Bug fixes

-   When selecting a temperature outside the data set for
    `step1_plot_T()` the colours of the prediction line and the ribbon
    are now consistent
-   When using the argument `temp_pred_C` within `step1_down()` no longer
    are predictions duplicated if the temperature is already in the data
-   Issue when no time = 0 rows present in the data and no `parms` provided
    to `step1_down()` now resolved

# AccelStab 1.0.0

-   Added a `NEWS.md` file to track changes to the package.

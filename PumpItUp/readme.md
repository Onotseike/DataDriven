# Problem Description

    This is where you'll find all of the documentation about this dataset and the problem we are trying to solve. For this competition, there are three subsections to the problem description:

## The Features in this Dataset

    Your goal is to predict the operating condition of a waterpoint for each record in the dataset. You are provided the following set of information about the waterpoints:
    
    * amount_tsh - Total static head (amount water available to waterpoint)
    * date_recorded - The date the row was entered
    * funder - Who funded the well
    * gps_height - Altitude of the well
    * installer - Organization that installed the well
    * longitude - GPS coordinate
    * latitude - GPS coordinate
    * wpt_name - Name of the waterpoint if there is one
    * num_private - 
    * basin - Geographic water basin
    * subvillage - Geographic location
    * region - Geographic location
    * region_code - Geographic location (coded)
    * district_code - Geographic location (coded)
    * lga - Geographic location
    * ward - Geographic location
    * population - Population around the well
    * public_meeting - True/False
    * recorded_by - Group entering this row of data
    * scheme_management - Who operates the waterpoint
    * scheme_name - Who operates the waterpoint
    * permit - If the waterpoint is permitted
    * construction_year - Year the waterpoint was constructed
    * extraction_type - The kind of extraction the waterpoint uses
    * extraction_type_group - The kind of extraction the waterpoint uses
    * extraction_type_class - The kind of extraction the waterpoint uses
    * management - How the waterpoint is managed
    * management_group - How the waterpoint is managed
    * payment - What the water costs
    * payment_type - What the water costs
    * water_quality - The quality of the water
    * quality_group - The quality of the water
    * quantity - The quantity of water
    * quantity_group - The quantity of water
    * source - The source of the water
    * source_type - The source of the water
    * source_class - The source of the water
    * waterpoint_type - The kind of waterpoint
    * waterpoint_type_group - The kind of waterpoint

## The Labels in this dataset
    The labels in this dataset are simple. There are three possible values:

    *   functional - the waterpoint is operational and there are no repairs needed
    *   functional needs repair - the waterpoint is operational, but needs repairs
    *   non functional - the waterpoint is not operational

## Submission Format
    The format for the submission file is simply the row id and the predicted label (for an example, see SubmissionFormat.csv on the data download page.

        For example, if you just predicted that all the waterpoints were functional you would have the following predictions:
        id      status_group
        50785	functional
        51630	functional
        17168	functional
        45559	functional
        49871	functional
    
    Your .csv file that you submit would look like:

        id,status_group
        50785,functional
        51630,functional
        17168,functional
        45559,functional
...
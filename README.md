# SampleDataStreamflow

This repository contains sample data for streamflow modeling.
Data for two regions is provided: Ohio and Missouri.

File Structure:
```
- [Ohio](Ohio/) or [Missouri](Missouri/)  
    Directories containing data for the respective regions.

    - `attributes_meta.csv`  
        Metadata for the locations in the study region, including Name, Latitude, Longitude, and Area.

    - `attributes_simple.csv`  
        Set of static attributes derived from past climate data.

    - `attributes_detailed.csv`  
        Set of detailed attributes derived from the HydroATLAS dataset.

    - `Output_Streamflow/`  
        Contains streamflow data for each gauge in the region.  
        - `{gauge_id}.csv`  
            Streamflow data with shape `[Time, 1]`, representing one output variable. Missing values may be present.

    - `Input_Timeseries/`  
        Contains input time series data for each gauge in the region.  
        - `{gauge_id}.csv`  
            Input time series data with shape `[Time, 15]`, representing 15 dynamic input variables.
```


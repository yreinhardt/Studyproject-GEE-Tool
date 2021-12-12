# Studyproject-GEE-Tool
GEE-Tool for timeseries analysis


## Data

**1. Selection of different Sentinel-5P Bands**

<code>Sulphur dioxide (SO2)</code> <code>SO2_column_number_density</code>

<code>Nitrogen dioxide (NO2)</code> <code>NO2_column_number_density</code>

<code>Carbon monoxide (CO)</code> <code>CO_column_number_density</code>

<code>Methane (CH4)</code> <code>CH4_column_volume_mixing_ratio_dry_air</code>

<code>Absorbing Aerosol Index (AAI)</code> <code>absorbing_aerosol_index</code>

<code>Formaldehyde (HCHO)</code> <code>tropospheric_HCHO_column_number_density</code>

<code>Ozone (O3)</code> <code>O3_column_number_density</code>

**2. Create Interval**

Interval using unit days.

If interval is not selected every possible Image between given daterange is returned as ImageCollection.

*Return:* ImageCollection

**3. Clip to Geometry**

Default clip to boundary of China.

*Optional*: Last drawn features as geometry input.

**4. Save layer**

Layer can be named. Name is used as identifier for further operations.

## Operations

**1. Spatial Statistics**

Pixelbased spatial statistics.

*Return:* single Image

Statistical measures:

<code>Arithmetic Mean(HCHO)</code> 

<code>Median</code> 

<code>Maximum</code> 

<code>Minimum</code>

**2. Calculate Difference**

Calculate difference in percentage between to single Images.

*Return:* difference Image.

### Vizualisation

**1. Timeseries**

Creates timeseries plot from one ImageCollection.

Creates timeseries plot from two Image Collections.

Selection of Layer by named required.

*Optional:* Set title, download

**2. Splitview**

Creates a Splitview with Splitviewpanel.

Select two single Images as right and left Image.

## Reclassification

**1. Timeseries**

Reclassify single Image.

6 Classes can be selected.

First class contains always values outside user given range (color = white)

Individuel selection of class ranges.

Each class has a fixed color.

*Return:* Image


## Download

Image and Feature/FeatureCollection can be downloaded as GeoTiff and Geojson.

Select Image by name.

Last drawn Feature is used for download as Geojson.

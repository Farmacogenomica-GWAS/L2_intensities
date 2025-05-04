#  L2_intensities File Processing

The `L2_intensities.hdf5` file was processed using Python, h5py, and pandas. The primary goal was to extract data and metadata from the file and convert it into a more accessible CSV format. The `L2_intensities.hdf5` file was obtained by using the Tierpsy Tracker.

**Key Steps:**

1.  **File Inspection**: The `L2_intensities.hdf5` file was inspected to identify its structure and contents, including groups and datasets.

2.  **Dataset Extraction**:
    * The following datasets were extracted and converted to individual CSV files:
        * `straighten_worm_intensity_median`
        * `trajectories_data_valid`
    * The `provenance_tracking` group, which contains metadata attributes, was extracted and written to a single-row CSV file.

3.  **Output Format**:
    * Extracted datasets were saved as CSV files.
    * Metadata attributes from the `provenance_tracking` group were saved as a single-row CSV file.

**Libraries Used:**

* `h5py`: For reading and navigating the HDF5 file structure.
* `pandas`: For creating and exporting DataFrames to CSV files.

**Purpose:**

The processing steps outlined above were performed to make the data contained within the `L2_intensities.hdf5` file more readily available for analysis. The conversion to CSV format allows for easier manipulation and exploration of the data using standard data analysis tools.  The provenance tracking metadata was extracted to maintain important information about the data's origin.

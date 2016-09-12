# Tax Foundation State Open Data

In an effort to both make data more available and useful to the general public, as well as to organize the various datasets we've collected, the Tax Foundation is developing standards for the recording and publication of state-level tax data. This repository details the schema for this data, as well as gives examples of its use. This schema will be used to define attributes of Tax Foundation data for use across various platforms. By using a standard format, we can keep our raw data in one centralized, version-controlled location while letting scripts format and push it to our various distribution channels.

## Overview

Inside `schema.yml` are rules defining various types of data, such as percentages (as seen in tax rates), currencies (as used in collections data), and other data types included in Tax Foundation datasets. The YAML format is used for ease of human-readability. These definitions are used to automatically error-check data and to create formatted copies for various channels in a uniform way.

Each dataset will require its own metadata file. This file will describe the contents a specific set of data. Data types in a dataset are declared and verified against regular expressions in `schema.yml` for conformity to standards.

## Example

The file `example-metadata.yml` is used to describe the data inside `example-dataset.csv`. This example covers the basics of naming and describing columns of data. The values for individual records can be programmatically checked against the regular expressions in `schema.yml` for validity. Then separate programs can be used to create versions of the raw data for consumption.

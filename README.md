# Tax Foundation State Open Data

In an effort to both make data more available and useful to the general public, as well as to organize the various datasets we've collected, the Tax Foundation is developing standards for the recording and publication of state-level tax data. This repository details the schema for this data, as well as gives examples of its use. This schema will be used to define attributes of Tax Foundation data for use across various platforms. By using a standard format, we can keep our raw data in one centralized, version-controlled location while letting scripts format and push it to our various distribution channels.

## Schema Overview

The data schema are defined at a higher level in `schema.yml`. The YAML format is used for ease of human-readability. Inside `schema.yml` are rules defining various types of data, such as percentages (as seen in tax rates), currencies (as used in collections data), and other data types included in Tax Foundation datasets. These definitions are used to automatically error-check data and to create formatted copies for various channels in a uniform way.

Each dataset will require its own metadata file. This file will describe the contents a specific set of data in terms that can be checked against `schema.yml`.
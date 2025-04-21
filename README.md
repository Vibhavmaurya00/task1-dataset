# Netflix Movies and TV Shows Dataset - Cleaned and Standardized

## Overview

This repository contains a cleaned and standardized dataset of movies and TV shows available on Netflix. The dataset has undergone several preprocessing steps in Excel to ensure consistency and quality, making it suitable for various data analysis and visualization tasks.

## Data Cleaning and Standardization Steps (Performed in Excel)

The following steps were performed on the original dataset using Microsoft Excel:

1.  **Handling Missing Values:**
    * Missing values were identified using Excel's filtering capabilities (e.g., blank cells) and the `ISBLANK()` function.
    * Depending on the column and the extent of missing data, different strategies were applied (e.g., removal of rows with critical missing information, imputation with a placeholder like "Unknown" for categorical columns where appropriate).

2.  **Removing Duplicate Rows:**
    * Duplicate rows were identified and removed using Excel's "Remove Duplicates" feature (located under the "Data" tab). This ensures that each entry in the dataset is unique.

3.  **Standardizing Text Values:**
    * Inconsistent text values within columns like "gender" and "country" were identified through manual inspection and using features like "Find and Replace" and potentially formulas (e.g., `TRIM()`, `LOWER()`, `PROPER()`).
    * These values were standardized to ensure uniformity (e.g., "Male", "Female"; consistent naming conventions for countries).

4.  **Converting Date Formats:**
    * Date columns were converted to a consistent `dd-mm-yyyy` format using Excel's "Format Cells" option and potentially the `TEXT()` function for more complex conversions. This ensures consistent date representation for analysis.

5.  **Renaming Column Headers:**
    * Column headers were renamed to be clean and uniform. This involved converting them to lowercase and replacing spaces with underscores (e.g., "Show ID" became "show\_id", "Release Year" became "release\_year"). This improves readability and ease of use in data analysis tools.

6.  **Checking and Fixing Data Types:**
    * Data types were inspected to ensure they were appropriate for the content of each column. For example, columns intended for numerical values (like age, if present in the original data) were checked to be numbers, and date columns were verified to be in a proper date format.

## Dataset Structure

The dataset contains information about Netflix titles, with the following cleaned and standardized column headers:

* `show_id`: Unique identifier for each title.
* `type`: Type of content (Movie or TV Show).
* `title`: Title of the movie or TV show.
* `director`: Director of the movie (if applicable).
* `cast`: Main cast members.
* `country`: Country of origin.
* `date_added`: Date when the title was added to Netflix (in `dd-mm-yyyy` format).
* `release_year`: Year of release.
* `rating`: TV rating or movie maturity rating.
* `duration`: Length of the movie or number of seasons for a TV show.
* `listed_in`: Genre(s) the title is listed under.
* `description`: Brief summary of the title.

## Usage

This cleaned and standardized dataset is ideal for:

* Exploratory Data Analysis (EDA) to understand trends in Netflix content.
* Building recommendation systems.
* Visualizing the distribution of content by type, genre, country, etc.
* Analyzing the growth of Netflix's content library over time.

You can download the dataset file (e.g., `netflix_cleaned.csv` or `netflix_cleaned.xlsx`) and use it with various data analysis tools and programming languages like Python (with libraries such as Pandas), R, or business intelligence platforms.


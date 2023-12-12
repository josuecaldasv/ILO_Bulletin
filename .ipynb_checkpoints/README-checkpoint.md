# ILO_Bulletin

This repository contains the code and resources needed to generate an automated bulletin for the International Labour Organization (ILO).

## Project Structure

The project is organized as follows:

- **main.py**: The main script for generating the bulletin. It dynamically creates sections based on the number of subfolders within the `data` folder, and populates each section with news items from JSON files.

- **template.html**: The HTML template that defines the layout and style of the bulletin. This file is used as a base to dynamically insert news data from each section and generate the final bulletin.

- **data/**: A folder containing subfolders, each representing a different section of the bulletin. Each subfolder contains JSON files with news data for that specific section. The structure should be as follows:
    ```
    data/
    ├── section_1/
    │   ├── news_item_1.json
    │   └── news_item_2.json
    │
    └── section_2/
        ├── news_item_3.json
        └── news_item_4.json
    ```

- **sample_bulletin.html**: The output file generated by `main.py`. It's the final HTML bulletin, ready for distribution or hosting.

## Viewing the Bulletin

The generated bulletin can be viewed online at the following URL: [ILO Bulletin](https://josuecaldasv.github.io/ILO_Bulletin/sample_bulletin.html).

This URL hosts the `sample_bulletin.html` file.

## How to Generate the Bulletin

To generate the bulletin:

1. Ensure the `data` folder is structured with subfolders for each section, containing JSON files for news items.

2. Run the `main.py` script: This script reads the news data from each subfolder in the `data` folder, applies it to the `template.html`, and generates `sample_bulletin.html`, which is the final bulletin file.

## How to Generate the bulletin

To generate the bulletin, run the `main.py` script. This script reads the news data from the `data` folder, applies it to the `template.html`, and generates `sample_bulletin.html`, which is the final bulletin file.

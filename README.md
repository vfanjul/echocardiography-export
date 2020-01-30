# echocardiography-export
Data structuring and export of echocardiography experiments

Excel template for structuring [Vevo 2100](https://www.visualsonics.com/product/imaging-systems/vevo-2100) reports. The output is a table in which each column is a parameter for each subject and experiment. This is intended for any researcher and does not require any programming habilities.

## Steps
1. Export reports as `.csv` in Vevo 2100
2. Open `VEVO table export.xlsx` and clear `report` sheet
3. Open exported `.csv` report and copy the whole page into the `report` sheet
4. Update data in `pivot table` sheet
5. Copy pivot table in a new file and erase rows and columns of no interest

## Notes
- Make sure decimal numbers are denoted by '.' and not ',' in both Excel and Vevo
- If `.csv` is incorrectly opened in Excel, import file from Excel and indicate appropriate separator (',', ';', tab...)
- If `.csv` is separated by ';', parameters such as 'LVID;d', 'LV Vol;s' may be incorrectly imported

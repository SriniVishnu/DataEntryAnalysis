##### This markdown document is about data entry analysis of three files ZOOP-TEMP, POND2010 , ZOOP-TEMP-MAIN

### PROJECT TITLE
Data Entry Analysis

### LIST OF DATA FILES IN THE DIRECTORY
1. [POND2010](https://github.com/SriniVishnu/DataEntryAnalysis/blob/master/pond2010.xlsx)
2. [ZOOPTEMP](https://github.com/SriniVishnu/DataEntryAnalysis/blob/master/zoop%20-%20temp-main.xlsx)
3. [ZOOPTEMP-MAIN](https://github.com/SriniVishnu/DataEntryAnalysis/blob/master/zoop%20-%20temp.xlsx)
4. [README.md](https://github.com/SriniVishnu/DataEntryAnalysis/blob/master/README.md)

### FILES NEWLY ADDED
1. [POND2010](https://github.com/SriniVishnu/DataEntryAnalysis/blob/master/pond2010.xlsx)
2. [ZOOPTEMP](https://github.com/SriniVishnu/DataEntryAnalysis/blob/master/zoop%20-%20temp-main.xlsx)
3. [ZOOPTEMP-MAIN](https://github.com/SriniVishnu/DataEntryAnalysis/blob/master/zoop%20-%20temp.xlsx)
4. [README.md](https://github.com/SriniVishnu/DataEntryAnalysis/blob/master/README.md)   

Note: All files are newly added.

### LAST MODIFIED
* Author/Contributor: Srinivasa Keerthy Vishnubhotla  
* Date and Time: 09/12/17 11:59 AM

### Problem Statement
The 3 files linked above were all intended to be part of the same study – the investigators wanted to examine the day-night distribution of 2 species of zooplankton across multiple years. The type of zooplankton they studied is called rotifers generally, and specifically the genus Conochilus, in which groups of individual rotifers stick together in colonies. The investigators plan to repeat this study for several more years. 

### Task 1 Problems Identification
#1: Based on class readings, prior experience, and your own good sense, list some of the problems in the way that the data are currently organized (there are at least 8 problems with these spreadsheets; try to identify as many as possible, but at least 4).
**Solution:** 
Problems identified are:

1. In the files, dates on which the samples were taken was given but the timestamp infomration is not available. This does not say wheather the sample was taken during the day or night.
2. Cuni/Chippo per Litre has negative values which is not possible. If there is any significance for it, it should be mentioned in data dictonary.
3. Colony size are in decimal form. Ceil function must be put on them.
4. No where it is mentioned what the Red and yellow highlights meant.
5. There is no units mentioned for Temperature, Depth, Density, Colony diametre.
6. No Yellow book map details for section B.
7. zoop-temp.xlsx and zoop-temp-main.xlsx  and pond2010.xlsx has same meta data. They can be combined to eliminate the data redundancy.
8. More details can be given in data dictionary. For example, no where it is mentioned what the column "z" meant. Columns can be more meaningful.

### Task 2 Solutions
#2: Suggest a new system for organization. Create a table in your Markdown document showing a potential template for later years of data collection that would address the problems you identified in #1.
#### **Solution**:
1. Instead of date, the column name can be "Timestamp" and values populated should include date along with hours, minutes and seconds. Among with this, there can be a column stating weather it is day or night. Because one cannot rely on time for day or night. This changes based on season. Hence it is better to include a column having two possible values "D/N".
2. No negative values must be entered for cuni/Chippo per Litre.
3. Colony size should have integers rather than decimals. 
4. Significance of Red and yellow higlights  should be metioned in data dictionary.
5. Beside every possible column, mention its units of measurement..
7. Include an Yellow book map for Section B data.
8. Name the columns with more meaningful names or column meaning must be included in data dictionary.
9. There is no need of seperate file for each year. There can just be two files. One for Cuni and one for Chippo. Table structure is given below.

### TABLES

**Table A: Chippo Table** 

| Timestamp | D/N  | Depth(mtrs) | Density (g/cm3)     | Colony Size(mtrs) | Chrophyl A | Temp(celcius) | Station |
|----------:|------|-------------|---------------------|-------------------|------------|---------------|---------|
|           |      |             |                     |                   |            |               |         |
|           |      |             |                     |                   |            |               |         |

**Table B: Cuni Table**  

| Timestamp | D/N  | Depth(mtrs) | Density (g/cm3)     | Colony Size(mtrs) | Chrophyl A | Temp(celcius) | Station |
|----------:|------|-------------|---------------------|-------------------|------------|---------------|---------|
|           |      |             |                     |                   |            |               |         |
|           |      |             |                     |                   |            |               |         |

### License

This project is licensed under the MIT License - see the [LICENSE](https://github.com/SriniVishnu/DataEntryAnalysis/blob/master/LICENSE) file for details

## <a name="naming"></a> 3. Naming Conventions

In this section, we describe the naming conventions used for raw and aggregated data.  These conventions can be expected to be stable over time and are intended for use by FCPS staff and research partners.  


[Back to the Top](#top)  [Back to Table of Contents](#codingStandardsTOC)

### <a name="nameStyle"></a> Naming Style

Whenever possible, we will try to use the fewest characters possible to unambiguously identify a datum.  This often requires several combinations of letters to be used in order to construct standardized names conforming to our naming conventions.  The sections below provide information about cases where static definitions exist (e.g., <a href="#demographics">Demographic Data</a>) and cases where the names are constructed from combinations of discrete pieces of information to identify the meaning of the datum (e.g., <a href="#assessment">Assessment Data</a>).  There are some common elements that are used to construct meaning as prefix or suffix elements:

Table. <em>Common Prefixes and Suffixes Used in Naming Conventions</em>

Prefix/Suffix | Meaning 
-------------- | ---------
sch | School
dist | District
id | Identifier/ID Number
std | Student
tch | Teacher
pct | Percent
n | Number/Count
nm | Name
yr | Year

[Back to the Top](#top) [Back to beginning of Section](#naming) [Back to Table of Contents](#codingStandardsTOC)

### <a name="demographics"></a> Demographic Data
The table below shows the names given to attributes used to reference demographic data.

<a name="demographicsTable"></a>
Table. <em>Demographic naming conventions</em>

Name | Definition | Datum Type
---- | ----------- | -----------
sasid | State Assigned Student ID | str15
stdid | Local Student ID | str15
pid | Person ID | int
schid | Unique School ID | str6 
schyr | School Year (Academic Year Ending) | int
schnm | School Name | str50
distnm | District Name | str50
distid | District ID | str3
firstnm | First Name | str50
mi | Middle Initial | str1
lastnm | Last Name | str50
dob | Date of Birth | date
sdate | Starting Date | date
edate | Ending Date | date
grade | The grade level of the student | byte
sex | The biophysiological sex of the student | byte
race | The ethnoracial identification of the student | byte
swd | Indicator for students receiving special education services | byte
ell | Indicator for students receiving English Learner services | byte
frl | Indicator for students receiving Free/Reduced Price Lunch | byte
tag | Indicator for students receiving Gifted/Talented or Primary Talent Pool services | byte
hhm | Indicator for Homeless/Highly Mobile Students | byte
migrant | Indicator for students receiving services from the Migrant education program | byte
section504 | Indicator of whether or not the student has a 504 plan | byte
immigrant | Indicator of whether or not the student is an immigrant | byte
refugee | Indicator of whether or not the student is a refugee | byte


[Back to the Top](#top) [Back to beginning of Section](#naming) [Back to Table of Contents](#codingStandardsTOC)

### <a name="assessment"></a> Assessment Data
We use a simple grammar for our assessment variables that can be defined with a regular expression: `(([a-z]{3}){2}) ([a-z]{2,3})([0-9]{1,2})?(item[0-9]{1,2})?`.  This expression translates into a grammar to represent discrete pieces of the information that can be used to uniquely identify the data of interest: `testCode + subjectCode + scoreCode [ + # ] [ + item# ]`; in this example, we use the square brackets to denote optional information that is used to extend the base grammar to additional use cases.

We've provided some tables below that can help you to understand the naming conventions based on the grammatical role identified previously (e.g., testCode, subjectCode, etc...).  

<a name="testCodeTable"></a>
Table. <em>testCode values and descriptors.</em>

testCode  | Meaning   | testCode  | Meaning
--------- | --------- | --------- | --------- 
act       | ACT       | acc       | ACCESS
adv       | AP        | aep       | AEPS
avb       | ASVAB     | brg       | Brigance
cog       | CogAT     | ctb       | CTBS
dib       | DIBELS    | fst       | FAST
grd       | GRADE     | inb       | IB
ibs       | ITBS      | kos       | KOSSA
kpr       | K-Prep    | kyt       | KYOTTE
map       | NWEA MAP  | ols       | OLSAT
psa       | PSAT      | sat       | SAT
str       | STAMP     | wpt       | WAPT

<a name="subjectCodeTable"></a>
Table. <em>subjectCode values and descriptors.</em>

subjectCode | Meaning | subjectCode | Meaning
--------- | --------- | --------- | ---------
adb  |  Adaptive Behavior  |  al1	 | 	Algebra I
al2	 | 	Algebra II  |  beh	 | 	Behavior
bio	 | 	Biology  |  bmg	 | 	Business Management
clc	 | 	Calculus  |  cap	 | 	Capstone
chm	 | 	Chemestry  |  chi	 | 	Chinese
chr	 | 	Chinese : Reading  |  chs	 | 	Chinese : Speaking
chw	 | 	Chinese : Writing  |  cog	 | 	Cognitive Skills
cme	 | 	Command of Evidence  |  cmp	 | 	Comprehension
com	 | 	Computer Science  |  ecn	 | 	Economics
env	 | 	Environmental Science  |  eur	 | 	European History
exp	 | 	Explore  |  ede	 | 	Expression of Ideas
fmo	 | 	Fine Motor Skills  |  fpa	 | 	Fine/Performing Arts
fre	 | 	French  |  frr	 | 	French : Reading
frs	 | 	French : Speaking  |  frw	 | 	French : Writing
geo	 | 	Geometry  |  ger	 | 	German
gov	 | 	Government and Politics  |  gmo	 | 	Gross Motor Skills
his	 | 	History  |  hge	 | 	Human Geography
isf	 | 	Initial Sound Fluency  |  jpn	 | 	Japanese
jpr	 | 	Japanese : Reading  |  jps	 | 	Japanese : Speaking
jpw	 | 	Japanese : Writing  |  lgc  |  Language/Communication
lat	 | 	Latin  |  lnf	 | 	Letter Naming Fluency
lst	 | 	Listening    |   lit	 | 	Literature
lrc  |  Literacy | mcn	 | 	Macroeconomics    
mth	 | 	Mathematics | icn	 | 	Microeconomics    
mus	 | 	Music Theory | nwf	 | 	Nonsense Word Fluency    
ora	 | 	Oral Language | orf	 | 	Oral Reading Fluency    
tot	 | 	Overall/Total Score | psf	 | 	Phoneme Segmentation Fluency    
pha	 | 	Phonological Awareness | pwb  |  Physical Well-Being
phy	 | 	Physics  |  pln	 | 	Plan
trg	 | 	Plane Geometry/Trigonometry  |  pal	 | 	Pre-Algebra
psd	 | 	Problem Solving & Data Analysis  |  psy	 | 	Psychology
rdg	 | 	Reading   |  rnw	 | 	Reading & Writing
rla	 | 	Reading/Language Arts  |  rtf	 | 	Retell Fluency
rhs	 | 	Rhetorical Skills  |  sci	 | 	Science
sel	 | 	Selection Index    |  shs  | Self-Help Skills
aso	 | 	Social Skills | soc	 | 	Social Studies    
esp	 | 	Spanish | esr	 | 	Spanish : Reading    
ess	 | 	Spanish : Speaking | esw	 | 	Spanish : Writing    
spk	 | 	Speaking | ecv	 | 	Standard English Conventions    
sts	 | 	Statistics | usm	 | 	Usage Mechanics    
wuf	 | 	Word Use Fluency | wrt	 | 	Writing     

<a name="scoreCodeTable"></a>
Table. <em>scoreCode values and descriptors.</em>

scoreCode | Meaning
--------- | ---------
dec | Deciles
gle | Grade Level equivalents
grw | Observed Growth
pct | Percentiles
lev | Performance level (e.g., Novice, Pass, etc...)
prj | Projected Growth
raw | Raw score
sc  | Scaled score
sgp | Student Growth Percentiles




[Back to the Top](#top)      [Back to beginning of Section](#naming)      [Back to Table of Contents](#codingStandardsTOC)


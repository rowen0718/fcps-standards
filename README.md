# <a name="top"></a> Office of Data, Research, and Accountability [DRA](http://www.fcps.net/administration/departments/data) Standards and Style Guides

* [Data Standards](#dataStandardsTOC)
* [Coding Standards](#codingStandards)



# <a name="dataStandardsTOC"></a> Data Standards 
## Table of Contents

* [Data Standards](#dataStandards)
    1. [I/O Requirements](#io)
        * [Handling and Access to Personally Identifiable Information](#pii)
        * [Aggregated Data](#aggregates)
        * [Data Suppression Rules](#suppressionRules)
        * [Standard Format of Data Deliverables](#standardFormat)
        * [Adding Data to the Data Systems](#dataToDatabase)
    2. [Typing/Casting](#typecast)
        * [Data Types](#dataTypes)
        * [Measurement Scales](#measurementScales)
        * [Numeric Encoding](#numericEncoding)
        * [Dates, Times, and Datetimes](#dateTime)
        * [Binary/Compressed Large OBjects](#lobs)
    3. [Metadata](#metadata)
        * [Codebook](#codebook)
        * [Data Dictionary](#dataDictionary)
        * [Labeling Numerically Encoded Data](#valueLabels)
        * [Labeling Variables/Columns](#variableLabels)

# <a name="dataStandards"></a> [DRA](http://www.fcps.net/administration/departments/data) Data Standards
Section related to data standards independent of coding practices.

[Back to the Top](#top)  [Back to Table of Contents](#dataStandardsTOC)

## <a name="io"></a> 1. Input/Output Requirements
Section related to input/output operations related to data coming into [DRA](http://www.fcps.net/administration/departments/data)

[Back to the Top](#top)  [Back to Table of Contents](#dataStandardsTOC)

### <a name="pii"></a> Handling and Access to Personally Identifiable Information (PII)

[Back to the Top](#top) [Back to Top of Section](#io) [Back to Table of Contents](#dataStandardsTOC)

### <a name="aggregates"></a> Aggregated Data

[Back to the Top](#top) [Back to Top of Section](#io) [Back to Table of Contents](#dataStandardsTOC)

### <a name="suppressionRules"></a> Data Suppression Rules

[Back to the Top](#top) [Back to Top of Section](#io) [Back to Table of Contents](#dataStandardsTOC)

### <a name="standardFormat"></a> Standard Format of Data Deliverables

[Back to the Top](#top) [Back to Top of Section](#io) [Back to Table of Contents](#dataStandardsTOC)

### <a name="dataToDatabase"></a> Adding Data to the Data Systems

[Back to the Top](#top) [Back to Top of Section](#io) [Back to Table of Contents](#dataStandardsTOC)

## <a name="typecast"></a> 2. Data Typing/Casting Practices
Section related to practices related to typing/casting data.

[Back to the Top](#top)  [Back to Table of Contents](#dataStandardsTOC)

### <a name="dataTypes"></a> Data Types

[Back to the Top](#top) [Back to Top of Section](#typecast) [Back to Table of Contents](#dataStandardsTOC)

### <a name="measurementScales"></a> Measurement Scales

[Back to the Top](#top) [Back to Top of Section](#typecast) [Back to Table of Contents](#dataStandardsTOC)

### <a name="numericEncoding"></a> Numeric Encoding

[Back to the Top](#top) [Back to Top of Section](#typecast) [Back to Table of Contents](#dataStandardsTOC)

### <a name="dateTime"></a> Dates, Times, and Datetimes 

[Back to the Top](#top) [Back to Top of Section](#typecast) [Back to Table of Contents](#dataStandardsTOC)

### <a name="lobs"></a> Binary/Compressed Large OBjects

[Back to the Top](#top) [Back to Top of Section](#typecast) [Back to Table of Contents](#dataStandardsTOC)

{ include metadata.md }





# <a name="codingStandardsTOC"></a> Coding Standards
## Table of Contents

* [Coding Standards](#codingStandards)
	1. [Introduction](#purpose)
	2. [File System Management](#fileSystem)
	    * [File Naming Conventions](#fileNames)
	    * [Directory Tree Structure](#directoryTree)
	    * [Versioning Files](#fileVersions)
	3. [Naming Conventions](#naming)
	    * [Naming Style](#nameStyle)
	    * [Demographic Data](#demographics)
	    * [Assessment Data](#assessment)
	4. [Documenting Code](#documentation)
	    * [Literate Programming](#literateProgramming)
	    * [File Headers](#fileHeader)
	    * [Block Comments](#blockComments)
	    * [In-line Comments](#inlineComments)
	5. [Development Guidance](#whenToDev)
	    * [Reusability](#codeReuse)
	    * [Replicability](#replicable)
	    * [Reliability](#reliability)
	    * [Responsibility](#responsibility)
	6. [Version Control](#vcs)
	    * [Git: Live it, Learn it, Love it](#git)
	    * [Repository Initialization](#gitInit)
	    * [Staging Code for Commit](#gitAdd)
	    * [Committing Code to Repository](#gitCommit)
	    * [Pushing Changes to Remote Repository](#gitPush)
	    * [Getting Changes from Remote Repository](#gitFetch)
	    * [Combining Changes from Other Repositories/Branches](#gitMerge)
	    * [Pull Requests](#pullRequests)
	    * [Code Contributions](#contributingCode)
	7. [Style Guides](#codeStyle)
	    * [Stata](#Stata)
	    * [R](#R)
	    * [Java](#Java)
	    * [SQL](#SQL)
	    * [Bash](#bash)
	    * [C#](#CSharp)
	    * [Visual Basic](#vb)
	    * [Julia](#Julia)
	    * [Python](#Python)
	    * [Batch](#batch)
	8. [Code Reviews](#codeReview)
	    * [Reviewing Code](#reviewingCode)
	    * [Checking Style](#checkingStyle)
	    * [QA/QC](#qaqc)
	9. [Collecting Business Rules](#businessRules)
	    * [User Stories](#userStories)
	    * [Epics](#epics)
	    * [Projects](#projects)
	10. [Testing](#testing)
	    * [Unit Testing](#unit)
	    * [Regression Tests](#regression)    
	    * [User Acceptance Testing](#uat)


# <a name="codingStandards"></a> Coding Standards

[Back to the Top](#top)  [Back to Table of Contents](#codingStandardsTOC)

## <a name="purpose"></a> 1. Introduction

[Back to the Top](#top)  [Back to Table of Contents](#codingStandardsTOC)

## <a name="fileSystem"></a> 2. File System Management

[Back to the Top](#top) [Back to beginning of Section](#fileSystem) [Back to Table of Contents](#codingStandardsTOC)

### <a name="fileNames"></a> File Naming Conventions

[Back to the Top](#top) [Back to beginning of Section](#fileSystem) [Back to Table of Contents](#codingStandardsTOC)

### <a name="directoryTree"></a> Directory Tree Structure

[Back to the Top](#top) [Back to beginning of Section](#fileSystem) [Back to Table of Contents](#codingStandardsTOC)

### <a name="fileVersions"></a> Versioning Files

[Back to the Top](#top) [Back to beginning of Section](#fileSystem) [Back to Table of Contents](#codingStandardsTOC)

## <a name="naming"></a> 3. Naming Conventions

[Back to the Top](#top)  [Back to Table of Contents](#codingStandardsTOC)

### <a name="nameStyle"></a> Naming Style

[Back to the Top](#top) [Back to beginning of Section](#naming) [Back to Table of Contents](#codingStandardsTOC)

### <a name="demographics"></a> Demographic Data

[Back to the Top](#top) [Back to beginning of Section](#naming) [Back to Table of Contents](#codingStandardsTOC)

### <a name="assessment"></a> Assessment Data

[Back to the Top](#top) [Back to beginning of Section](#naming) [Back to Table of Contents](#codingStandardsTOC)

## <a name="documentation"></a> 4. Documenting Code

[Back to the Top](#top) [Back to Table of Contents](#codingStandardsTOC)

### <a name="literateProgramming"></a> Literate Programming

[Back to the Top](#top) [Back to beginning of Section](#documentation) [Back to Table of Contents](#codingStandardsTOC)

### <a name="fileHeader"></a> File Headers

[Back to the Top](#top) [Back to beginning of Section](#documentation) [Back to Table of Contents](#codingStandardsTOC)

### <a name="blockComments"></a> Block Comments

[Back to the Top](#top) [Back to beginning of Section](#documentation) [Back to Table of Contents](#codingStandardsTOC)

### <a name="inlineComments"></a> In-line Comments

[Back to the Top](#top) [Back to beginning of Section](#documentation) [Back to Table of Contents](#codingStandardsTOC)

## <a name="whenToDev"></a> 5. Development Guidance

[Back to the Top](#top)  [Back to Table of Contents](#codingStandardsTOC)

### <a name="codeReuse"></a> Reusability

[Back to the Top](#top) [Back to beginning of Section](#whenToDev) [Back to Table of Contents](#codingStandardsTOC)

### <a name="replicable"></a> Replicability

[Back to the Top](#top) [Back to beginning of Section](#whenToDev) [Back to Table of Contents](#codingStandardsTOC)

### <a name="reliability"></a> Reliability

[Back to the Top](#top) [Back to beginning of Section](#whenToDev) [Back to Table of Contents](#codingStandardsTOC)

### <a name="responsibility"></a> Responsibility

[Back to the Top](#top) [Back to beginning of Section](#whenToDev) [Back to Table of Contents](#codingStandardsTOC)

## <a name="vcs"></a> 6. Version Control

[Back to the Top](#top)  [Back to Table of Contents](#codingStandardsTOC)

### <a name="git"></a> Git: Live it, Learn it, Love it

[Back to the Top](#top) [Back to beginning of Section](#vcs) [Back to Table of Contents](#codingStandardsTOC)

### <a name="gitInit"></a> Repository Initialization

[Back to the Top](#top) [Back to beginning of Section](#vcs) [Back to Table of Contents](#codingStandardsTOC)

### <a name="gitAdd"></a> Staging Code for Commit

[Back to the Top](#top) [Back to beginning of Section](#vcs) [Back to Table of Contents](#codingStandardsTOC)

### <a name="gitCommit"></a> Committing Code to Repository

[Back to the Top](#top) [Back to beginning of Section](#vcs) [Back to Table of Contents](#codingStandardsTOC)

### <a name="gitPush"></a> Pushing Changes to Remote Repository

[Back to the Top](#top) [Back to beginning of Section](#vcs) [Back to Table of Contents](#codingStandardsTOC)

### <a name="gitFetch"></a> Getting Changes from Remote Repository

[Back to the Top](#top) [Back to beginning of Section](#vcs) [Back to Table of Contents](#codingStandardsTOC)

### <a name="gitMerge"></a> Combining Changes from Other Repositories/Branches

[Back to the Top](#top) [Back to beginning of Section](#vcs) [Back to Table of Contents](#codingStandardsTOC)

### <a name="pullRequests"></a> Pull Requests

[Back to the Top](#top) [Back to beginning of Section](#vcs) [Back to Table of Contents](#codingStandardsTOC)

### <a name="contributingCode"></a> Code Contributions

[Back to the Top](#top) [Back to beginning of Section](##vcs) [Back to Table of Contents](#codingStandardsTOC)

## <a name="codeStyle"></a> 7. Style Guides

[Back to the Top](#top)  [Back to Table of Contents](#codingStandardsTOC)

### <a name="Stata"></a> Stata

[Back to the Top](#top) [Back to beginning of Section](#codeStyle) [Back to Table of Contents](#codingStandardsTOC)

### <a name="R"></a> R

[Back to the Top](#top) [Back to beginning of Section](#codeStyle) [Back to Table of Contents](#codingStandardsTOC)

### <a name="Java"></a> Java

[Back to the Top](#top) [Back to beginning of Section](#codeStyle) [Back to Table of Contents](#codingStandardsTOC)

### <a name="SQL"></a> SQL

[Back to the Top](#top) [Back to beginning of Section](#codeStyle) [Back to Table of Contents](#codingStandardsTOC)

### <a name="bash"></a> Bash

[Back to the Top](#top) [Back to beginning of Section](#codeStyle) [Back to Table of Contents](#codingStandardsTOC)

### <a name="CSharp"></a> C#

[Back to the Top](#top) [Back to beginning of Section](#codeStyle) [Back to Table of Contents](#codingStandardsTOC)

### <a name="vb"></a> Visual Basic

[Back to the Top](#top) [Back to beginning of Section](#codeStyle) [Back to Table of Contents](#codingStandardsTOC)

### <a name="Julia"></a> Julia

[Back to the Top](#top) [Back to beginning of Section](#codeStyle) [Back to Table of Contents](#codingStandardsTOC)

### <a name="Python"></a> Python

[Back to the Top](#top) [Back to beginning of Section](#codeStyle) [Back to Table of Contents](#codingStandardsTOC)

### <a name="batch"></a> Batch

[Back to the Top](#top) [Back to beginning of Section](#codeStyle) [Back to Table of Contents](#codingStandardsTOC)

## <a name="codeReview"></a> 8. Code Reviews

[Back to the Top](#top)  [Back to Table of Contents](#codingStandardsTOC)

### <a name="reviewingCode"></a> Reviewing Code

[Back to the Top](#top) [Back to beginning of Section](#codeReview) [Back to Table of Contents](#codingStandardsTOC)

### <a name="checkingStyle"></a> Checking Style

[Back to the Top](#top) [Back to beginning of Section](#codeReview) [Back to Table of Contents](#codingStandardsTOC)

### <a name="qaqc"></a> 9. QA/QC

[Back to the Top](#top) [Back to beginning of Section](#codeReview) [Back to Table of Contents](#codingStandardsTOC)

## <a name="businessRules"></a> Collecting Business Rules

[Back to the Top](#top)  [Back to Table of Contents](#codingStandardsTOC)

### <a name="userStories"></a> User Stories

[Back to the Top](#top) [Back to beginning of Section](#businessRules) [Back to Table of Contents](#codingStandardsTOC)

### <a name="epics"></a> Epics

[Back to the Top](#top) [Back to beginning of Section](#businessRules) [Back to Table of Contents](#codingStandardsTOC)

### <a name="projects"></a> Projects

[Back to the Top](#top) [Back to beginning of Section](#businessRules) [Back to Table of Contents](#codingStandardsTOC)

## <a name="testing"></a> 10. Testing

[Back to the Top](#top)  [Back to Table of Contents](#codingStandardsTOC)

### <a name="unit"></a> Unit Testing

[Back to the Top](#top) [Back to beginning of Section](#testing) [Back to Table of Contents](#codingStandardsTOC)

### <a name="regression"></a> Regression Tests    

[Back to the Top](#top) [Back to beginning of Section](#testing) [Back to Table of Contents](#codingStandardsTOC)

### <a name="uat"></a> User Acceptance Testing

[Back to the Top](#top) [Back to beginning of Section](#testing) [Back to Table of Contents](#codingStandardsTOC)
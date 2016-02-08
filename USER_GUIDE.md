##	Public Budget Database User's Guide
### Budget of the United States Government, Fiscal Year 2016

### Prepared by: Budget Analysis Branch, Office of Management and Budget February 2015
 
This document describes three data files that contain an extract of the Office of Management and Budget (OMB) budget database.  These files can be used to reproduce many of the totals published in the Budget and examine unpublished details below the levels of aggregation published in the Budget.  These data, however, have some limitations to their scope and usefulness.

The following sections describe the sources and limitations of the data, as well as the content, format, and coding of the data files.

## 1.  Data sources and limitations

### a. Sources of data

Historical data for completed fiscal years are summarized from the financial records of the U.S. Government maintained by the Office of Management and Budget (OMB) and the Department of the Treasury.  The totals are generally consistent with data published in the *Monthly Treasury Statement*, by the Fiscal Service of the Department of the Treasury.  Differences between the Treasury publications and the Budget arise from a small number of reporting and classification corrections made subsequent to the Treasury publications and some conceptual differences between OMB and Treasury reporting.
  
In addition, these historical records are adjusted each year to conform to the agency and account structure of the current budget.  For example, data originally reported in the 1966 Budget by the Department of Health, Education, and Welfare, now appear under the Department of Health and Human Services, the Department of Education, or the Social Security Administration, as appropriate.  Lastly, the historical database has been updated for changes in the functional classification of accounts and in the Budget Enforcement Act (BEA) categorization.

Budget estimates for the current fiscal year (2015) and the budget year (2016) are prepared by agencies, based on the definitions and guidance contained in OMB Circular A-11, "Preparation, Submission, and Execution of the Budget."  Budget totals for these years reflect the President’s fiscal policy and economic assumptions, which are extensively described in the Budget documents.

The data files provide sufficient detail to produce: (a) outlay totals by agency, subfunction, and Budget Enforcement Act category that are consistent with the totals presented in the 2016 Budget; (b) receipt totals by source, as shown in various published tables in the Budget; and (c) the deficit (on-budget, off-budget, and unified budget basis).  In addition, outlays can be further disaggregated by grants to State and local governments and non-grants.

### b.  Fiscal years

The data in these files are for fiscal years.  Prior to 1977, the fiscal year began on July 1 and ended on June 30.  For example, fiscal year 1965 began on July 1, 1964, and ended on June 30, 1965.  Beginning with fiscal year 1977, the fiscal year begins on October 1 and ends on September 30.  For example, fiscal year 2013 began on October 1, 2012, and ended on September 30, 2013.  Fiscal year 1976 ended on June 30, 1976, and fiscal year 1977 began on October 1, 1976.  The period July 1, 1976, to September 30, 1976, is called the "transition quarter" or TQ.

### c.  Units of measure

Data for budget authority, outlays, offsetting receipts, and governmental receipts are shown in thousands of dollars.

### d.  Limitations

These data files do not contain data by object classes, data for program and financing accounts, character class (other than grants to State and local governments), personnel summaries, or credit schedules.  Account-level details are based on the proposed Budget only and do not include current services estimates.

With few exceptions, these files present account-level details that are consistent with the account structure of the current Budget.  For governmental receipts and offsetting receipts, data prior to 1982 are aggregates in sufficient detail to produce the published tables, but are not "true" account-level details.  For budget authority, no data are available prior to 1976.  For outlays, data for 1962-1981 tend to be account-level details.  Exceptions include the Legislative Branch and Department of Defense, which are available only at bureau-level detail in the earlier years.

Users of these data files should be careful to review and understand the effects that these limitations may have on their analysis of budget data and trends.  For example, computation of compound annual growth rates of various receipt accounts in the Budget could be severely affected by the discontinuities in account-level details prior to 1982.

### e.  Further information 

Readers who are not already familiar with the Federal Budget should gain a familiarity with the concepts and organization of the budget before proceeding.  The following documents may be helpful: 

**Analytical Perspectives, Budget of the United States Government, Fiscal Year 2016**. This document contains analyses that are designed to highlight specified program areas or provide other significant presentations of Budget data that place the Budget in perspective.  It includes a discussion of the concepts underlying the organization of the Budget and the presentation of Budget data, economic assumptions underlying the Budget estimates, Federal receipts and collections, including user fees and tax expenditures, Federal spending, the Budget Enforcement Act, and other topics.  A particularly useful chapter is "Budget Concepts," which contains a discussion of budget concepts.  Also of particular use is a report entitled, “Table 29-1. Federal Budget By Agency and Account,” which contains a listing of all appropriation and fund accounts in the Budget.  (This report is available online in the Supplemental Materials section at:  http://www.whitehouse.gov/omb/budget/Analytical_Perspectives/.)

**OMB Circular A-11** provides instructions to agencies in preparing Budget submissions, including details for entry into the Budget database.

In addition, there is extensive literature on the Federal Budget that could be usefully consulted.

## 2.  Data files and file formats

The account-level data is available in spreadsheet and file import format.

### a.  Spreadsheet format

Files are provided in “CSV” format.  Virtually any spreadsheet program can read this common format.  In “CSV” format, data fields are separated by commas, text fields are contained inside double quote marks, and numerical fields do not have embedded commas.  Each record is contained on a single line.  This format is commonly used by database software.  Separate files for receipts, outlays, and budget authority are available in each of these formats and are described in detail below.

### b.  File names, contents, and sequence

In all files, the records are sequenced by agency code, bureau code, account code, subfunction code, BEA category, grant/non-grant, and on-/off-budget field.

The files with the account-level data are:
  - `outlays.csv`	— Outlays and offsetting receipts, 1962-2020, in csv format.
  - `receipts.csv` — Governmental receipts, 1962-2020, in file csv format.
  - `budauth.csv`	— Budget authority and offsetting receipts, 1976-2020, in csv format.

Offsetting receipts are in the budget authority files as well as the outlay files.  These amounts are needed to calculate net budget authority and net outlays.

## 3.  Categorization of budget data

The categorization of budget data differs slightly among receipts, outlays, and budget authority files.

### a.  Budget authority and outlay files

Account details are categorized using the following keys:

**Agency:** Agency codes generally correspond to the Cabinet department or independent agency with primary responsibility for the program.  There are two major exceptions to this definition: (1) the Legislative Branch and the Judiciary are displayed as agencies, though they are separate branches of Government; and (2) intragovernmental payments of interest to trust funds, payments of employer share of employee retirement contributions, and interest paid to the Outer Continental Shelf escrow account are classified as "undistributed offsetting receipts."  The agency coding used in the data files is consistent with the tables in the Budget documents that present budget authority and outlays by agency.  These codes and titles differ from the “Treasury Agency” code, described below.  In addition, some allowances are not distributed by agency or by function and are given a special agency code.

**Bureau:** Bureaus are major subdivisions within Cabinet departments that correspond to major organizational areas.  Within Cabinet departments, these major organizational areas may be called "bureaus" (e.g., the Bureau of the Census within the Commerce Department or the Bureau of Labor Statistics within the Labor Department), “services” (e.g., the Internal Revenue Service within the Treasury Department or the Economic Research Service within the Agriculture Department); “offices” (e.g., Office of Postsecondary Education in the Education Department) or they may be broad budget categories (e.g., Procurement or Military Personnel in the Defense Department).  Table 1 presents a listing of the agency and bureau categories used in the data files.

**Account:** These numbers are assigned by the Treasury Department and are used for budget presentation and financial management.  In some instances, groups of small accounts (usually miscellaneous special and trust fund accounts) have been consolidated into single accounts.

**Subfunction:** Accounts are categorized by the subfunctions shown in Table 2.  Accounts that include multiple subfunctions are subdivided into subfunction components.

**Treasury Agency:** These codes are defined in the *Treasury Financial Manual, Supplement to Volume I, Federal Account Symbols and Titles*, which contains the titles corresponding to these codes.

**Budget Enforcement Act category:** The Budget Enforcement Act (the "Act") made distinctions between mandatory and discretionary accounts for certain provisions of the Act.  This distinction is still used for scorekeeping and accounts are categorized accordingly.  Initially, accounts were assigned categories based on the agreement shown in the Act’s statement of managers.  Since that time, Administration and Congressional scorekeepers maintain the list, assigning new accounts and adjusting existing accounts when there is agreement.  Where an account includes mandatory and discretionary activities, separate lines of data, appropriately coded, will be found in the data files.  The possible values for this code are:

**Discretionary:** Discretionary spending is controlled through annual appropriations acts.

**Mandatory:** Mandatory spending generally operates under permanent authority.  Statutes generally specify what must be paid and who is eligible to receive payments.  Governmental receipt accounts are categorized as "governmental receipts" as described below.

**Net interest:** Interest payments to and from the public and intragovernmental payments of interest, primarily to trust funds, are not included as either mandatory or discretionary spending.

Readers wanting more information on this topic may refer to several chapters in the *Analytical Perspectives* volume.

**Grant/Non-grant:** Grants to State and local governments are separated from non-grant outlays, based on the definitions in OMB Circular A-11 for schedule C data.

### b.  Receipts files

Receipt account data are categorized as follows:

**Source category:** These are major categories of governmental receipts, such as individual income tax receipts or corporation income tax receipts.  (See Table 3.)

**Source subcategory:** These present further detail within source categories. (See Table 3.)

**Account:** These are assigned by the Treasury Department and are used for budget presentation as well as financial management.  In some instances, groups of small accounts (usually miscellaneous receipt accounts) have been consolidated into single accounts.

**Treasury Agency:** These codes are defined in the *Treasury Financial Manual, Supplement to Volume I, Federal Account Symbols and Titles*, which contains the titles corresponding to these codes.

## 4.  Description of the fields in the outlay files

The following table describes the fields of data for the account-level files.  For data files in spreadsheet format, the fields are separate spreadsheet columns.  For files in file import format, commas, as previously described, separate the fields.

<table>
  <thead>
	<tr>
	  <th>Field number</th>
	  <th>Field name</th>
	  <th>Description</th>
	  <th>Valid values</th>
	</tr>
  </thead>
  <tbody>
  <tr>
    <td>1</td>
    <td>Agency code</td>
    <td>3-digit numerical code for Cabinet department or independent agency</td>
    <td>See Table 1 (below) "Listing of Agency and Bureau Codes"</td>
  </tr>
  <tr>
    <td>2</td>
    <td>Agency name</td>
    <td>Agency name from Table 1 (maximum: 89 characters)</td>
    <td>See Table 1</td>
  </tr>
  <tr>
    <td>3</td>
    <td>Bureau code</td>
    <td>2-digit numerical code for the bureau within the Cabinet department or independent agency</td>
    <td>See Table 1</td>
  </tr>
  <tr>
    <td>4</td>
    <td>Bureau name</td>
    <td>Bureau name from Table 1 (maximum: 89 characters)</td>
    <td>See Table 1</td>
  </tr>
  <tr>
    <td>5</td>
    <td>Account code</td>
    <td>4-digit code (outlays) or 6-digit code (offsetting receipts)</td>
    <td>Any 4- or 6-digit number</td>
  </tr>
  <tr>
    <td>6</td>
    <td>Account name</td>
    <td>Account name (maximum: 160 characters)</td>
    <td>Any text</td>
  </tr>
  <tr>
    <td>7</td>
    <td>Treasury Agency code</td>
    <td>2-digit numerical code for the agency, assigned by the Treasury Department</td>
    <td>See Treasury publication cited above</td>
  </tr>
  <tr>
    <td>8</td>
    <td>Subfunction code</td>
    <td>3-digit numerical code for the subfunction</td>
    <td>See Table 2, “Listing of Functions and Subfunctions”</td>
  </tr>
  <tr>
    <td>9</td>
    <td>Subfunction title</td>
    <td>Subfunction title (maximum: 72 characters)</td>
    <td>See Table 2</td>
  </tr>
  <tr>
    <td>10</td>
    <td>BEA category</td>
    <td>Budget Enforcement Act category</td>
    <td>“Mandatory,” “Discretionary,” or “Net interest”</td>
  </tr>
  <tr>
    <td>11</td>
    <td>Grant/non-grant split</td>
    <td>Identifier to indicate if the outlays are grant or non-grant (outlays only)</td>
    <td>“Grant” or “Nongrant”</td>
  </tr>
  <tr>
    <td>12</td>
    <td>On- and off-budget indicator</td>
    <td>Social Security trust funds and the Postal Service are off-budget, all other accounts are on-budget</td>
    <td>“On-budget” or “Off-budget”</td>
  </tr>
  <tr>
    <td>13</td>
    <td>1962 value</td>
    <td>Actual amounts, in thousands of dollars, for FY 1962</td>
    <td>Outlays are usually positive values.  Offsetting receipts are usually negative values.</td>
  </tr>
  <tr>
    <td>14-27</td>
    <td>1963 – 1976 values</td>
    <td>Actual amounts, in thousands of dollars, for each fiscal year</td>
    <td>(same as above)</td>
  </tr>
  <tr>
    <td>28</td>
    <td>TQ value</td>
    <td>Actual amounts, in thousands of dollars, for the “transitional quarter” (see note above)</td>
    <td>(same as above)</td>
  </tr>
  <tr>
    <td>29-66</td>
    <td>1977 – 2014 values</td>
    <td>Actual amounts, in thousands of dollars, for each fiscal year</td>
    <td>(same as above)</td>
  </tr>
  <tr>
    <td>67-72</td>
    <td>2015 – 2020 values</td>
    <td>Estimated amounts, in thousands of dollars, for FY 2015 through FY 2020</td>
    <td>(same as above)</td>
  </tr>
  </tbody>
</table>


## 5.  Description of the fields in the budget authority files

The following table describes the fields of data for the account-level files.  For data files in spreadsheet format, the fields are separate spreadsheet columns.  For files in file import format, the fields are separated by commas, as described above.

<table>
  <thead>
	<tr>
	  <th>Field number</th>
	  <th>Field name</th>
	  <th>Description</th>
	  <th>Valid values</th>
	</tr>
  </thead>
  <tbody>
  <tr>
    <td>1</td>
    <td>Agency code</td>
    <td>3-digit numerical code for Cabinet department or independent agency</td>
    <td>See Table 1 (below) "Listing of Agency and Bureau Codes" </td>
  </tr>
  <tr>
    <td>2</td>
    <td>Agency name</td>
    <td>Agency name from Table 1 (maximum: 89 characters)</td>
    <td>See Table 1</td>
  </tr>
  <tr>
    <td>3</td>
    <td>Bureau code</td>
    <td>2-digit numerical code for the bureau within the Cabinet department or independent agency</td>
    <td>See Table 1</td>
  </tr>
  <tr>
    <td>4</td>
    <td>Bureau name</td>
    <td>Bureau name from Table 1 (maximum: 89 characters)</td>
    <td>See Table 1</td>
  </tr>
  <tr>
    <td>5</td>
    <td>Account code</td>
    <td>4-digit code (outlays) or 6-digit code (offsetting receipts)</td>
    <td>Any 4- or 6- digit number</td>
  </tr>
  <tr>
    <td>6</td>
    <td>Account name</td>
    <td>Account name (maximum: 160 characters)</td>
    <td>Any text</td>
  </tr>
  <tr>
    <td>7</td>
    <td>Treasury Agency code</td>
    <td>2-digit numerical code for the agency, assigned by the Treasury Department</td>
    <td>See Treasury publication cited above</td>
  </tr>
  <tr>
    <td>8</td>
    <td>Subfunction code</td>
    <td>3-digit numerical code for the subfunction</td>
    <td>See Table 2, “Listing of Functions and Subfunctions”</td>
  </tr>
  <tr>
    <td>9</td>
    <td>Subfunction title</td>
    <td>Subfunction title (maximum: 72 characters)</td>
    <td>See Table 2</td>
  </tr>
  <tr>
    <td>10</td>
    <td>BEA category</td>
    <td>Budget Enforcement Act category</td>
    <td>“Mandatory,” “Discretionary,” or “Net interest”</td>
  </tr>
  <tr>
    <td>11</td>
    <td>On- and off-budget indicator</td>
    <td>Social Security trust funds and the Postal Service are off-budget, all other accounts are on-budget</td>
    <td>“On-budget” or “Off-budget”</td>
  </tr>
  <tr>
    <td>12</td>
    <td>1976 value</td>
    <td>Actual amounts, in thousands of dollars, for FY 1976</td>
    <td>Budget authority is usually shown as a positive value.  Offsetting receipts are usually negative values.</td>
  </tr>
  <tr>
    <td>13</td>
    <td>TQ value</td>
    <td>Actual amounts, in thousands of dollars, for the “transitional quarter” (see note above)</td>
    <td>(same as above)</td>
  </tr>
  <tr>
    <td>14-51</td>
    <td>1977 – 2014 values</td>
    <td>Actual amounts, in thousands of dollars, for each fiscal year</td>
    <td>(same as above)</td>
  </tr>
  <tr>
    <td>52-57</td>
    <td>2015 – 2020 values</td>
    <td>Estimated amounts, in thousands of dollars, for FY 2015 through FY 2020</td>
    <td>(same as above)</td>
  </tr>
  </tbody>
</table>


## 6.  Description of the fields in the receipts files

The following table describes the fields of data for the account-level files.  For data files in spreadsheet format, the fields are separate spreadsheet columns.  For files in file import format, the fields are separated by commas, as described above.

<table>
  <thead>
	<tr>
	  <th>Field number</th>
	  <th>Field name</th>
	  <th>Description</th>
	  <th>Valid values</th>
	</tr>
  </thead>
  <tbody>
  <tr>
    <td>1</td>
    <td>Source category code</td>
    <td>3-digit numerical code for source category</td>
    <td>See Table 3 (below) "Source Categories for Receipts"</td>
  </tr>
  <tr>
    <td>2</td>
    <td>Source category name</td>
    <td>Title for receipts category (maximum: 41 characters)</td>
    <td>See Table 3</td>
  </tr>
  <tr>
    <td>3</td>
    <td>Source subcategory</td>
    <td>2-digit numerical code for the source subcategory</td>
    <td>See Table 3</td>
  </tr>
  <tr>
    <td>4</td>
    <td>Source subcategory name</td>
    <td>Title for receipts subcategory (maximum: 35 characters)</td>
    <td>See Table 3</td>
  </tr>
  <tr>
    <td>5</td>
    <td>Agency code</td>
    <td>3-digit numerical code for Cabinet department or independent agency</td>
    <td>See Table 1 (below) “Listing of Agency and Bureau Codes”</td>
  </tr>
  <tr>
    <td>6</td>
    <td>Agency name</td>
    <td>Agency name from Table 1 (maximum: 89 characters)</td>
    <td>See Table 1</td>
  </tr>
  <tr>
    <td>7</td>
    <td>Bureau code</td>
    <td>2-digit numerical code for the bureau within the Cabinet department or independent agency</td>
    <td>See Table 1</td>
  </tr>
  <tr>
    <td>8</td>
    <td>Bureau name</td>
    <td>Bureau name from Table 1 (maximum: 89 characters)</td>
    <td>See Table 1</td>
  </tr>
  <tr>
    <td>9</td>
    <td>Account code</td>
    <td>6-digit numerical code for the account</td>
    <td>Any 6-digit number</td>
  </tr>
  <tr>
    <td>10</td>
    <td>Account name</td>
    <td>Account name (maximum: 114 characters)</td>
    <td>Any text</td>
  </tr>
  <tr>
    <td>11</td>
    <td>Treasury Agency code</td>
    <td>2-digit numerical code for the agency, assigned by the Treasury Department</td>
    <td>See Treasury publication cited above</td>
  </tr>
  <tr>
    <td>12</td>
    <td>On- and off-budget indicator</td>
    <td>Social Security trust funds and the Postal Service are off-budget, all other accounts are on-budget</td>
    <td>“On-budget” or “Off-budget”</td>
  </tr>
  <tr>
    <td>13</td>
    <td>1962 value</td>
    <td>Actual amounts, in thousands of dollars, for FY 1962</td>
    <td>Receipts are usually shown as positive values</td>
  </tr>
  <tr>
    <td>14 - 27</td>
    <td>1963 - 1976 values</td>
    <td>Actual amounts, in thousands of dollars, for FY 1963 through FY 1976</td>
    <td>(same as above)</td>
  </tr>
  <tr>
    <td>28</td>
    <td>TQ value</td>
    <td>Actual amounts, in thousands of dollars, for the “transitional quarter” (see note above)</td>
    <td>(same as above)</td>
  </tr>
  <tr>
    <td>29-66</td>
    <td>1977 - 2014 values</td>
    <td>Actual amounts, in thousands of dollars, for each fiscal year</td>
    <td>(same as above)</td>
  </tr>
  <tr>
    <td>67-72</td>
    <td>2015 - 2020 values</td>
    <td>Estimated amounts, in thousands of dollars, for FY 2015 through FY 2020</td>
    <td>(same as above)</td>
  </tr>
  </tbody>
</table>


## 7.  Reference tables

The following tables present: (a) agency and bureau codes and titles used in the data files; (b) function and subfunction codes and titles; and (c) receipt source category and subcategory titles.

<table>
  <caption>Table 1.  Listing of Agency and Bureau Codes Used in the Public Budget Database</caption>
  <thead>
	<tr>
	  <th>Agency</th>
	  <th>Bureau</th>
	  <th>Title</th>
	</tr>
  </thead>
  <tbody>
  <tr>
    <td>001</td>
    <td></td>
    <td>Legislative Branch</td>
  </tr>
  <tr>
    <td>001</td>
    <td>05</td>
    <td>Senate</td>
  </tr>
  <tr>
    <td>001</td>
    <td>10</td>
    <td>House of Representatives</td>
  </tr>
  <tr>
    <td>001</td>
    <td>11</td>
    <td>Joint Items</td>
  </tr>
  <tr>
    <td>001</td>
    <td>12</td>
    <td>Office of Compliance</td>
  </tr>
  <tr>
    <td>001</td>
    <td>13</td>
    <td>Capitol Police</td>
  </tr>
  <tr>
    <td>001</td>
    <td>14</td>
    <td>Congressional Budget Office</td>
  </tr>
  <tr>
    <td>001</td>
    <td>15</td>
    <td>Architect of the Capitol</td>
  </tr>
  <tr>
    <td>001</td>
    <td>18</td>
    <td>Botanic Garden</td>
  </tr>
  <tr>
    <td>001</td>
    <td>25</td>
    <td>Library of Congress</td>
  </tr>
  <tr>
    <td>001</td>
    <td>30</td>
    <td>Government Publishing Office</td>
  </tr>
  <tr>
    <td>001</td>
    <td>35</td>
    <td>Government Accountability Office</td>
  </tr>
  <tr>
    <td>001</td>
    <td>40</td>
    <td>United States Tax Court</td>
  </tr>
  <tr>
    <td>001</td>
    <td>45</td>
    <td>Legislative Branch Boards and Commissions</td>
  </tr>
  <tr>
    <td>001</td>
    <td>60</td>
    <td>John C. Stennis Center for Public Service Training and Development</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>002</td>
    <td></td>
    <td>Judicial Branch</td>
  </tr>
  <tr>
    <td>002</td>
    <td>05</td>
    <td>Supreme Court of the United States</td>
  </tr>
  <tr>
    <td>002</td>
    <td>07</td>
    <td>United States Court of Appeals for the Federal Circuit</td>
  </tr>
  <tr>
    <td>002</td>
    <td>10</td>
    <td>Court of Customs and Patent Appeals</td>
  </tr>
  <tr>
    <td>002</td>
    <td>15</td>
    <td>United States Court of International Trade</td>
  </tr>
  <tr>
    <td>002</td>
    <td>20</td>
    <td>Court of Claims</td>
  </tr>
  <tr>
    <td>002</td>
    <td>25</td>
    <td>Courts of Appeals, District Courts, and other Judicial Services</td>
  </tr>
  <tr>
    <td>002</td>
    <td>26</td>
    <td>Administrative Office of the United States Courts</td>
  </tr>
  <tr>
    <td>002</td>
    <td>30</td>
    <td>Federal Judicial Center</td>
  </tr>
  <tr>
    <td>002</td>
    <td>34</td>
    <td>Bicentennial Expenses, The Judiciary</td>
  </tr>
  <tr>
    <td>002</td>
    <td>35</td>
    <td>Judicial Retirement Funds</td>
  </tr>
  <tr>
    <td>002</td>
    <td>37</td>
    <td>National Commission on Judicial Discipline and Removal</td>
  </tr>
  <tr>
    <td>002</td>
    <td>39</td>
    <td>United States Sentencing Commission</td>
  </tr>
  <tr>
    <td>002</td>
    <td>42</td>
    <td>Violent Crime Reduction Programs</td>
  </tr>
  <tr>
    <td>002</td>
    <td>99</td>
    <td>The Judiciary, activities</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>005</td>
    <td></td>
    <td>Department of Agriculture</td>
  </tr>
  <tr>
    <td>005</td>
    <td>03</td>
    <td>Office of the Secretary</td>
  </tr>
  <tr>
    <td>005</td>
    <td>04</td>
    <td>Executive Operations</td>
  </tr>
  <tr>
    <td>005</td>
    <td>05</td>
    <td>Departmental Management</td>
  </tr>
  <tr>
    <td>005</td>
    <td>07</td>
    <td>Office of Civil Rights</td>
  </tr>
  <tr>
    <td>005</td>
    <td>08</td>
    <td>Office of Inspector General</td>
  </tr>
  <tr>
    <td>005</td>
    <td>10</td>
    <td>Office of the General Counsel</td>
  </tr>
  <tr>
    <td>005</td>
    <td>12</td>
    <td>Office of Chief Information Officer</td>
  </tr>
  <tr>
    <td>005</td>
    <td>13</td>
    <td>Economic Research Service</td>
  </tr>
  <tr>
    <td>005</td>
    <td>14</td>
    <td>Office of Chief Financial Officer</td>
  </tr>
  <tr>
    <td>005</td>
    <td>15</td>
    <td>National Agricultural Statistics Service</td>
  </tr>
  <tr>
    <td>005</td>
    <td></td>
    <td>Department of Agriculture – continued</td>
  </tr>
  <tr>
    <td>005</td>
    <td>16</td>
    <td>Hazardous Materials Management</td>
  </tr>
  <tr>
    <td>005</td>
    <td>18</td>
    <td>Agricultural Research Service</td>
  </tr>
  <tr>
    <td>005</td>
    <td>19</td>
    <td>Buildings and Facilities</td>
  </tr>
  <tr>
    <td>005</td>
    <td>20</td>
    <td>National Institute of Food and Agriculture</td>
  </tr>
  <tr>
    <td>005</td>
    <td>32</td>
    <td>Animal and Plant Health Inspection Service</td>
  </tr>
  <tr>
    <td>005</td>
    <td>35</td>
    <td>Food Safety and Inspection Service</td>
  </tr>
  <tr>
    <td>005</td>
    <td>37</td>
    <td>Grain Inspection, Packers and Stockyards Administration</td>
  </tr>
  <tr>
    <td>005</td>
    <td>45</td>
    <td>Agricultural Marketing Service</td>
  </tr>
  <tr>
    <td>005</td>
    <td>47</td>
    <td>Risk Management Agency</td>
  </tr>
  <tr>
    <td>005</td>
    <td>49</td>
    <td>Farm Service Agency</td>
  </tr>
  <tr>
    <td>005</td>
    <td>53</td>
    <td>Natural Resources Conservation Service</td>
  </tr>
  <tr>
    <td>005</td>
    <td>55</td>
    <td>Rural Development</td>
  </tr>
  <tr>
    <td>005</td>
    <td>60</td>
    <td>Rural Utilities Service</td>
  </tr>
  <tr>
    <td>005</td>
    <td>63</td>
    <td>Rural Housing Service</td>
  </tr>
  <tr>
    <td>005</td>
    <td>65</td>
    <td>Rural Business—Cooperative Service</td>
  </tr>
  <tr>
    <td>005</td>
    <td>68</td>
    <td>Foreign Agricultural Service</td>
  </tr>
  <tr>
    <td>005</td>
    <td>84</td>
    <td>Food and Nutrition Service</td>
  </tr>
  <tr>
    <td>005</td>
    <td>96</td>
    <td>Forest Service</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>006</td>
    <td></td>
    <td>Department of Commerce</td>
  </tr>
  <tr>
    <td>006</td>
    <td>05</td>
    <td>Departmental Management</td>
  </tr>
  <tr>
    <td>006</td>
    <td>06</td>
    <td>Economic Development Administration</td>
  </tr>
  <tr>
    <td>006</td>
    <td>07</td>
    <td>Bureau of the Census</td>
  </tr>
  <tr>
    <td>006</td>
    <td>08</td>
    <td>Economics and Statistics Administration</td>
  </tr>
  <tr>
    <td>006</td>
    <td>15</td>
    <td>Regional Development Program</td>
  </tr>
  <tr>
    <td>006</td>
    <td>25</td>
    <td>International Trade Administration</td>
  </tr>
  <tr>
    <td>006</td>
    <td>30</td>
    <td>Bureau of Industry and Security</td>
  </tr>
  <tr>
    <td>006</td>
    <td>40</td>
    <td>Minority Business Development Agency</td>
  </tr>
  <tr>
    <td>006</td>
    <td>44</td>
    <td>United States Travel and Tourism Administration</td>
  </tr>
  <tr>
    <td>006</td>
    <td>48</td>
    <td>National Oceanic and Atmospheric Administration</td>
  </tr>
  <tr>
    <td>006</td>
    <td>51</td>
    <td>U.S. Patent and Trademark Office</td>
  </tr>
  <tr>
    <td>006</td>
    <td>53</td>
    <td>Technology Administration</td>
  </tr>
  <tr>
    <td>006</td>
    <td>54</td>
    <td>National Technical Information Service</td>
  </tr>
  <tr>
    <td>006</td>
    <td>55</td>
    <td>National Institute of Standards and Technology</td>
  </tr>
  <tr>
    <td>006</td>
    <td>60</td>
    <td>National Telecommunications and Information Administration</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>007</td>
    <td></td>
    <td>Department of Defense—Military Programs</td>
  </tr>
  <tr>
    <td>007</td>
    <td>05</td>
    <td>Military Personnel</td>
  </tr>
  <tr>
    <td>007</td>
    <td>10</td>
    <td>Operation and Maintenance</td>
  </tr>
  <tr>
    <td>007</td>
    <td>12</td>
    <td>International Reconstruction and Other Assistance</td>
  </tr>
  <tr>
    <td>007</td>
    <td>15</td>
    <td>Procurement</td>
  </tr>
  <tr>
    <td>007</td>
    <td>20</td>
    <td>Research, Development, Test, and Evaluation</td>
  </tr>
  <tr>
    <td>007</td>
    <td>25</td>
    <td>Military Construction</td>
  </tr>
  <tr>
    <td>007</td>
    <td></td>
    <td>Department of Defense—Military Programs – continued</td>
  </tr>
  <tr>
    <td>007</td>
    <td>30</td>
    <td>Family Housing</td>
  </tr>
  <tr>
    <td>007</td>
    <td>37</td>
    <td>Special Foreign Currency Program</td>
  </tr>
  <tr>
    <td>007</td>
    <td>40</td>
    <td>Revolving and Management Funds</td>
  </tr>
  <tr>
    <td>007</td>
    <td>45</td>
    <td>Allowances</td>
  </tr>
  <tr>
    <td>007</td>
    <td>55</td>
    <td>Trust Funds</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>009</td>
    <td></td>
    <td>Department of Health and Human Services</td>
  </tr>
  <tr>
    <td>009</td>
    <td>10</td>
    <td>Food and Drug Administration</td>
  </tr>
  <tr>
    <td>009</td>
    <td>15</td>
    <td>Health Resources and Services Administration</td>
  </tr>
  <tr>
    <td>009</td>
    <td>17</td>
    <td>Indian Health Service</td>
  </tr>
  <tr>
    <td>009</td>
    <td>20</td>
    <td>Centers for Disease Control and Prevention</td>
  </tr>
  <tr>
    <td>009</td>
    <td>25</td>
    <td>National Institutes of Health</td>
  </tr>
  <tr>
    <td>009</td>
    <td>30</td>
    <td>Substance Abuse and Mental Health Services Administration</td>
  </tr>
  <tr>
    <td>009</td>
    <td>33</td>
    <td>Agency for Healthcare Research and Quality</td>
  </tr>
  <tr>
    <td>009</td>
    <td>35</td>
    <td>Health Resources Administration</td>
  </tr>
  <tr>
    <td>009</td>
    <td>38</td>
    <td>Centers for Medicare and Medicaid Services</td>
  </tr>
  <tr>
    <td>009</td>
    <td>70</td>
    <td>Administration for Children and Families</td>
  </tr>
  <tr>
    <td>009</td>
    <td>75</td>
    <td>Administration for Community Living</td>
  </tr>
  <tr>
    <td>009</td>
    <td>90</td>
    <td>Departmental Management</td>
  </tr>
  <tr>
    <td>009</td>
    <td>91</td>
    <td>Program Support Center</td>
  </tr>
  <tr>
    <td>009</td>
    <td>92</td>
    <td>Office of the Inspector General</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>010</td>
    <td></td>
    <td>Department of the Interior</td>
  </tr>
  <tr>
    <td>010</td>
    <td>04</td>
    <td>Bureau of Land Management</td>
  </tr>
  <tr>
    <td>010</td>
    <td>06</td>
    <td>Bureau of Ocean Energy Management</td>
  </tr>
  <tr>
    <td>010</td>
    <td>08</td>
    <td>Office of Surface Mining Reclamation and Enforcement</td>
  </tr>
  <tr>
    <td>010</td>
    <td>10</td>
    <td>Bureau of Reclamation</td>
  </tr>
  <tr>
    <td>010</td>
    <td>11</td>
    <td>Central Utah Project</td>
  </tr>
  <tr>
    <td>010</td>
    <td>12</td>
    <td>United States Geological Survey</td>
  </tr>
  <tr>
    <td>010</td>
    <td>14</td>
    <td>Bureau of Mines</td>
  </tr>
  <tr>
    <td>010</td>
    <td>18</td>
    <td>United States Fish and Wildlife Service</td>
  </tr>
  <tr>
    <td>010</td>
    <td>20</td>
    <td>National Biological Service</td>
  </tr>
  <tr>
    <td>010</td>
    <td>22</td>
    <td>Bureau of Safety and Environmental Enforcement</td>
  </tr>
  <tr>
    <td>010</td>
    <td>24</td>
    <td>National Park Service</td>
  </tr>
  <tr>
    <td>010</td>
    <td>76</td>
    <td>Bureau of Indian Affairs and Bureau of Indian Education</td>
  </tr>
  <tr>
    <td>010</td>
    <td>82</td>
    <td>Insular Affairs</td>
  </tr>
  <tr>
    <td>010</td>
    <td>84</td>
    <td>Departmental Offices</td>
  </tr>
  <tr>
    <td>010</td>
    <td>85</td>
    <td>Insular Affairs</td>
  </tr>
  <tr>
    <td>010</td>
    <td>86</td>
    <td>Office of the Solicitor</td>
  </tr>
  <tr>
    <td>010</td>
    <td>88</td>
    <td>Office of Inspector General</td>
  </tr>
  <tr>
    <td>010</td>
    <td>90</td>
    <td>Office of the Special Trustee for American Indians</td>
  </tr>
  <tr>
    <td>010</td>
    <td>92</td>
    <td>National Indian Gaming Commission</td>
  </tr>
  <tr>
    <td>010</td>
    <td>95</td>
    <td>Department-Wide Programs</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>011</td>
    <td></td>
    <td>Department of Justice</td>
  </tr>
  <tr>
    <td>011</td>
    <td>03</td>
    <td>General Administration</td>
  </tr>
  <tr>
    <td>011</td>
    <td>04</td>
    <td>United States Parole Commission</td>
  </tr>
  <tr>
    <td>011</td>
    <td>05</td>
    <td>Legal Activities and U.S. Marshals</td>
  </tr>
  <tr>
    <td>011</td>
    <td>06</td>
    <td>Radiation Exposure Compensation</td>
  </tr>
  <tr>
    <td>011</td>
    <td>07</td>
    <td>Interagency Law Enforcement</td>
  </tr>
  <tr>
    <td>011</td>
    <td>08</td>
    <td>National Security Division</td>
  </tr>
  <tr>
    <td>011</td>
    <td>10</td>
    <td>Federal Bureau of Investigation</td>
  </tr>
  <tr>
    <td>011</td>
    <td>12</td>
    <td>Drug Enforcement Administration</td>
  </tr>
  <tr>
    <td>011</td>
    <td>14</td>
    <td>Bureau of Alcohol, Tobacco, Firearms, and Explosives</td>
  </tr>
  <tr>
    <td>011</td>
    <td>20</td>
    <td>Federal Prison System</td>
  </tr>
  <tr>
    <td>011</td>
    <td>21</td>
    <td>Office of Justice Programs</td>
  </tr>
  <tr>
    <td>011</td>
    <td>30</td>
    <td>Violent Crime Reduction Trust Fund</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>012</td>
    <td></td>
    <td>Department of Labor</td>
  </tr>
  <tr>
    <td>012</td>
    <td>05</td>
    <td>Employment and Training Administration</td>
  </tr>
  <tr>
    <td>012</td>
    <td>10</td>
    <td>Office of the American Workplace</td>
  </tr>
  <tr>
    <td>012</td>
    <td>11</td>
    <td>Employee Benefits Security Administration</td>
  </tr>
  <tr>
    <td>012</td>
    <td>12</td>
    <td>Pension Benefit Guaranty Corporation</td>
  </tr>
  <tr>
    <td>012</td>
    <td>15</td>
    <td>Office of Workers' Compensation Programs</td>
  </tr>
  <tr>
    <td>012</td>
    <td>16</td>
    <td>Wage and Hour Division</td>
  </tr>
  <tr>
    <td>012</td>
    <td>17</td>
    <td>Employment Standards Administration</td>
  </tr>
  <tr>
    <td>012</td>
    <td>18</td>
    <td>Occupational Safety and Health Administration</td>
  </tr>
  <tr>
    <td>012</td>
    <td>19</td>
    <td>Mine Safety and Health Administration</td>
  </tr>
  <tr>
    <td>012</td>
    <td>20</td>
    <td>Bureau of Labor Statistics</td>
  </tr>
  <tr>
    <td>012</td>
    <td>22</td>
    <td>Office of Federal Contract Compliance Programs</td>
  </tr>
  <tr>
    <td>012</td>
    <td>23</td>
    <td>Office of Labor Management Standards</td>
  </tr>
  <tr>
    <td>012</td>
    <td>25</td>
    <td>Departmental Management</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>014</td>
    <td></td>
    <td>Department of State</td>
  </tr>
  <tr>
    <td>014</td>
    <td>05</td>
    <td>Administration of Foreign Affairs</td>
  </tr>
  <tr>
    <td>014</td>
    <td>10</td>
    <td>International Organizations and Conferences</td>
  </tr>
  <tr>
    <td>014</td>
    <td>15</td>
    <td>International Commissions</td>
  </tr>
  <tr>
    <td>014</td>
    <td>25</td>
    <td>Other</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>015</td>
    <td></td>
    <td>Department of the Treasury</td>
  </tr>
  <tr>
    <td>015</td>
    <td>04</td>
    <td>Financial Crimes Enforcement Network</td>
  </tr>
  <tr>
    <td>015</td>
    <td>05</td>
    <td>Departmental Offices</td>
  </tr>
  <tr>
    <td>015</td>
    <td>07</td>
    <td>Office of Revenue Sharing</td>
  </tr>
  <tr>
    <td>015</td>
    <td>09</td>
    <td>Interagency Law Enforcement</td>
  </tr>
  <tr>
    <td>015</td>
    <td>11</td>
    <td>Federal Financing Bank</td>
  </tr>
  <tr>
    <td>015</td>
    <td>12</td>
    <td>Fiscal Service</td>
  </tr>
  <tr>
    <td>015</td>
    <td>13</td>
    <td>Alcohol and Tobacco Tax and Trade Bureau</td>
  </tr>
  <tr>
    <td>015</td>
    <td>20</td>
    <td>Bureau of Engraving and Printing</td>
  </tr>
  <tr>
    <td>015</td>
    <td>25</td>
    <td>United States Mint</td>
  </tr>
  <tr>
    <td>015</td>
    <td></td>
    <td>Department of the Treasury – continued</td>
  </tr>
  <tr>
    <td>015</td>
    <td>45</td>
    <td>Internal Revenue Service</td>
  </tr>
  <tr>
    <td>015</td>
    <td>57</td>
    <td>Comptroller of the Currency</td>
  </tr>
  <tr>
    <td>015</td>
    <td>58</td>
    <td>Office of Thrift Supervision</td>
  </tr>
  <tr>
    <td>015</td>
    <td>60</td>
    <td>Interest on the Public Debt</td>
  </tr>
  <tr>
    <td>015</td>
    <td>99</td>
    <td>Department of the Treasury, activities</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td>Social Security Administration</td>
  </tr>
  <tr>
    <td>016</td>
    <td>00</td>
    <td>Social Security Administration</td>
  </tr>
  <tr>
    <td>017</td>
    <td>00</td>
    <td>Social Security Administration</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>018</td>
    <td></td>
    <td>Department of Education</td>
  </tr>
  <tr>
    <td>018</td>
    <td>10</td>
    <td>Office of Elementary and Secondary Education</td>
  </tr>
  <tr>
    <td>018</td>
    <td>12</td>
    <td>Office of Innovation and Improvement</td>
  </tr>
  <tr>
    <td>018</td>
    <td>15</td>
    <td>Office of English Language Acquisition</td>
  </tr>
  <tr>
    <td>018</td>
    <td>20</td>
    <td>Office of Special Education and Rehabilitative Services</td>
  </tr>
  <tr>
    <td>018</td>
    <td>30</td>
    <td>Office of Vocational and Adult Education</td>
  </tr>
  <tr>
    <td>018</td>
    <td>40</td>
    <td>Office of Postsecondary Education</td>
  </tr>
  <tr>
    <td>018</td>
    <td>45</td>
    <td>Office of Federal Student Aid</td>
  </tr>
  <tr>
    <td>018</td>
    <td>50</td>
    <td>Institute of Education Sciences</td>
  </tr>
  <tr>
    <td>018</td>
    <td>80</td>
    <td>Departmental Management</td>
  </tr>
  <tr>
    <td>018</td>
    <td>85</td>
    <td>Hurricane Education Recovery</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>019</td>
    <td></td>
    <td>Department of Energy</td>
  </tr>
  <tr>
    <td>019</td>
    <td>05</td>
    <td>National Nuclear Security Administration</td>
  </tr>
  <tr>
    <td>019</td>
    <td>10</td>
    <td>Environmental and Other Defense Activities</td>
  </tr>
  <tr>
    <td>019</td>
    <td>20</td>
    <td>Energy Programs</td>
  </tr>
  <tr>
    <td>019</td>
    <td>50</td>
    <td>Power Marketing Administration</td>
  </tr>
  <tr>
    <td>019</td>
    <td>60</td>
    <td>Departmental Administration</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>020</td>
    <td>00</td>
    <td>Environmental Protection Agency</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>021</td>
    <td></td>
    <td>Department of Transportation</td>
  </tr>
  <tr>
    <td>021</td>
    <td>04</td>
    <td>Office of the Secretary</td>
  </tr>
  <tr>
    <td>021</td>
    <td>12</td>
    <td>Federal Aviation Administration</td>
  </tr>
  <tr>
    <td>021</td>
    <td>15</td>
    <td>Federal Highway Administration</td>
  </tr>
  <tr>
    <td>021</td>
    <td>17</td>
    <td>Federal Motor Carrier Safety Administration</td>
  </tr>
  <tr>
    <td>021</td>
    <td>18</td>
    <td>National Highway Traffic Safety Administration</td>
  </tr>
  <tr>
    <td>021</td>
    <td>27</td>
    <td>Federal Railroad Administration</td>
  </tr>
  <tr>
    <td>021</td>
    <td>36</td>
    <td>Federal Transit Administration</td>
  </tr>
  <tr>
    <td>021</td>
    <td>40</td>
    <td>Saint Lawrence Seaway Development Corporation</td>
  </tr>
  <tr>
    <td>021</td>
    <td>50</td>
    <td>Pipeline and Hazardous Materials Safety Administration</td>
  </tr>
  <tr>
    <td>021</td>
    <td>56</td>
    <td>Office of Inspector General</td>
  </tr>
  <tr>
    <td>021</td>
    <td>61</td>
    <td>Surface Transportation Board</td>
  </tr>
  <tr>
    <td>021</td>
    <td>65</td>
    <td>Bureau of Transportation Statistics</td>
  </tr>
  <tr>
    <td>021</td>
    <td></td>
    <td>Department of Transportation – continued</td>
  </tr>
  <tr>
    <td>021</td>
    <td>70</td>
    <td>Maritime Administration</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>023</td>
    <td></td>
    <td>General Services Administration</td>
  </tr>
  <tr>
    <td>023</td>
    <td>05</td>
    <td>Real Property Activities</td>
  </tr>
  <tr>
    <td>023</td>
    <td>10</td>
    <td>Supply and Technology Activities</td>
  </tr>
  <tr>
    <td>023</td>
    <td>30</td>
    <td>General Activities</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>024</td>
    <td></td>
    <td>Department of Homeland Security</td>
  </tr>
  <tr>
    <td>024</td>
    <td>10</td>
    <td>Departmental Management and Operations</td>
  </tr>
  <tr>
    <td>024</td>
    <td>20</td>
    <td>Office of the Inspector General</td>
  </tr>
  <tr>
    <td>024</td>
    <td>30</td>
    <td>Citizenship and Immigration Services</td>
  </tr>
  <tr>
    <td>024</td>
    <td>40</td>
    <td>United States Secret Service</td>
  </tr>
  <tr>
    <td>024</td>
    <td>43</td>
    <td>Office of the Under Secretary for Border and Transportation Security</td>
  </tr>
  <tr>
    <td>024</td>
    <td>45</td>
    <td>Transportation Security Administration</td>
  </tr>
  <tr>
    <td>024</td>
    <td>49</td>
    <td>Federal Law Enforcement Training Center</td>
  </tr>
  <tr>
    <td>024</td>
    <td>50</td>
    <td>Security, Enforcement, and Investigations</td>
  </tr>
  <tr>
    <td>024</td>
    <td>55</td>
    <td>Immigration and Customs Enforcement</td>
  </tr>
  <tr>
    <td>024</td>
    <td>58</td>
    <td>U.S. Customs and Border Protection</td>
  </tr>
  <tr>
    <td>024</td>
    <td>60</td>
    <td>United States Coast Guard</td>
  </tr>
  <tr>
    <td>024</td>
    <td>65</td>
    <td>National Protection and Programs Directorate</td>
  </tr>
  <tr>
    <td>024</td>
    <td>70</td>
    <td>Federal Emergency Management Agency</td>
  </tr>
  <tr>
    <td>024</td>
    <td>80</td>
    <td>Science and Technology</td>
  </tr>
  <tr>
    <td>024</td>
    <td>85</td>
    <td>Domestic Nuclear Detection Office</td>
  </tr>
  <tr>
    <td>024</td>
    <td>90</td>
    <td>Information Analysis and Infrastructure Protection</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>025</td>
    <td></td>
    <td>Department of Housing and Urban Development</td>
  </tr>
  <tr>
    <td>025</td>
    <td>03</td>
    <td>Public and Indian Housing Programs</td>
  </tr>
  <tr>
    <td>025</td>
    <td>06</td>
    <td>Community Planning and Development</td>
  </tr>
  <tr>
    <td>025</td>
    <td>09</td>
    <td>Housing Programs</td>
  </tr>
  <tr>
    <td>025</td>
    <td>12</td>
    <td>Government National Mortgage Association</td>
  </tr>
  <tr>
    <td>025</td>
    <td>28</td>
    <td>Policy Development and Research</td>
  </tr>
  <tr>
    <td>025</td>
    <td>29</td>
    <td>Fair Housing and Equal Opportunity</td>
  </tr>
  <tr>
    <td>025</td>
    <td>32</td>
    <td>Office of Lead Hazard Control and Healthy Homes</td>
  </tr>
  <tr>
    <td>025</td>
    <td>35</td>
    <td>Management and Administration</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>026</td>
    <td>00</td>
    <td>National Aeronautics and Space Administration</td>
  </tr>
  <tr>
    <td>027</td>
    <td>00</td>
    <td>Office of Personnel Management</td>
  </tr>
  <tr>
    <td>028</td>
    <td>00</td>
    <td>Small Business Administration</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>029</td>
    <td></td>
    <td>Department of Veterans Affairs</td>
  </tr>
  <tr>
    <td>029</td>
    <td>15</td>
    <td>Veterans Health Administration</td>
  </tr>
  <tr>
    <td>029</td>
    <td>25</td>
    <td>Benefits Programs</td>
  </tr>
  <tr>
    <td>029</td>
    <td>40</td>
    <td>Departmental Administration</td>
  </tr>
  <tr>
    <td>100</td>
    <td></td>
    <td>Executive Office of the President</td>
  </tr>
  <tr>
    <td>100</td>
    <td>05</td>
    <td>The White House</td>
  </tr>
  <tr>
    <td>100</td>
    <td>10</td>
    <td>Executive Residence at the White House</td>
  </tr>
  <tr>
    <td>100</td>
    <td>15</td>
    <td>Special Assistance to the President and the Official Residence of the Vice President</td>
  </tr>
  <tr>
    <td>100</td>
    <td>20</td>
    <td>Council of Economic Advisers</td>
  </tr>
  <tr>
    <td>100</td>
    <td>25</td>
    <td>Council on Environmental Quality and Office of Environmental Quality</td>
  </tr>
  <tr>
    <td>100</td>
    <td>26</td>
    <td>Council on International Economic Policy</td>
  </tr>
  <tr>
    <td>100</td>
    <td>27</td>
    <td>Council on Wage and Price Stability</td>
  </tr>
  <tr>
    <td>100</td>
    <td>30</td>
    <td>Office of Policy Development</td>
  </tr>
  <tr>
    <td>100</td>
    <td>35</td>
    <td>National Security Council and Homeland Security Council</td>
  </tr>
  <tr>
    <td>100</td>
    <td>40</td>
    <td>National Space Council</td>
  </tr>
  <tr>
    <td>100</td>
    <td>45</td>
    <td>National Critical Materials Council</td>
  </tr>
  <tr>
    <td>100</td>
    <td>50</td>
    <td>Office of Administration</td>
  </tr>
  <tr>
    <td>100</td>
    <td>51</td>
    <td>Armstrong Resolution</td>
  </tr>
  <tr>
    <td>100</td>
    <td>53</td>
    <td>Office of National Service</td>
  </tr>
  <tr>
    <td>100</td>
    <td>55</td>
    <td>Office of Management and Budget</td>
  </tr>
  <tr>
    <td>100</td>
    <td>60</td>
    <td>Office of National Drug Control Policy</td>
  </tr>
  <tr>
    <td>100</td>
    <td>65</td>
    <td>Office of Science and Technology Policy</td>
  </tr>
  <tr>
    <td>100</td>
    <td>70</td>
    <td>Office of the United States Trade Representative</td>
  </tr>
  <tr>
    <td>100</td>
    <td>75</td>
    <td>Office of Telecommunications Policy</td>
  </tr>
  <tr>
    <td>100</td>
    <td>80</td>
    <td>The Points of Light Foundation</td>
  </tr>
  <tr>
    <td>100</td>
    <td>85</td>
    <td>White House Conference for a Drug Free America</td>
  </tr>
  <tr>
    <td>100</td>
    <td>90</td>
    <td>Special Action Office for Drug Abuse Prevention</td>
  </tr>
  <tr>
    <td>100</td>
    <td>91</td>
    <td>Office of Drug Abuse Policy</td>
  </tr>
  <tr>
    <td>100</td>
    <td>95</td>
    <td>Unanticipated Needs</td>
  </tr>
  <tr>
    <td>100</td>
    <td>97</td>
    <td>Expenses of Management Improvement</td>
  </tr>
  <tr>
    <td>100</td>
    <td>98</td>
    <td>Presidential Transition</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td>Other Independent Agencies</td>
  </tr>
  <tr>
    <td>154</td>
    <td>00</td>
    <td>Federal Drug Control Programs</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>184</td>
    <td></td>
    <td>International Assistance Programs</td>
  </tr>
  <tr>
    <td>184</td>
    <td>03</td>
    <td>Millennium Challenge Corporation</td>
  </tr>
  <tr>
    <td>184</td>
    <td>05</td>
    <td>International Security Assistance</td>
  </tr>
  <tr>
    <td>184</td>
    <td>10</td>
    <td>Multilateral Assistance</td>
  </tr>
  <tr>
    <td>184</td>
    <td>15</td>
    <td>Agency for International Development</td>
  </tr>
  <tr>
    <td>184</td>
    <td>20</td>
    <td>Overseas Private Investment Corporation</td>
  </tr>
  <tr>
    <td>184</td>
    <td>25</td>
    <td>Trade and Development Agency</td>
  </tr>
  <tr>
    <td>184</td>
    <td>35</td>
    <td>Peace Corps</td>
  </tr>
  <tr>
    <td>184</td>
    <td>40</td>
    <td>Inter-American Foundation</td>
  </tr>
  <tr>
    <td>184</td>
    <td>50</td>
    <td>African Development Foundation</td>
  </tr>
  <tr>
    <td>184</td>
    <td>60</td>
    <td>International Monetary Programs</td>
  </tr>
  <tr>
    <td>184</td>
    <td>70</td>
    <td>Military Sales Program</td>
  </tr>
  <tr>
    <td>184</td>
    <td></td>
    <td>International Assistance Programs – continued</td>
  </tr>
  <tr>
    <td>184</td>
    <td>75</td>
    <td>Special Assistance Initiatives</td>
  </tr>
  <tr>
    <td>184</td>
    <td>77</td>
    <td>Special Assistance for Israel</td>
  </tr>
  <tr>
    <td>184</td>
    <td>80</td>
    <td>International Commodity Agreements</td>
  </tr>
  <tr>
    <td>184</td>
    <td>82</td>
    <td>Economic Stabilization Activities</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>200</td>
    <td></td>
    <td>Other Defense Civil Programs</td>
  </tr>
  <tr>
    <td>200</td>
    <td>05</td>
    <td>Military Retirement</td>
  </tr>
  <tr>
    <td>200</td>
    <td>07</td>
    <td>Retiree Health Care</td>
  </tr>
  <tr>
    <td>200</td>
    <td>10</td>
    <td>Educational Benefits</td>
  </tr>
  <tr>
    <td>200</td>
    <td>15</td>
    <td>American Battle Monuments Commission</td>
  </tr>
  <tr>
    <td>200</td>
    <td>20</td>
    <td>Armed Forces Retirement Home</td>
  </tr>
  <tr>
    <td>200</td>
    <td>25</td>
    <td>Cemeterial Expenses</td>
  </tr>
  <tr>
    <td>200</td>
    <td>30</td>
    <td>Forest and Wildlife Conservation, Military Reservations</td>
  </tr>
  <tr>
    <td>200</td>
    <td>35</td>
    <td>The Mildred and Claude Pepper Foundation</td>
  </tr>
  <tr>
    <td>200</td>
    <td>40</td>
    <td>Ryukyu Islands, Army</td>
  </tr>
  <tr>
    <td>200</td>
    <td>45</td>
    <td>Selective Service System</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>202</td>
    <td>00</td>
    <td>Corps of Engineers—Civil Works</td>
  </tr>
  <tr>
    <td>301</td>
    <td>00</td>
    <td>ACTION</td>
  </tr>
  <tr>
    <td>302</td>
    <td>00</td>
    <td>Administrative Conference of the United States</td>
  </tr>
  <tr>
    <td>303</td>
    <td>00</td>
    <td>Advisory Commission on Conferences in Ocean Shipping</td>
  </tr>
  <tr>
    <td>304</td>
    <td>00</td>
    <td>Advisory Commission on Intergovernmental Relations</td>
  </tr>
  <tr>
    <td>305</td>
    <td>00</td>
    <td>Advisory Committee on Federal Pay</td>
  </tr>
  <tr>
    <td>306</td>
    <td>00</td>
    <td>Advisory Council on Historic Preservation</td>
  </tr>
  <tr>
    <td>308</td>
    <td>00</td>
    <td>American Revolution Bicentennial Administration</td>
  </tr>
  <tr>
    <td>309</td>
    <td>00</td>
    <td>Appalachian Regional Commission</td>
  </tr>
  <tr>
    <td>310</td>
    <td>00</td>
    <td>Architectural and Transportation Barriers Compliance Board</td>
  </tr>
  <tr>
    <td>312</td>
    <td>00</td>
    <td>Aviation Safety Commission</td>
  </tr>
  <tr>
    <td>313</td>
    <td>00</td>
    <td>Barry Goldwater Scholarship and Excellence in Education Foundation</td>
  </tr>
  <tr>
    <td>315</td>
    <td>00</td>
    <td>Cabinet Comm on Opportunities for Spanish Speaking</td>
  </tr>
  <tr>
    <td>316</td>
    <td>00</td>
    <td>Central Intelligence Agency</td>
  </tr>
  <tr>
    <td>318</td>
    <td>00</td>
    <td>Christopher Columbus Quincentennary Jubilee Commission</td>
  </tr>
  <tr>
    <td>319</td>
    <td>00</td>
    <td>Citizens’ Commission on Public Service and Compensation</td>
  </tr>
  <tr>
    <td>321</td>
    <td>00</td>
    <td>Commission for the Preservation of America’s Heritage Abroad</td>
  </tr>
  <tr>
    <td>322</td>
    <td>00</td>
    <td>Commission for the Study of International Migration and Cooperative Economic Development</td>
  </tr>
  <tr>
    <td>323</td>
    <td>00</td>
    <td>Commission of Fine Arts</td>
  </tr>
  <tr>
    <td>324</td>
    <td>00</td>
    <td>Commission on Agricultural Workers</td>
  </tr>
  <tr>
    <td>325</td>
    <td>00</td>
    <td>Commission on American Shipbuilding</td>
  </tr>
  <tr>
    <td>326</td>
    <td>00</td>
    <td>Commission on Civil Rights</td>
  </tr>
  <tr>
    <td>327</td>
    <td>00</td>
    <td>Commission on Education of the Deaf</td>
  </tr>
  <tr>
    <td>329</td>
    <td>00</td>
    <td>Commission on Federal Paperwork</td>
  </tr>
  <tr>
    <td>330</td>
    <td>00</td>
    <td>Commission on Government Procurement</td>
  </tr>
  <tr>
    <td>331</td>
    <td>00</td>
    <td>Commission on National and Community Service</td>
  </tr>
  <tr>
    <td>332</td>
    <td>00</td>
    <td>Commission on Highway Beautification</td>
  </tr>
  <tr>
    <td>333</td>
    <td>00</td>
    <td>Commission on the Bicentennial of the U.S. Constitution</td>
  </tr>
  <tr>
    <td>334</td>
    <td>00</td>
    <td>Comm on Org of the Gov for Conduct of Foreign Poli</td>
  </tr>
  <tr>
    <td>335</td>
    <td>00</td>
    <td>Comm on Review of National Policy Toward Gambling</td>
  </tr>
  <tr>
    <td>336</td>
    <td>00</td>
    <td>Commission on the Ukraine Famine</td>
  </tr>
  <tr>
    <td>338</td>
    <td>00</td>
    <td>Committee for Purchase from People who are Blind or Severely Disabled, activities</td>
  </tr>
  <tr>
    <td>339</td>
    <td>00</td>
    <td>Commodity Futures Trading Commission</td>
  </tr>
  <tr>
    <td>340</td>
    <td>00</td>
    <td>Community Development Credit Unions Revolving Fund</td>
  </tr>
  <tr>
    <td>341</td>
    <td>00</td>
    <td>Community Services Administration</td>
  </tr>
  <tr>
    <td>342</td>
    <td>00</td>
    <td>Construction Corregidor-Bataan Memorial</td>
  </tr>
  <tr>
    <td>343</td>
    <td>00</td>
    <td>Consumer Product Safety Commission</td>
  </tr>
  <tr>
    <td>344</td>
    <td>00</td>
    <td>Corporation for Public Broadcasting</td>
  </tr>
  <tr>
    <td>345</td>
    <td>00</td>
    <td>United States Court of Appeals for Veterans Claims</td>
  </tr>
  <tr>
    <td>346</td>
    <td>00</td>
    <td>Defense Manpower Commission</td>
  </tr>
  <tr>
    <td>347</td>
    <td>00</td>
    <td>Defense Nuclear Facilities Safety Board</td>
  </tr>
  <tr>
    <td>348</td>
    <td>00</td>
    <td>Delaware River Basin Commission</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>349</td>
    <td></td>
    <td>District of Columbia</td>
  </tr>
  <tr>
    <td>349</td>
    <td>10</td>
    <td>District of Columbia Courts</td>
  </tr>
  <tr>
    <td>349</td>
    <td>20</td>
    <td>District of Columbia Corrections</td>
  </tr>
  <tr>
    <td>349</td>
    <td>30</td>
    <td>District of Columbia General and Special Payments</td>
  </tr>
  <tr>
    <td>349</td>
    <td>40</td>
    <td>District of Columbia Financing</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>350</td>
    <td>00</td>
    <td>Equal Employment Opportunity Commission</td>
  </tr>
  <tr>
    <td>351</td>
    <td>00</td>
    <td>Export-Import Bank of the United States</td>
  </tr>
  <tr>
    <td>352</td>
    <td>00</td>
    <td>Farm Credit Administration</td>
  </tr>
  <tr>
    <td>353</td>
    <td>00</td>
    <td>Farm Credit System Assistance Board</td>
  </tr>
  <tr>
    <td>354</td>
    <td>00</td>
    <td>Farm Credit System Financial Assistance Corporation</td>
  </tr>
  <tr>
    <td>355</td>
    <td>00</td>
    <td>Farm Credit System Insurance Corporation</td>
  </tr>
  <tr>
    <td>356</td>
    <td>00</td>
    <td>Federal Communications Commission</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>357</td>
    <td></td>
    <td>Federal Deposit Insurance Corporation</td>
  </tr>
  <tr>
    <td>357</td>
    <td>10</td>
    <td>Bank Insurance</td>
  </tr>
  <tr>
    <td>357</td>
    <td>20</td>
    <td>Deposit Insurance</td>
  </tr>
  <tr>
    <td>357</td>
    <td>30</td>
    <td>FSLIC Resolution</td>
  </tr>
  <tr>
    <td>357</td>
    <td>35</td>
    <td>Orderly Liquidation</td>
  </tr>
  <tr>
    <td>357</td>
    <td>40</td>
    <td>FDIC–Office of Inspector General</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>360</td>
    <td>00</td>
    <td>Federal Election Commission</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>362</td>
    <td></td>
    <td>Federal Financial Institutions Examination Council</td>
  </tr>
  <tr>
    <td>362</td>
    <td>20</td>
    <td>Federal Financial Institutions Examination Council Appraisal Subcommittee</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>364</td>
    <td>00</td>
    <td>Federal Housing Finance Board</td>
  </tr>
  <tr>
    <td>365</td>
    <td>00</td>
    <td>Federal Labor Relations Authority</td>
  </tr>
  <tr>
    <td>366</td>
    <td>00</td>
    <td>Federal Maritime Commission</td>
  </tr>
  <tr>
    <td>367</td>
    <td>00</td>
    <td>Federal Mediation and Conciliation Service</td>
  </tr>
  <tr>
    <td>368</td>
    <td>00</td>
    <td>Federal Mine Safety and Health Review Commission</td>
  </tr>
  <tr>
    <td>369</td>
    <td>00</td>
    <td>Federal Retirement Thrift Investment Board</td>
  </tr>
  <tr>
    <td>370</td>
    <td>00</td>
    <td>Federal Trade Commission</td>
  </tr>
  <tr>
    <td>371</td>
    <td>00</td>
    <td>Franklin Delano Roosevelt Memorial Commission</td>
  </tr>
  <tr>
    <td>372</td>
    <td>00</td>
    <td>Harry S Truman Scholarship Foundation</td>
  </tr>
  <tr>
    <td>373</td>
    <td>00</td>
    <td>Institute of American Indian and Alaska Native Culture and Arts Development</td>
  </tr>
  <tr>
    <td>376</td>
    <td>00</td>
    <td>United States Interagency Council on Homelessness</td>
  </tr>
  <tr>
    <td>377</td>
    <td>00</td>
    <td>International Cultural and Trade Center Commission</td>
  </tr>
  <tr>
    <td>378</td>
    <td>00</td>
    <td>International Trade Commission</td>
  </tr>
  <tr>
    <td>379</td>
    <td>00</td>
    <td>Interstate Commerce Commission</td>
  </tr>
  <tr>
    <td>380</td>
    <td>00</td>
    <td>Interstate Commission on the Potomac River Basin</td>
  </tr>
  <tr>
    <td>381</td>
    <td>00</td>
    <td>James Madison Memorial Fellowship Foundation</td>
  </tr>
  <tr>
    <td>382</td>
    <td>00</td>
    <td>Japan-United States Friendship Commission</td>
  </tr>
  <tr>
    <td>383</td>
    <td>00</td>
    <td>Joint Commission on the Coinage</td>
  </tr>
  <tr>
    <td>384</td>
    <td>00</td>
    <td>Joint Federal-State Land Use Planning Commission</td>
  </tr>
  <tr>
    <td>385</td>
    <td>00</td>
    <td>Legal Services Corporation</td>
  </tr>
  <tr>
    <td>386</td>
    <td>00</td>
    <td>Lowell Historical Canyon District Commission</td>
  </tr>
  <tr>
    <td>387</td>
    <td>00</td>
    <td>Marine Mammal Commission</td>
  </tr>
  <tr>
    <td>388</td>
    <td>00</td>
    <td>Martin Luther King, Jr. Federal Holiday Commission</td>
  </tr>
  <tr>
    <td>389</td>
    <td>00</td>
    <td>Merit Systems Protection Board</td>
  </tr>
  <tr>
    <td>390</td>
    <td>00</td>
    <td>Motor Carrier Ratemaking Study Commission</td>
  </tr>
  <tr>
    <td>391</td>
    <td>00</td>
    <td>National Afro-American History and Culture Commission</td>
  </tr>
  <tr>
    <td>392</td>
    <td>00</td>
    <td>National Alcohol Fuels Commission</td>
  </tr>
  <tr>
    <td>393</td>
    <td>00</td>
    <td>National Archives and Records Administration</td>
  </tr>
  <tr>
    <td>394</td>
    <td>00</td>
    <td>National Capital Planning Commission</td>
  </tr>
  <tr>
    <td>395</td>
    <td>00</td>
    <td>National Commission on American Indian, Alaska Native, and Native Hawaiian Housing</td>
  </tr>
  <tr>
    <td>396</td>
    <td>00</td>
    <td>Nat. Comm. for the Review of Federal and State Laws</td>
  </tr>
  <tr>
    <td>397</td>
    <td>00</td>
    <td>National Commission on Agricultural Finance</td>
  </tr>
  <tr>
    <td>400</td>
    <td>00</td>
    <td>National Commission on Libraries and Information Science</td>
  </tr>
  <tr>
    <td>401</td>
    <td>00</td>
    <td>National Commission on Migrant Education</td>
  </tr>
  <tr>
    <td>402</td>
    <td>00</td>
    <td>National Commission on Responsibilities for Financing Postsecondary Education</td>
  </tr>
  <tr>
    <td>403</td>
    <td>00</td>
    <td>National Commission on Severely Distressed Public Housing</td>
  </tr>
  <tr>
    <td>404</td>
    <td>00</td>
    <td>National Commission on Social Security</td>
  </tr>
  <tr>
    <td>405</td>
    <td>00</td>
    <td>National Commission on Student Financial Assist.</td>
  </tr>
  <tr>
    <td>406</td>
    <td>00</td>
    <td>National Commission on Supplies and Shortages</td>
  </tr>
  <tr>
    <td>407</td>
    <td>00</td>
    <td>Nat Comm on Financing of Postsecondary Education</td>
  </tr>
  <tr>
    <td>408</td>
    <td>00</td>
    <td>Nat Comm on the International Year of the Child</td>
  </tr>
  <tr>
    <td>409</td>
    <td>00</td>
    <td>Nat Comm on the Observance of Inter Year of Women</td>
  </tr>
  <tr>
    <td>410</td>
    <td>00</td>
    <td>National Commission on Water Quality</td>
  </tr>
  <tr>
    <td>411</td>
    <td>00</td>
    <td>National Commission to Prevent Infant Mortality</td>
  </tr>
  <tr>
    <td>412</td>
    <td>00</td>
    <td>National Commission on Marihuana and Drug Abuse</td>
  </tr>
  <tr>
    <td>413</td>
    <td>00</td>
    <td>National Council on Disability</td>
  </tr>
  <tr>
    <td>414</td>
    <td>00</td>
    <td>National Council on Public Works Improvement</td>
  </tr>
  <tr>
    <td>415</td>
    <td>00</td>
    <td>National Credit Union Administration</td>
  </tr>
  <tr>
    <td>416</td>
    <td>00</td>
    <td>National Economic Commission, Salaries & Expenses</td>
  </tr>
  <tr>
    <td>417</td>
    <td>00</td>
    <td>National Endowment for the Arts</td>
  </tr>
  <tr>
    <td>418</td>
    <td>00</td>
    <td>National Endowment for the Humanities</td>
  </tr>
  <tr>
    <td>419</td>
    <td>00</td>
    <td>National Institute of Building Sciences</td>
  </tr>
  <tr>
    <td>420</td>
    <td>00</td>
    <td>National Labor Relations Board</td>
  </tr>
  <tr>
    <td>421</td>
    <td>00</td>
    <td>National Mediation Board</td>
  </tr>
  <tr>
    <td>422</td>
    <td>00</td>
    <td>National Science Foundation</td>
  </tr>
  <tr>
    <td>423</td>
    <td>00</td>
    <td>National Transportation Policy Study Commission</td>
  </tr>
  <tr>
    <td>424</td>
    <td>00</td>
    <td>National Transportation Safety Board</td>
  </tr>
  <tr>
    <td>425</td>
    <td>00</td>
    <td>National Water Commission</td>
  </tr>
  <tr>
    <td>426</td>
    <td>00</td>
    <td>Native Hawaiians Study Commission</td>
  </tr>
  <tr>
    <td>428</td>
    <td>00</td>
    <td>Neighborhood Reinvestment Corporation</td>
  </tr>
  <tr>
    <td>429</td>
    <td>00</td>
    <td>Nuclear Regulatory Commission</td>
  </tr>
  <tr>
    <td>430</td>
    <td>00</td>
    <td>Nuclear Safety Oversight Committee</td>
  </tr>
  <tr>
    <td>431</td>
    <td>00</td>
    <td>Nuclear Waste Technical Review Board</td>
  </tr>
  <tr>
    <td>432</td>
    <td>00</td>
    <td>Occupational Safety and Health Review Commission</td>
  </tr>
  <tr>
    <td>434</td>
    <td>00</td>
    <td>Office of Government Ethics</td>
  </tr>
  <tr>
    <td>435</td>
    <td>00</td>
    <td>Office of Navajo and Hopi Indian Relocation</td>
  </tr>
  <tr>
    <td>436</td>
    <td>00</td>
    <td>Office of Special Counsel</td>
  </tr>
  <tr>
    <td>437</td>
    <td>00</td>
    <td>Office of the Nuclear Waste Negotiator</td>
  </tr>
  <tr>
    <td>438</td>
    <td>00</td>
    <td>Panama Canal Commission</td>
  </tr>
  <tr>
    <td>440</td>
    <td>00</td>
    <td>Postal Service</td>
  </tr>
  <tr>
    <td>441</td>
    <td>00</td>
    <td>Pres. Comm. for Study of Ethical Problems in Medicine</td>
  </tr>
  <tr>
    <td>442</td>
    <td>00</td>
    <td>President’s Commission on Catastrophic Nuclear Accidents</td>
  </tr>
  <tr>
    <td>443</td>
    <td>00</td>
    <td>President’s Commission on Pension Policy</td>
  </tr>
  <tr>
    <td>444</td>
    <td>00</td>
    <td>President's Council on Youth Opportunities</td>
  </tr>
  <tr>
    <td>445</td>
    <td>00</td>
    <td>Privacy Protection Study Commission</td>
  </tr>
  <tr>
    <td>446</td>
    <td>00</td>
    <td>Railroad Retirement Board</td>
  </tr>
  <tr>
    <td>447</td>
    <td>00</td>
    <td>Renegotiation Board</td>
  </tr>
  <tr>
    <td>448</td>
    <td>00</td>
    <td>Resolution Trust Corporation</td>
  </tr>
  <tr>
    <td>449</td>
    <td>00</td>
    <td>Securities and Exchange Commission</td>
  </tr>
  <tr>
    <td>450</td>
    <td>00</td>
    <td>Select Commission on Immigration & Refugee Policy</td>
  </tr>
  <tr>
    <td>452</td>
    <td>00</td>
    <td>Smithsonian Institution</td>
  </tr>
  <tr>
    <td>453</td>
    <td>00</td>
    <td>State Justice Institute</td>
  </tr>
  <tr>
    <td>454</td>
    <td>00</td>
    <td>Susquehanna River Basin Commission</td>
  </tr>
  <tr>
    <td>455</td>
    <td>00</td>
    <td>Tennessee Valley Authority</td>
  </tr>
  <tr>
    <td>456</td>
    <td>00</td>
    <td>United States Holocaust Memorial Museum</td>
  </tr>
  <tr>
    <td>458</td>
    <td>00</td>
    <td>United States Institute of Peace</td>
  </tr>
  <tr>
    <td>459</td>
    <td>00</td>
    <td>United States Metric Board</td>
  </tr>
  <tr>
    <td>460</td>
    <td>00</td>
    <td>United States Railway Association</td>
  </tr>
  <tr>
    <td>462</td>
    <td>00</td>
    <td>United States Synthetic Fuels Corporation</td>
  </tr>
  <tr>
    <td>463</td>
    <td>00</td>
    <td>Washington Metropolitan Area Transit Authority</td>
  </tr>
  <tr>
    <td>464</td>
    <td>00</td>
    <td>Water Resources Council</td>
  </tr>
  <tr>
    <td>465</td>
    <td>00</td>
    <td>Christopher Columbus Fellowship Foundation</td>
  </tr>
  <tr>
    <td>466</td>
    <td>00</td>
    <td>Community Investment Program</td>
  </tr>
  <tr>
    <td>467</td>
    <td>00</td>
    <td>Intelligence Community Management Account</td>
  </tr>
  <tr>
    <td>468</td>
    <td>00</td>
    <td>Affordable Housing and Bank Enterprise (FDIC)</td>
  </tr>
  <tr>
    <td>469</td>
    <td>00</td>
    <td>Joint Federal-State Commission on Policies and Programs Affecting Alaska Natives</td>
  </tr>
  <tr>
    <td>470</td>
    <td>00</td>
    <td>National Advisory Council on the Public Service</td>
  </tr>
  <tr>
    <td>474</td>
    <td>00</td>
    <td>Institute of Museum and Library Services</td>
  </tr>
  <tr>
    <td>475</td>
    <td>00</td>
    <td>Thomas Jefferson Commemoration Commission</td>
  </tr>
  <tr>
    <td>476</td>
    <td>00</td>
    <td>United Mine Workers of America Benefit Funds</td>
  </tr>
  <tr>
    <td>477</td>
    <td>00</td>
    <td>Emergency Loan Guarantee Board</td>
  </tr>
  <tr>
    <td>478</td>
    <td>00</td>
    <td>National Council on Indian Opportunities</td>
  </tr>
  <tr>
    <td>479</td>
    <td>00</td>
    <td>Military Compensation and Retirement Modernization Commission</td>
  </tr>
  <tr>
    <td>482</td>
    <td>00</td>
    <td>National Commission on Cost of Higher Education</td>
  </tr>
  <tr>
    <td>483</td>
    <td>00</td>
    <td>National Commission on Financial Institutions Reform, Recovery, and Enforcement</td>
  </tr>
  <tr>
    <td>484</td>
    <td>00</td>
    <td>National Commission on Independent Higher Education</td>
  </tr>
  <tr>
    <td>485</td>
    <td>00</td>
    <td>Corporation for National and Community Service</td>
  </tr>
  <tr>
    <td>486</td>
    <td>00</td>
    <td>United States Enrichment Corporation Fund</td>
  </tr>
  <tr>
    <td>487</td>
    <td>00</td>
    <td>Morris K. Udall and Stewart L. Udall Foundation</td>
  </tr>
  <tr>
    <td>491</td>
    <td>00</td>
    <td>JFK Assassination Records Review Board</td>
  </tr>
  <tr>
    <td>492</td>
    <td>00</td>
    <td>National Education Goals Panel</td>
  </tr>
  <tr>
    <td>493</td>
    <td>00</td>
    <td>National Education Standards and Improvement Council</td>
  </tr>
  <tr>
    <td>499</td>
    <td>00</td>
    <td>Ounce of Prevention Council</td>
  </tr>
  <tr>
    <td>500</td>
    <td>00</td>
    <td>National Bankruptcy Review Commission</td>
  </tr>
  <tr>
    <td>505</td>
    <td>00</td>
    <td>Other Commissions and Boards</td>
  </tr>
  <tr>
    <td>506</td>
    <td>00</td>
    <td>River Basin Commissions</td>
  </tr>
  <tr>
    <td>510</td>
    <td>00</td>
    <td>Chemical Safety and Hazard Investigation Board</td>
  </tr>
  <tr>
    <td>511</td>
    <td>00</td>
    <td>Court Services and Offender Supervision Agency for the District of Columbia</td>
  </tr>
  <tr>
    <td>512</td>
    <td>00</td>
    <td>Presidio Trust</td>
  </tr>
  <tr>
    <td>513</td>
    <td>00</td>
    <td>Denali Commission</td>
  </tr>
  <tr>
    <td>514</td>
    <td>00</td>
    <td>Broadcasting Board of Governors</td>
  </tr>
  <tr>
    <td>515</td>
    <td>00</td>
    <td>Commission on Ocean Policy</td>
  </tr>
  <tr>
    <td>516</td>
    <td>00</td>
    <td>Oklahoma City National Memorial Trust</td>
  </tr>
  <tr>
    <td>517</td>
    <td>00</td>
    <td>Delta Regional Authority</td>
  </tr>
  <tr>
    <td>518</td>
    <td>00</td>
    <td>National Veterans Business Development Corporation</td>
  </tr>
  <tr>
    <td>519</td>
    <td>00</td>
    <td>Vietnam Education Foundation</td>
  </tr>
  <tr>
    <td>521</td>
    <td>00</td>
    <td>United States-Canada Alaska Rail Commission</td>
  </tr>
  <tr>
    <td>525</td>
    <td>00</td>
    <td>Election Assistance Commission</td>
  </tr>
  <tr>
    <td>526</td>
    <td>00</td>
    <td>Public Company Accounting Oversight Board</td>
  </tr>
  <tr>
    <td>527</td>
    <td>00</td>
    <td>Standard Setting Body</td>
  </tr>
  <tr>
    <td>528</td>
    <td>00</td>
    <td>Telecommunications Development Fund</td>
  </tr>
  <tr>
    <td>530</td>
    <td>00</td>
    <td>Affordable Housing Program</td>
  </tr>
  <tr>
    <td>531</td>
    <td>00</td>
    <td>Electric Reliability Organization</td>
  </tr>
  <tr>
    <td>534</td>
    <td>00</td>
    <td>Office of the Federal Coordinator for Alaska Natural Gas Transportation Projects</td>
  </tr>
  <tr>
    <td>535</td>
    <td>00</td>
    <td>Privacy and Civil Liberties Oversight Board</td>
  </tr>
  <tr>
    <td>537</td>
    <td>00</td>
    <td>Federal Housing Finance Agency</td>
  </tr>
  <tr>
    <td>538</td>
    <td>00</td>
    <td>National Infrastructure Bank</td>
  </tr>
  <tr>
    <td>539</td>
    <td>00</td>
    <td>Recovery Act Accountability and Transparency Board</td>
  </tr>
  <tr>
    <td>542</td>
    <td>00</td>
    <td>Council of the Inspectors General on Integrity and Efficiency</td>
  </tr>
  <tr>
    <td>573</td>
    <td>00</td>
    <td>Northern Border Regional Commission</td>
  </tr>
  <tr>
    <td>575</td>
    <td>00</td>
    <td>National Railroad Passenger Corporation Office of Inspector General</td>
  </tr>
  <tr>
    <td>576</td>
    <td>00</td>
    <td>Securities Investor Protection Corporation</td>
  </tr>
  <tr>
    <td>579</td>
    <td>00</td>
    <td>Patient-Centered Outcomes Research Trust Fund</td>
  </tr>
  <tr>
    <td>580</td>
    <td>00</td>
    <td>Corporation for Travel Promotion</td>
  </tr>
  <tr>
    <td>581</td>
    <td>00</td>
    <td>Bureau of Consumer Financial Protection</td>
  </tr>
  <tr>
    <td>582</td>
    <td>00</td>
    <td>Civilian Property Realignment Board</td>
  </tr>
  <tr>
    <td>584</td>
    <td>00</td>
    <td>Indian Law and Order Commission</td>
  </tr>
  <tr>
    <td>586</td>
    <td>00</td>
    <td>Gulf Coast Ecosystem Restoration Council</td>
  </tr>
  <tr>
    <td>587</td>
    <td>00</td>
    <td>Public Defender Service for the District of Columbia</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>900</td>
    <td></td>
    <td>Allowances</td>
  </tr>
  <tr>
    <td>900</td>
    <td>05</td>
    <td>Allowances </td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>902</td>
    <td>00</td>
    <td>Undistributed Offsetting Receipts
</td>
  </tr>
  <tr>
    <td>930</td>
    <td>00</td>
    <td>Miscellaneous Receipts Below the Reporting Threshold</td>
  </tr>
  </tbody>
</table>


<table>
  <caption>Table 2.  Listing of Functions and Subfunctions</caption>
  <thead>
	<tr>
	  <th>Function and Subfunction Code</th>
	  <th>Function and Subfunction Title</th>
	</tr>
  </thead>
  <tbody>
  <tr>
    <td>050</td>
    <td>National Defense</td>
  </tr>
  <tr>
    <td>051</td>
    <td>Department of Defense-Military</td>
  </tr>
  <tr>
    <td>053</td>
    <td>Atomic energy defense activities</td>
  </tr>
  <tr>
    <td>054</td>
    <td>Defense-related activities</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>150</td>
    <td>International Affairs</td>
  </tr>
  <tr>
    <td>151</td>
    <td>International development and humanitarian assistance</td>
  </tr>
  <tr>
    <td>152</td>
    <td>International security assistance</td>
  </tr>
  <tr>
    <td>153</td>
    <td>Conduct of foreign affairs</td>
  </tr>
  <tr>
    <td>154</td>
    <td>Foreign information and exchange activities</td>
  </tr>
  <tr>
    <td>155</td>
    <td>International financial programs</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>250</td>
    <td>General Science, Space, and Technology</td>
  </tr>
  <tr>
    <td>251</td>
    <td>General science and basic research</td>
  </tr>
  <tr>
    <td>252</td>
    <td>Space flight, research, and supporting activities</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>270</td>
    <td>Energy</td>
  </tr>
  <tr>
    <td>271</td>
    <td>Energy supply</td>
  </tr>
  <tr>
    <td>272</td>
    <td>Energy conservation</td>
  </tr>
  <tr>
    <td>274</td>
    <td>Emergency energy preparedness</td>
  </tr>
  <tr>
    <td>276</td>
    <td>Energy information, policy, and regulation</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>300</td>
    <td>Natural Resources and Environment</td>
  </tr>
  <tr>
    <td>301</td>
    <td>Water resources</td>
  </tr>
  <tr>
    <td>302</td>
    <td>Conservation and land management</td>
  </tr>
  <tr>
    <td>303</td>
    <td>Recreational resources</td>
  </tr>
  <tr>
    <td>304</td>
    <td>Pollution control and abatement</td>
  </tr>
  <tr>
    <td>306</td>
    <td>Other natural resources</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>350</td>
    <td>Agriculture</td>
  </tr>
  <tr>
    <td>351</td>
    <td>Farm income stabilization</td>
  </tr>
  <tr>
    <td>352</td>
    <td>Agricultural research and services</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>370</td>
    <td>Commerce and Housing Credit</td>
  </tr>
  <tr>
    <td>371</td>
    <td>Mortgage credit</td>
  </tr>
  <tr>
    <td>372</td>
    <td>Postal service</td>
  </tr>
  <tr>
    <td>373</td>
    <td>Deposit insurance</td>
  </tr>
  <tr>
    <td>376</td>
    <td>Other advancement of commerce</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>400</td>
    <td>Transportation</td>
  </tr>
  <tr>
    <td>401</td>
    <td>Ground transportation</td>
  </tr>
  <tr>
    <td>402</td>
    <td>Air transportation</td>
  </tr>
  <tr>
    <td>403</td>
    <td>Water transportation</td>
  </tr>
  <tr>
    <td>400</td>
    <td>Transportation – continued</td>
  </tr>
  <tr>
    <td>407</td>
    <td>Other transportation</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>450</td>
    <td>Community and Regional Development</td>
  </tr>
  <tr>
    <td>451</td>
    <td>Community development</td>
  </tr>
  <tr>
    <td>452</td>
    <td>Area and regional development</td>
  </tr>
  <tr>
    <td>453</td>
    <td>Disaster relief and insurance</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>500</td>
    <td>Education, Training, Employment, and Social Services</td>
  </tr>
  <tr>
    <td>501</td>
    <td>Elementary, secondary, and vocational education</td>
  </tr>
  <tr>
    <td>502</td>
    <td>Higher education</td>
  </tr>
  <tr>
    <td>503</td>
    <td>Research and general education aids</td>
  </tr>
  <tr>
    <td>504</td>
    <td>Training and employment</td>
  </tr>
  <tr>
    <td>505</td>
    <td>Other labor services</td>
  </tr>
  <tr>
    <td>506</td>
    <td>Social services</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>550</td>
    <td>Health</td>
  </tr>
  <tr>
    <td>551</td>
    <td>Health care services</td>
  </tr>
  <tr>
    <td>552</td>
    <td>Health research and training</td>
  </tr>
  <tr>
    <td>554</td>
    <td>Consumer and occupational health and safety</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>570</td>
    <td>Medicare</td>
  </tr>
  <tr>
    <td>571</td>
    <td>Medicare</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>600</td>
    <td>Income Security</td>
  </tr>
  <tr>
    <td>601</td>
    <td>General retirement and disability insurance (excluding social security)</td>
  </tr>
  <tr>
    <td>602</td>
    <td>Federal employee retirement and disability</td>
  </tr>
  <tr>
    <td>603</td>
    <td>Unemployment compensation</td>
  </tr>
  <tr>
    <td>604</td>
    <td>Housing assistance</td>
  </tr>
  <tr>
    <td>605</td>
    <td>Food and nutrition assistance</td>
  </tr>
  <tr>
    <td>609</td>
    <td>Other income security</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>650</td>
    <td>Social Security</td>
  </tr>
  <tr>
    <td>651</td>
    <td>Social security</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>700</td>
    <td>Veterans Benefits and Services</td>
  </tr>
  <tr>
    <td>701</td>
    <td>Income security for veterans</td>
  </tr>
  <tr>
    <td>702</td>
    <td>Veterans education, training, and rehabilitation</td>
  </tr>
  <tr>
    <td>703</td>
    <td>Hospital and medical care for veterans</td>
  </tr>
  <tr>
    <td>704</td>
    <td>Veterans housing</td>
  </tr>
  <tr>
    <td>705</td>
    <td>Other veterans benefits and services</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>750</td>
    <td>Administration of Justice</td>
  </tr>
  <tr>
    <td>751</td>
    <td>Federal law enforcement activities</td>
  </tr>
  <tr>
    <td>750</td>
    <td>Administration of Justice – continued</td>
  </tr>
  <tr>
    <td>752</td>
    <td>Federal litigative and judicial activities</td>
  </tr>
  <tr>
    <td>753</td>
    <td>Federal correctional activities</td>
  </tr>
  <tr>
    <td>754</td>
    <td>Criminal justice assistance</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>800</td>
    <td>General Government</td>
  </tr>
  <tr>
    <td>801</td>
    <td>Legislative functions</td>
  </tr>
  <tr>
    <td>802</td>
    <td>Executive direction and management</td>
  </tr>
  <tr>
    <td>803</td>
    <td>Central fiscal operations</td>
  </tr>
  <tr>
    <td>804</td>
    <td>General property and records management</td>
  </tr>
  <tr>
    <td>805</td>
    <td>Central personnel management</td>
  </tr>
  <tr>
    <td>806</td>
    <td>General purpose fiscal assistance</td>
  </tr>
  <tr>
    <td>808</td>
    <td>Other general government</td>
  </tr>
  <tr>
    <td>809</td>
    <td>Deductions for offsetting receipts</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>900</td>
    <td>Net Interest</td>
  </tr>
  <tr>
    <td>901</td>
    <td>Interest on Treasury debt securities (gross)</td>
  </tr>
  <tr>
    <td>902</td>
    <td>Interest received by on-budget trust funds</td>
  </tr>
  <tr>
    <td>903</td>
    <td>Interest received by off-budget trust funds</td>
  </tr>
  <tr>
    <td>908</td>
    <td>Other interest</td>
  </tr>
  <tr>
    <td>909</td>
    <td>Other investment income</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>920</td>
    <td>Allowances</td>
  </tr>
  <tr>
    <td>923</td>
    <td>Immigration Reform</td>
  </tr>
  <tr>
    <td>924</td>
    <td>Adjustment for Budget Control Act Caps (Non-Security)</td>
  </tr>
  <tr>
    <td>925</td>
    <td>Future Disaster Costs</td>
  </tr>
  <tr>
    <td>928</td>
    <td>Adjustment to Benefit Payment Timing</td>
  </tr>
  <tr>
    <td>929</td>
    <td>Placeholder for Outyear OCO Costs</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>950</td>
    <td>Undistributed Offsetting Receipts</td>
  </tr>
  <tr>
    <td>951</td>
    <td>Employer share, employee retirement (on-budget)</td>
  </tr>
  <tr>
    <td>952</td>
    <td>Employer share, employee retirement (off-budget)</td>
  </tr>
  <tr>
    <td>953</td>
    <td>Rents and royalties on the Outer Continental Shelf</td>
  </tr>
  <tr>
    <td>954</td>
    <td>Sale of major assets</td>
  </tr>
  <tr>
    <td>959</td>
    <td>Other undistributed offsetting receipts</td>
  </tr>
  </tbody>
</table>


<table>
  <caption>Table 3.  Source Categories for Receipts</caption>
  <thead>
	<tr>
	  <td>Source Category Code</td>
	  <td>Source Subcategory Code</td>
	  <td>Category and Subcategory Title</td>
	</tr>
  </thead>
  <tbody>
  <tr>
    <td>931</td>
    <td></td>
    <td>Individual Income Taxes</td>
  </tr>
  <tr>
    <td></td>
    <td>00</td>
    <td>Individual Income Taxes</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>932</td>
    <td></td>
    <td>Corporation Income Taxes</td>
  </tr>
  <tr>
    <td></td>
    <td>00</td>
    <td>Corporation Income Taxes</td>
  </tr>
  <tr>
    <td></td>
    <td>05</td>
    <td>Corporation Income Taxes</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>933</td>
    <td></td>
    <td>Social Insurance Taxes and Contributions</td>
  </tr>
  <tr>
    <td></td>
    <td>05</td>
    <td>Employment Taxes and Contributions</td>
  </tr>
  <tr>
    <td></td>
    <td>10</td>
    <td>Unemployment Insurance</td>
  </tr>
  <tr>
    <td></td>
    <td>15</td>
    <td>Other Retirement Contributions</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>934</td>
    <td></td>
    <td>Excise Taxes</td>
  </tr>
  <tr>
    <td></td>
    <td>00</td>
    <td>Excise Taxes</td>
  </tr>
  <tr>
    <td></td>
    <td>05</td>
    <td>Federal Fund Excise Taxes</td>
  </tr>
  <tr>
    <td></td>
    <td>10</td>
    <td>Trust Fund Excise Taxes</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>935</td>
    <td></td>
    <td>Estate and Gift Taxes</td>
  </tr>
  <tr>
    <td></td>
    <td>00</td>
    <td>Estate and Gift Taxes</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>936</td>
    <td></td>
    <td>Customs Duties</td>
  </tr>
  <tr>
    <td></td>
    <td>00</td>
    <td>Custom Duties and Fees</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>937</td>
    <td></td>
    <td>Misc. Governmental Receipts</td>
  </tr>
  <tr>
    <td></td>
    <td>00</td>
    <td>Misc. Governmental Receipts</td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>938</td>
    <td></td>
    <td>Legislative Proposals</td>
  </tr>
  <tr>
    <td></td>
    <td>00</td>
    <td>Legislative Proposals</td>
  </tr>
  </tbody>
</table>

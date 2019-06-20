---
layout: info-page
title: Vision
permalink: /vision
---

RPEDS seeks to create efficiencies for higher education researchers who using publically-available “open” data. RPEDS products will be consistent, authoritative, centrally stored and accessible at no/minimal cost to partners researchers.

RPEDS seeks to discuss, develop, host, and maintain 1) **a master institutional/entity lookup table** containing additional metadata to reflect local preferences, and 2) **a database containing institution/entity level** **data** that has been cleaned, compiled, and verified across multiple years to ease analysis and visualization.

Initial **“open data”** includes postsecondary education data and population demographic, beginning with the U.S. Department of Education (IPEDS, CDR, PEPS), Veterans Administration and the U.S. Census Bureau.

Initial **“local”** data may include custom-collected tuition and fee data for institutions and key measures for institutions reporting through a non-Washington parent, including Northeastern University-Seattle, University of Phoenix, and Western Governors University.

While initially formed in Washington, RPEDS will include all available states and geographies, especially when integrating federal data sources, to allow both for comparison/benchmarking and the potential to open database access and expand collaboration to researchers in other states.

## We envision that RPEDS [at this point in time] will:

 - **Bring stakeholders together to establish modified crosswalks of Institutional Characteristics and groupings.** Categorical variables are the foundation of our aggregated statistics, but we are not aware of any formal efforts (recently) to establish and host a shared crosswalk that codifies the generally accepted modification at the local level. Examples include recategorizing “4-year” colleges that primarily confer associates and certificates as “two-year participation in state aid programs, and variables for control, and sector association membership.
  - **Address processing, storing, and retrieving “corrected” IPEDS data**. Consistent and centrally stored IPEDS data is
   undoubtedly mundane, but the current process is incredibly inefficient for researchers and developers.
-  **Be simply, cheaply, and rapidly developed**. The faster we can save folks the drudgery of manually wrangling IPEDS, the better; can be done with at low cost without much custom development.
- **Be sustainable and expandable**. While a counterpoint to cheap and fast, it is important to be thoughtful about how/when datasets will be refreshed, how customizable output files will be, whether other    public datasets might be included, and if there are other pain-points to consider.
 - **Bring together open and like-minded partners to work together**. This point is at the bottom of the list since collaboration is the absolute foundation and motivation for this project. It started with two groups and is open to all who share our vision.

## Options and approaches to solving main issues:

- Defining and agreeing on the “corrected“ fields will be a critical discussion that involves main stakeholders. It also is a great example of why there is often variation in (esp sector-level) analyses from different groups using the exact same dataset.
- Cleaning/compilation could be (semi)automated through business rules and scripts, as IPEDS and other federal data files are mostly consistent -- but just not enough to be easy to work with.
- Multiple options for storage/retrieval to balance complexity, cost, and flexibility:

	 - **Flat file repositories** such as Socrata’s  [opendatanetwork.com](http://www.opendatanetwork.com) and [data.wa.gov](http://data.wa.gov), [data.world](http://data.world) or Kaggle
	 - **Cloud-hosted relational databases** with custom development    including Enterprise solutions, including MS SQL
   Server (used by    WSAC) or Oracle, or less expensive solutions such
   as MySQL or    PostgreSQL.
	 - **Unstructured data____** (base, lake, etc)  – perhaps overkill for    pilot as storing entity level aggregated data.

## Why IPEDS?

Among higher education data sources, the federal Integrated Postsecondary Education Data System (IPEDS) is perhaps the most commonly used source for calculating statistics at the institution-, sector-, state-, and national-levels. IPEDS is frequently used by institutional staff, policy makers, reporters, and researchers, and has been utilized as a primary data source or cited in countless articles, reports, and studies: over 4,000 references in academic article published since 2014 and typically a dozen or more references each month in the general media.

## Strengths of IPEDS: 
-	Breadth and depth of topics and measures are far greater than other federal sources, such as PEPS, DAPIP, or VA
-	Inclusion of approximately 7,500 institutions, including all those participating in federal Title IV programs
-	Relatively consistent use of data definitions over multiple year periods. 
-	Data is downloadable through the in multiple file formats including CSV, ACCESS, SAS, and STATA.
-	Generally-defined data release schedule.

## Weaknesses of IPEDS data: 
IPEDS users in Washington state have identified the data compilation, transformation and cleaning stages as one of the most time consuming and prone to analytical inconsistencies, in particular, the following main areas addressed in this vision document:
-	Universe of reporting institutions is far smaller than the other federal sources noted above (7,500 institutions vs 45,000+)
-	Reconciling entities and ID codes can be extremely difficult for both federal[^1] and state[^2] administrative data
-	Preparing and using data for time series are time-consuming and can be difficult. Some issues noted include year specific field name that change order from the query tool, and MS Access and CSV’s do not contain year fields.
-	Definition changes between years may lead to analysis issues[^3].
- In some states, specific IPEDS categories, such as level and sector, often do not align with state-recognized groupings[^4]. These adjusted categories are often not documented by local users and thus inconsistently applied. and while users can use alternative categories such as Institutional Category[^5] , some IPEDS surveys differ depending on the assigned sector, including widely used elements such as graduation and retention rate, admissions, and cost of attendance. 
## Opportunities to Enhance IPEDS
-	New custom categories including participation in state aid programs, award levels, association memberships.
-	Add supplemental tables containing “missing” and child institution data for select measures.
-	Updated institution openings and closures occurring between IPEDS releases using related data.
## Threats 
-	Data cleaning and validation could introduce errors
-	Ongoing maintenance will require capital and oversight
-	Usage may not justify investment
-	NCES may launch new IPEDS portal in 2-5 years
## Potential partners that might be able to help or provide input:
(contacted, interested, committed)  
#### State and Regional Partners, Contacts, Users
-	Education Researchers: CEDR, CSF, ERDC, WSAC, WSIPP, WTB, others...
-	Institutional staff and researchers at institutions
  - ○	UW (project co-leads)
-	IPEDS State Coordinator (Darby Kaikkonen, SBCTC)
-	Professional Groups: PNAIRP and WERA  
- Stakeholder Associations: COP, ICW, NWCCF
-	Students in ed policy, iSchool, informatics, etc. 
#### National/ Regional Partners, Contacts, or Users
-	Associations: AASCU, APLU, SHEEO, WICHE, etc
-	Professional Groups: AIR
-	Administrators: IPEDS/NCES and RTI
-	Research orgs and foundations: BMGF, Lumina, Ballmer, New America, Urban Institute 
#### External funding (financial or in-kind)
-	Socrata’s OpenDataNetwork could be a nearly Out-of-the-Box solution, and they potentially could help build the connectors and scripts at low cost. The Publica platform could also host data with more governance 
-	Other corporations/institutional resources. Could include executive service corps, donation of platform, tools, server space, monetary support etc. 
## Future Opportunities
The evolution of RPEDS is a group conversation and exploration, but some ideas discussed have included:
-	Scaling to include local preferences for “Institutional Characteristics” for other states.
-	Build out of robust front end for non-specialist use, which may include custom queries and visualization.
-	Expansion to other education-focused datasets including PK12, Postsecondary, and Workforce data sources, such Department of Education’s Student Loan and Campus Based Aid data sets, US Department of Veterans Affairs, and licensing Peterson’s Common Data Set. 
-	Expansion to non-education focussed datasets, including US Census and the American Community Survey, Bureau of Labor and Statistics, and other open sources. 
 
## Appendix A: New and Revised Variables or Records to Consider
Note: this list is under development and actively being added to. 
#### Revised Variables
-	Level: focus on colleges offering baccalaureate degrees but primarily conferring associate and below awards, revising using IPEDS Institutional Category (INSTCAT) variable. 	
-	Control: Redesignation to address institutions changing their IRS designation, mostly for profit to nonprofit status 
-	Sector: combines revised level and revised control
-	Active/Closed Status: to address recent closures or teach outs between IPEDS releases 
-	Alternate State: to account for institutions that have historic precedence in Washington
#### New Variables	
-	Name Abbreviation: CWU, EWU, TESC, UW-B, UW-S, UW-T, WSU, WWU
-	Superlevel and supersector: coalescing revised level and sector “four year and higher” and “two year and less” x three control categories.
-	Subsector: considering state preferred nomenclature and assignment for Research vs. Comprehensive/Regional universities, CTC’s offering  baccalaureate degrees, etc. 
-	State Sector Association Membership
-	National Association Memberships: could be crosstabbed for ACE, AASCU, APLU, NAICU, AAU, AACC, and Other?
-	State Grant Participation: could be crosstabbed for participation years
#### New Records and Numeric Data
-	Including alternate, branch and shared campus locations for GIS purposes
-	Key measures for online institutions that have large presence in Washington but IPEDS reports as single institution in another state: might include enrollment and completion measures for Northeastern, University of Phoenix and Western Governors University


---

[^1]: NCES TRP 42 for discussion of IPEDS Unit ID, OPEID and VA facility codes. DAPIP matching is doubly difficult. 
[^2]: Washington’s Workforce and Training Coordinating Board Career Bridge
[^3]: NPEC’s History and Origins of Survey Items for IPEDS gives critical background
[^4]: Primary corrections will align to generally accepted local (WA) preferences: Washington CTC’s offering bachelor’s degrees recategorized back to 2-year institutions; Northwest Indian College as a separate category; deciding on rules for institutional control changes (e.g. former for-profits rechartered as nonprofit). See Appendix A for more examples. 
[^5]: This issue has been identified and discussed by NCES Technical Review Panel 48 
<div class="footnotes">

</div>


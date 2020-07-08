# Site Architecture:
- ReadMe
- Summary
- Video Presentatin
- Final Notbook
- Link to predictions story
- Descriptive Vizualizations Story
- Recommendations Story
- Cluster Story




# Project Title 

Using publicly available data from the US Department of Housing and Urban Development (HUD), we attempt to predict surges in multifamily housing markets before they happen.  

# Tools




# Planning

Crucial to any successful project is the planning phase, specifically: defining the MVP, or Minimal Viable Product
Decision was made to use the Top25 loan amounts
Back to the MVP - the first pass that if Clifton came over he needed to see something 'now'
    - a recommendation based on the model and the actual model we build that asserts those recommendations
Per capita was not used int he MVP but in feature engineering
When segmenting the data, wanted to be as simple as possible

Held a strengths vs weaknesses meeting to help guide our efforts in the 
A market gets hot, investors come in and buy all they can, making the property hotter.  Eventually a threshold is reached where
they decide its best to build new
rather than buy existing property - refinance - they take their money and build new
MVP is to find the moment where everything gets hot.  When does the buying market get hot.  Then take it to see if there's a secondary spike in the future where the building market gets hot.  Classification model will highlight what we consider a trend, and decide if what we find is viable
Initial expoloration on Houston, Dallas, and Seattle - maybe we can find what's driving those markets, then test our findings against the Top 25 

Target variable new construction in dollars - the class of the market  - the classification is the end target

## Time Series Regression Hypothesis

$H_0$ - Mortgage Lending and market development are independent from each other
$H_a$ - Mortgage Lending and market development are dependent on each other

## Classification (ANOVA)

The mean final mortgage amount among all markets is indistinguishable
The mean final mortgage amount among all markets is different

A single observation would be the total final mortgage amount for a city (market) and year of that mortgage

## Data Dictionary

**Block Grant** - A block of money from the federal government given to state and local governments for use in social welfare programs like law enforcement, community development, and health services.  Unlike categorical grants, block grants are not earmarked for anything specific, so local governments can spend them as they see fit.  

**FHA** - 'Federal Housing Administration' - With regards to this project, we are talking about monetary loans that come from the Federal Housing Administration, also known as 'FHA Loans.'  These are federally-backed loans from approved money lenders made to people designated as low-to-moderate income, although there is no max or minimun income level listed for qualification.  They do, however, tend to be geared toward people with lower credit scores (as low as 500) to help get them into home ownership.

**HFA Risk Sharing** - 'Housing Finance Agency' - the regulatory body of the US Department of Housing and Urban Development (HUD), they took over financial affairs and daily operations of both Fannie Mae and Freddie Mac, who were selling mortgage-backed securities.  'HFA Risk Sharing' means that the HFA is sharing the risk of the loan with the FHA; if the loan defaults, both agencies split the loss.  Seeing this in our data means the multi-unit property / building has been purchased and the commitment is firm.

**Firm Commitment** - also known as 'firm commitment underwriting,' a firm commitment is a lender's promise to enter a loan agreement with a borrower.  As it pertains to this investigation, since the construction of new multifamily units is both expensive and intensive, we consider the value of 'Firm Issued' to mean that the money was allocated as promised and that the construction of new units took place.

**MAP** - 'Multifamily Accelerated Processing' - decentralized command from HUD, MAP allows underwriters (the people looking at your credit history) at qualified lenders to prepare FHA forms and conduct the preliminary underwriting for certain applications.  Not only does this speed up the process, but it reduces the risk HUD faces when allocating funds; MAP approved underwriters are their boots on the ground.

**TAP** - 'Traditional Application Processing' - In order for a lender to be part of the 'MAP' process, all of its underwriters must complete specialized HUD training where they learn all the parameters of HUD financing.  Without this training, applications must be processed by a HUD field staff member, which takes more time because only HUD-approved underwriters can decide whether or not a loan should be financed.

**LIHTC Designation** - 'Low Income Housing Tax Credit' - aimed at private equity, this is a federal tax credit to incentivize new construction of multi- and single-family homes for low-income individuals.  There are several parameters which must be met (e.g: building residents can't have a net income of over 50% of surrounding area net incomes), and the total allocation amount is based on the state's population size, at about $2.70 per person.

**'Tax Exempt Bond' Designation** - cities sell bonds to raise money for public improvements.  A tax-exempt bond (or, 'municipal bond')is desirable to investors because the interests they earn on their investment (the bond) is tax free.

**'HOME' Designation** - 'Home Investment Partnership Program' - a federal assistance program provided by HUD to provide decent and affordable housing, paticularly to low- and very-low-income Americans.  It is the single biggest block grant providing approximately $2B (2020 estimates) to states and municipalities looking to increase the amount of affordable housing within the US.

**'CDBG' Designation** - 'Community Development Block Grant' - a federal grant meant to develop viable urban communities by providing decent housing and expanding economic opportunities for people of low- to moderate-incomes.  Not only meant for housing and economic development, but for disaster recovery as well.

**'Section 202 Refi' Designation** - a federal program encouraging non-profit entitites to build housing with supportive services for severely low-income senior citizens.  The buildings must be specifically designed to service the needs of the elderly and either all residents must be over the age of 62 or have 80% of its occupants over the age of 55.

**'IRP Decoupling' Designation** - 'Interest Reduction Payments Decoupling' - some borrowers qualify for a government subsidy (financial assistance) that helps reduce their monthly interest payments.  This subsidy is paid directly to the lender to help cover the interest rate of the loan.  All well and good, but if the owner refinances, all the leftover interest the lender is expecting to make is lost.  An IRP Decopuling allows that remaining interest to move into the refinanced loan amount, so the lender can still plan on receiving the original interest payments despite the refinancing.  Wherever you see this designation, a refinance is likely to have taken place, though its specifics are not available 

**'HOME VI' Designation** - Title VI is funding for federally recognized tribes and Tribally Designated Housing Entities meant for refinancing and new home construction, as well as all the costs associated with community development.


## Summary Background on Stakeholder, TestFit.io

Based in Dallas, TX and originally named 'BuildingForge,' TestFit.io was founded by Clifton Harness (CEO) and Ryan Griege(CTO) in October of 2015.  They are a software company specifically meant to help architects craft buildings more quickly through their generative design tools that translate over to AutoCAD, a poplular tool used in all phases of the construction process.  Their enhanced visualizations help architects test parametric designs while streamlining the feasibility study process for commercial projects, both substantial roadblocks in any community investment project.

In January 2020, TestFit.io received $2,000,000 from Parkway Venture Capital, which they have earmarked for both personnel and market growth.  They are currently looking to expand their offerings into retail floorplan analysis ('adjacency studies') and hospital construction.  

## Functions Used In Acquiring, Preparing, Exploring, and Modeling the Data

**Acquiring (Wrangling)**

**Preparing**

**Exploring**

**Modeling**# hud-capstone.github.io

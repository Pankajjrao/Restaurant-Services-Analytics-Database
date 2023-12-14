Def :- Online Analytical Processing

What is OLAP?
	It is a system for performing multi-dimensional analysis at high speed on large volumes of data.
	Large volumes of data can come from data warehouses or data mart etc.
	OLAP is ideal for tasks such as data mining, business intelligence and complex analytical calculations.
	OLAP is optimized for conducting complex data analysis and OLAP systems are designed to be used by data scientists and business analysts etc.

Multi-dimensional:-
	Multi dimensional data here means the multiple ways  data can be categorized and viewed .
	for example :-
	Time can be viewed as days, months, hours, years .
	Sales can be viewed in terms of diff products such as cars, bikes etc.
	and these can further viewed as sale of car per year or sale of bikes quarter etc.
	SO,
	multiple combinations of these dimensions (TIME AND PRODUCTS) can create multiple dimensions and having multiple dimensions creates a need for Multi-dimensional analysis.

OLAP CUBE :-
	![[Pasted image 20231214140700.png]]
	OLAP cube is a way to organize and analyze your data in multiple dimensions making it easy to explore and understand various information from different perspectives.

SCHEMAS in OLAP systems:-
	Fact table = 
		fact table is a central table that typically contains numerical values or performance metrics, and it often represents events or transactions.
		Fact tables store the quantitative data that you want to analyze, such as measures of business activities. Common examples of measures found in fact tables include:
		Sales, Revenue, Quantity, Profit, Count of Events.
		> Fact table contains more rows and less columns.
		> Fact table contains Foreign keys	
	Dimension Table :-
		 Also known as Lookup tables. these tables contains descriptive attributes or columns that can be used for filtering, aggregating and grouping the data.
		 >Dimension tables contains less rows and more attributes or columns
		 >Fact table contains Primary keys	 which becomes foreign key in Fact table
		

1. STAR SCHEMA :- 
			Star schema contains a single fact table surrounded by one or more dimension tables. It is a simple and easy to understand schema as compared to snowflake schema.
			![[Pasted image 20231214141827.png]]
		
 2. SNOWFLAKE SCHEMA:-
			 Snowflake schema is similar to star schema but it normalizes the dimension tables by breaking them into sub dimensions, which helps in saving storage but slows the query performance.
			 ![[Pasted image 20231214142215.png]]
			


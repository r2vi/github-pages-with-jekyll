# Your GitHub Learning Lab Repository for GitHub Pages

Welcome to **your** repository for your GitHub Learning Lab course. This repository will be used during the different activities that I will be guiding you through. 

Oh! I haven't introduced myself...

I'm the GitHub Learning Lab bot and I'm here to help guide you in your journey to learn and master the various topics covered in this course. I will be using Issue and Pull Request comments to communicate with you. In fact, I already added an issue for you to check out.

![issue tab](https://lab.github.com/public/images/issue_tab.png)

I'll meet you over there, can't wait to get started!

`This repository is licensed under [MIT](../LICENSE) (c) 2019 GitHub, Inc.`

```DAX
DAX
Avg Income by State and Avg. Last 6 month purchases by state correlation for Avg. Last 6 month purchases by state = 
VAR __CORRELATION_TABLE = VALUES('Regression Table'[Y])
VAR __COUNT =
	COUNTX(
		KEEPFILTERS(__CORRELATION_TABLE),
		CALCULATE(
			SUM('Regression Table'[X])
				* SUM('Regression Table'[Y])
		)
	)
VAR __SUM_X =
	SUMX(
		KEEPFILTERS(__CORRELATION_TABLE),
		CALCULATE(SUM('Regression Table'[X]))
	)
VAR __SUM_Y =
	SUMX(
		KEEPFILTERS(__CORRELATION_TABLE),
		CALCULATE(SUM('Regression Table'[Y]))
	)
VAR __SUM_XY =
	SUMX(
		KEEPFILTERS(__CORRELATION_TABLE),
		CALCULATE(
			SUM('Regression Table'[X]) * SUM('Regression Table'[Y])
				* 1.
		)
	)
VAR __SUM_X2 =
	SUMX(
		KEEPFILTERS(__CORRELATION_TABLE),
		CALCULATE(SUM('Regression Table'[X]) ^ 2)
	)
VAR __SUM_Y2 =
	SUMX(
		KEEPFILTERS(__CORRELATION_TABLE),
		CALCULATE(
			SUM('Regression Table'[Y])
				^ 2
		)
	)
RETURN
	DIVIDE(
		__COUNT * __SUM_XY - __SUM_X * __SUM_Y * 1.,
		SQRT(
			(__COUNT * __SUM_X2 - __SUM_X ^ 2)
				* (__COUNT * __SUM_Y2 - __SUM_Y ^ 2)
		)
	)^2
  ```
  Dax
  ```SSAS
  DAX
  ALL( [<table> | <column>[, <column>[, <column>[,…]]]] )
  ```

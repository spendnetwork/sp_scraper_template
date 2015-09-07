
###Notes on the Spend Network morph scrapers for spend files. (sp_)


Where possible, try to stick to the template, editing only the 'VARIABLES' and 'SCRAPE DATA' sections.
This is to keep future editing easier and possible with Search/Replace function.
Especially as we move in to 100s of scrapers.


```
#### IMPORTS 1.0
#### FUNCTIONS 1.0
#### VARIABLES 1.0
#### READ HTML 1.0
#### SCRAPE DATA
#### STORE DATA 1.0
#### EOF
```


---

The goal of the SCRAPE DATA section is to create the 'data' list in this format.

```
[[csvYr, csvMth, url],
[csvYr, csvMth, url],
[csvYr, csvMth, url]]
```

Any extra module imports or code needed to achieve this should stay in this section.

---

For quaterly files, try to save the quarter in the 'csvMth' variable with this relationship:

```
Q1 = Jan-Mar
Q2 = Apr-Jun
Q3 = Jul-Sep
Q4 = Oct-Dec
```

If the source uses different months or they can not be identified, store as Q0.

```
Q0 = Any other quaterly file
```

# San Nicolas de los Garza - COVID Cases vs. Complaints per Affected Legal Good

This repository is done with the purpose of completing a project task for a course. The main focus was to find an analysis problem to be plotted based on a city we're familiar with. For which, I chose San Nicolas de los Garza, Nuevo Leon, Mexico.
The problem is to find a correlation between increase of COVID cases and a crime measurement in the city during a certain period of time so we can draw conclusions from that.

## Official Assignment Information

Before working on this assignment please read these instructions fully. In the submission area, you will notice that you can click the link to **Preview the Grading** for each step of the assignment. This is the criteria that will be used for peer grading. Please familiarize yourself with the criteria before beginning the assignment.

This assignment requires that you to find **at least** two datasets on the web which are related, and that you visualize these datasets to answer a question with the broad topic of **weather phenomena** (see below) for the region of **San Nicolás de los Garza, Nuevo León, Mexico**, or **Mexico** more broadly.

You can merge these datasets with data from different regions if you like! For instance, you might want to compare **San Nicolás de los Garza, Nuevo León, Mexico** to Ann Arbor, USA. In that case at least one source file must be about **San Nicolás de los Garza, Nuevo León, Mexico**.

You are welcome to choose datasets at your discretion, but keep in mind **they will be shared with your peers**, so choose appropriate datasets. Sensitive, confidential, illicit, and proprietary materials are not good choices for datasets for this assignment. You are welcome to upload datasets of your own as well, and link to them using a third party repository such as github, bitbucket, pastebin, etc. Please be aware of the Coursera terms of service with respect to intellectual property.

Also, you are welcome to preserve data in its original language, but for the purposes of grading you should provide english translations. You are welcome to provide multiple visuals in different languages if you would like!

As this assignment is for the whole course, you must incorporate principles discussed in the first week, such as having as high data-ink ratio (Tufte) and aligning with Cairo’s principles of truth, beauty, function, and insight.

Here are the assignment instructions:

 * State the region and the domain category that your data sets are about (e.g., **San Nicolás de los Garza, Nuevo León, Mexico** and **weather phenomena**).
 * You must state a question about the domain category and region that you identified as being interesting.
 * You must provide at least two links to available datasets. These could be links to files such as CSV or Excel files, or links to websites which might have data in tabular form, such as Wikipedia pages.
 * You must upload an image which addresses the research question you stated. In addition to addressing the question, this visual should follow Cairo's principles of truthfulness, functionality, beauty, and insightfulness.
 * You must contribute a short (1-2 paragraph) written justification of how your visualization addresses your stated research question.

What do we mean by **weather phenomena**?  For this category you might want to consider seasonal changes, natural disasters, or historical trends.

### Tips
* Wikipedia is an excellent source of data, and I strongly encourage you to explore it for new data sources.
* Many governments run open data initiatives at the city, region, and country levels, and these are wonderful resources for localized data sources.
* Several international agencies, such as the [United Nations](http://data.un.org/), the [World Bank](http://data.worldbank.org/), the [Global Open Data Index](http://index.okfn.org/place/) are other great places to look for data.
* This assignment requires you to convert and clean datafiles. Check out the discussion forums for tips on how to do this from various sources, and share your successes with your fellow students!

### Example
Looking for an example? Here's what our course assistant put together for the **Ann Arbor, MI, USA** area using **sports and athletics** as the topic. [Example Solution File](./readonly/Assignment4_example.pdf)

## Previous configurations

In order to run this script, you will need:

- The necessary libraries installed
- Create .env file with the necessary environmental variables
- Obtain input files

### Installing the libraries

The script works with the following versions:
- python `3.11.5`
- pandas `2.1.0`
- numpy `1.25.2`
- matplotlib `3.7.2`
- python-dotenv `1.0.0`

To install the necessary libraries, run the following code in a Python executer
``` CMD Commands
pip install python-dotenv
```

To view the version of your libraries, run the following:
``` CMD Commands
pip show python-dotenv
```

Another alternate method to view all of the installed libraries if the following:
``` CMD Commands
pip show list
```

### Environmental variables

The `.env` file needs to have the following environmental variables for the script to work properly:

- `covid_reports`: File obtained from municity database with COVID-19 cases reported during a certain period of time.
- `city_complaints`: File obtained from municity database with affected legal goods reported during a certain period of time.
- `start_date`: Date where you wish for the period to be calculated from
- `end_date`: Date where you wish for the period to be calculated to

Your `.env` file should look like this:

``` textplain
covid_reports='Casos-positivos-diarios-en-San-Nicolas-de-los-Garza-Promedio-movil-de-7-dias.csv'
city_complaints='Denuncias-segun-bien-afectado-en-San-Nicolas-de-los-GarzaClic-en-el-grafico-para-seleccionar.csv'
start_date = '2020-02-01'
end_date = '2021-08-01'
```

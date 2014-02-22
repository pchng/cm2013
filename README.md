2013 Chicago Marathon Results
=============================

This consists of two parts: A python-based scraper to grab the results into CSV format, and an IPython Notebook used to analyze the results using the venerable [pandas](http://pandas.pydata.org/) data analysis library.

The scraper can also work with past years, not just 2013, but I have not tested it out.

The scraper was tested out on Python 2.7.x.

Using the scraper
-----------------
First, clone the repository and `cd` to the directory.

    pip install -r requirements.txt
    
Then you can run the scraper with the following command: (Will save it to file called `chicago_marathon_results.csv`)

    python chicago_marathon_results_scraper.py 2013 -n 1000 > chicago_marathon_results.csv

To view the output as well, you can use `tee` like so:

    python chicago_marathon_results_scraper.py 2013 -n 1000 | tee chicago_marathon_results.csv

For other usage, use the `--help` option:

    python chicago_marathon_results_scraper.py --help


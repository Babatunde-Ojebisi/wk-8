# COVID-19 Research Data Analysis

**Student:** Babatunde Ojebisi  
**Course:** Python Programming  
**Assignment:** COVID-19 Dataset Analysis  

## What This Project Does

This project analyzes COVID-19 research papers from the CORD-19 dataset. I wanted to understand:
- How many papers were published each year during the pandemic
- Which journals published the most COVID research
- What topics researchers were focusing on
- How the research landscape changed over time

## Files in This Project

- **`main.py`** - My main analysis script (this is the important one!)
- **`sample_metadata.csv`** - The dataset I'm analyzing (1,000 research papers)
- **`requirements.txt`** - Python packages needed (though my main script uses built-ins)
- **`my_analysis_results.json`** - Results file created when you run the analysis

## How to Run My Analysis

1. Make sure you have Python installed (I used Python 3.12)
2. Put all the files in the same folder
3. Open terminal/command prompt in that folder
4. Run: `python main.py`

That's it! The script will do everything and show you the results.

## What I Found (Key Results)

### Publication Trends
- **2020-2022** were the peak years for COVID research
- Research stayed pretty consistent across years (around 240-260 papers per year in my sample)
- The pandemic really drove a lot of scientific research!

### Top Journals
The biggest medical journals published most of the COVID research:
1. **The Lancet** - 109 papers (10.9%)
2. **Nature** - 106 papers (10.6%) 
3. **BMJ** - 105 papers (10.5%)
4. **PLOS ONE** - 105 papers (10.5%)
5. **Science** - 101 papers (10.1%)

### Research Focus
Most common topics in paper titles:
- **Clinical studies** (patients, treatment, clinical)
- **Vaccine research** (vaccine, immunization, antibody)
- **Public health** (health, disease, infection)
- **Medical treatments** (therapy, medical, treatment)

## Challenges I Faced

### Data Issues
- **Missing data:** Some papers didn't have complete information
- **Date formats:** Had to figure out how to parse dates properly
- **Text processing:** Cleaning up paper titles was trickier than expected
- **Large dataset:** The full CORD-19 dataset is huge, so I used a sample

### Technical Challenges
- **Package installation:** Had trouble installing some Python packages
- **Memory usage:** Processing lots of text data at once
- **Error handling:** Making sure the script doesn't crash on bad data

### Solutions I Found
- Used Python's built-in libraries instead of external packages
- Created a sample dataset that's easier to work with
- Added lots of error checking and data validation
- Made text-based visualizations instead of fancy graphs

## What I Learned

### Technical Skills
- How to read and process CSV files in Python
- Using dictionaries and lists to organize data
- Working with dates and text processing
- Creating simple data visualizations
- Handling missing and messy data

### Data Science Concepts
- **Data cleaning is really important** - most of my time was spent on this!
- **Real data is messy** - nothing is perfect in the real world
- **Visualization helps understanding** - even simple charts make patterns clear
- **Documentation matters** - commenting code helps a lot later

### Domain Knowledge
- COVID research exploded during the pandemic
- High-impact journals were the main outlets for COVID research
- Clinical and vaccine research were major focus areas
- International collaboration was important

## Code Structure

I organized my code into a class called `COVIDAnalyzer` with these methods:

- `load_csv_data()` - Loads the dataset from CSV file
- `explore_dataset()` - Shows basic info about the data
- `clean_my_data()` - Removes bad records and fixes issues
- `analyze_publications()` - Counts papers by year
- `analyze_journals()` - Finds top publishing journals
- `analyze_research_topics()` - Looks at common words in titles
- `create_summary_report()` - Saves results to JSON file

## If I Had More Time

Things I would add or improve:

### Analysis Improvements
- **Abstract analysis:** Look at paper abstracts, not just titles
- **Author networks:** See which researchers collaborate
- **Geographic analysis:** Compare research by country
- **Citation analysis:** Find the most influential papers

### Technical Improvements
- **Better visualizations:** Use matplotlib or plotly for real charts
- **Web interface:** Build a Streamlit app for interactive exploration
- **Database:** Use a proper database instead of CSV files
- **Performance:** Make it faster for larger datasets

### Data Improvements
- **Full dataset:** Analyze all CORD-19 papers, not just a sample
- **Real-time updates:** Get the latest research papers
- **Multiple sources:** Combine different research databases

## Reflection

### What Went Well
- Got the basic analysis working with built-in Python libraries
- Found interesting patterns in the data
- Created a complete pipeline from raw data to insights
- Learned a lot about data cleaning and processing

### What Was Difficult
- Dealing with messy, real-world data
- Package installation issues on my computer
- Figuring out the best way to analyze text data
- Making the results easy to understand

### Most Important Learning
The biggest thing I learned is that **data cleaning takes way more time than the actual analysis!** About 70% of my work was just getting the data into a usable format. This is apparently normal in data science, but it was surprising to me.

Also, I realized that you don't always need fancy tools - sometimes simple approaches work just as well and are easier to understand.

## Resources I Used

- **Python Documentation:** For learning about built-in libraries
- **CORD-19 Dataset:** Original data source from Kaggle
- **Stack Overflow:** For troubleshooting coding issues
- **Course Materials:** Class notes on data analysis techniques

## Running the Full Version

If you want to try the advanced version with better visualizations:

```bash
pip install pandas matplotlib seaborn wordcloud
python covid_analysis.py
```

Or for the web interface:
```bash
pip install streamlit
streamlit run simple_streamlit_app.py
```

---

**Note:** This was a really interesting assignment! I learned a lot about both the technical side of data analysis and the actual research landscape during COVID-19. The data tells a fascinating story about how the scientific community responded to the pandemic.
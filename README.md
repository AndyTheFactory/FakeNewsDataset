# FakeNewsDataset

a consolidated and cleaned up version of the opensources Fake News dataset
Fake News Corpus (cite) comprises 8,529,090 individual articles, classified into 12 classes: reliable, unreliable, political, bias, fake, conspiracy, 
rumor clickbait, junk science, satire, hate and unknown. The articles were scraped between the end of 2017 and the beginning of 2018 from various 
news websites, totaling 647 distinct sources, collecting articles dating from various years leading to the 2016 US elections and the year after. 
Documents were classified based on their source, based on the curated website list provided by opensources.co using a leading to a 
high imbalanced class distribution.

This consolidated and cleaned Fake News Corpus Dataset is a refined and enhanced version of the "opensources.co Fake News dataset". 
This dataset, is a valuable resource for research and analysis in the domain of misinformation, disinformation, and fake news detection.

The oroginal Fake News Corpus comprises a vast collection of 8,529,090 individual articles, categorized into 12 distinct classes:  reliable, unreliable, political, bias, fake, conspiracy, 
rumor clickbait, junk science, satire, hate and unknown.

The articles within this dataset were systematically gathered by the original authors through web scraping activities 
conducted between the end of 2017 and the beginning of 2018.
These articles were sourced from a diverse range of news websites, resulting in a compilation from 647 distinct online sources. 

Documents were classified based on their source, using a curated website list provided by opensources.co, 
a crowdsourced platform for tracking online information sources. Their proposed source classification method, was based on six criteria: 
- Title and Domain name analysis,
- “About Us” analysis,
- source or study mentioning,
- writing style analysis,
- aesthetic analysis and social media analysis.


After extensive data cleaning and duplicate removal we retain 5,915,569 records

## Languages

English

## Data Sample


An example record looks as follows.

```
{
  'id': 4059480,
  'type': 'political',
  'domain': 'dailycaller.com',
  'scraped_at': '2017-11-27',
  'url': 'http://dailycaller.com/buzz/massachusettsunited-states/page/2/',
  'authors': 'Jeff Winkler, Jonathan Strong, Ken Blackwell, Pat Mcmahon, Julia Mcclatchy, Admin, Matt Purple',
  'title': 'The Daily Caller',
  'content':'New Hampshire is the state with the highest median income in the nation, according to the U.S. Census Bureauâ€™s report on income, poverty and health insurance',
}
```

## Data Fields

- `id`: The unique article ID
- `type`: the label of the record (one of: reliable, unreliable, political, bias, fake, conspiracy, 
rumor clickbait, junk science, satire, hate)
- 'scraped_at': date of the original scrape run
- 'url': original article url
- 'authors': comma separated list of scraped authors
- 'title': original scraped article title
- `content`: full article text

## Data Statistics


Label | Nr Records
:---| :---:
reliable    |  1807323
political   |   968205
bias        |   769874
fake        |   762178
conspiracy  |   494184
rumor       |   375963
unknown     |   230532
clickbait   |   174176
unreliable  |   104537
satire      |    84735
junksci     |    79099
hate        |    64763
----------- | ---------
total | 5915569 

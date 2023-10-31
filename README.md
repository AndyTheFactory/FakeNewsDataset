# FakeNewsDataset
a consolidated and cleaned up version of the "opensources.co Fake News dataset"

**To Download, check the [Releases](https://github.com/AndyTheFactory/FakeNewsDataset/releases)**

The original Fake News Corpus comprises **8,529,090** individual articles, classified into 12 classes: *reliable, unreliable, political, bias, fake, conspiracy, 
rumor clickbait, junk science, satire, hate and unknown*. The articles were scraped between the end of 2017 and the beginning of 2018 from various 
news websites, totaling 647 distinct sources, collecting articles dating from various years leading to the 2016 US elections and the year after. 
Documents were classified based on their source, based on the curated website list provided by opensources.co using a leading to a 
high imbalanced class distribution. Their proposed source classification method, was based on six criteria: 
- Title and Domain name analysis,
- “About Us” analysis,
- source or study mentioning,
- writing style analysis,
- aesthetic analysis and social media analysis.

After extensive data cleaning and duplicate removal we retain 5,915,569 records, downloadable from huggingface or in the [Releases](https://github.com/AndyTheFactory/FakeNewsDataset/releases) tab

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
reliable    |  1,807,323
political   |   968205,
bias        |   769,874
fake        |   762,178
conspiracy  |   494,184
rumor       |   375,963
unknown     |   230,532
clickbait   |   174,176
unreliable  |   104,537
satire      |    84,735
junksci     |    79,099
hate        |    64,763
----------- | ---------
total | 5,915,569 

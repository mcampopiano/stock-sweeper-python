# Python Stock Sweeper

I completed this project following along with Sam Focht at [https://www.youtube.com/watch?v=oZSNFFdkEP0&list=PLaYT64KWZAEPe5pYXZkVO4Rnt1pyneQzP](
https://www.youtube.com/watch?v=oZSNFFdkEP0&list=PLaYT64KWZAEPe5pYXZkVO4Rnt1pyneQzP)

## How it works
Downloaded a list of publicly traded companies from [nasdaq.com](https://www.nasdaq.com/market-activity/stocks/screener?exchange=nasdaq&letter=0&render=download), looped through it to get all of the symbols, then made calls to the TDAmeritrade API to get certain information for each of them, including P/E and PEG ratios, 52 week high and net profit margins. With this information, additional filters allow the user to view only companies that meet a certain criteria.

### Things learned during this project
1. How to use pandas to:
  1. Read excel and CSV files;
  1. Create a data frame
1. How to use Pickle to autocreate and name files
1. How to create a loop to get all desired information from the api (since the app makes several thousand requests, and the api only allows 500 at a time, used a while loop and incremented start and end points to automatically loop through 500 at a time until all were complete.)

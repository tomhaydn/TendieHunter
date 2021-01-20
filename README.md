# Introduction & Explanation

TendieHunter is a cli-based tool to detect and plot asx stocks being heavily discussed within the ASX_Bets/other reddit communities. The program is built on python and uses the [PSAW PushShift API Wrapper](https://pypi.org/project/psaw/).

Tested working on Python 3.7.7, no other tests.

The information you receive from this package should not be taken as financial advice and is purely an attempt to showcase the memery in these types of pump and dump subreddits.

## Installation

```
1. git clone https://github.com/tomeady/TendieHunter.git
2. pip install
```

## Usage

```
1. cd TendieHunter
2. python TendieHunter.py
```

## Arguments

- Datatype
- Default
- Descriptions

```
--sub
```
- string
- ASX_Bets
- The subreddit to target

```
--limitPerDay 
```
- integer (>=1&&<=500)
- 250
- The limit of submissions to process per day


```
--backDate 
```
- integer (>=1&&<=180)
- 30
- The amount of days back from today to process


```
--minRequiredMentions 
```
- integer (>=1&&<=10)
- 3
- The minimum required mentions on a given day to be plotted

## Examples

```
python TendieHunter.py --backDate 50 --minRequiredMentions 1 --limitPerDay 500
```

![Example 1](https://polarhcms.com/api/v1/media/object/478/1611107734651_Screenshot%202021-01-20%20125523.png)

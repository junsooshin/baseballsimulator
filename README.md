# Baseball Game Simulator in Python

Name: Junsoo Derek Shin

Date: 13 June 2017

## Running this program:

`python baseball.py lineup1.txt lineup2.txt`

For the lineup files, put team name (any string is fine), full names of 9 
batters, full name of a pitcher, separated by commas and in single line.

## Important Notes:
- Players with names used by other players don't work (for 2016, Chris Young
  and Matt Duffy are the only such players).

- In the batter and pitcher files, I manually modified "Name" column name to 
  "Name" by stripping strange characters.

- In the league file, I manually modified "Season" column name to "Season" by 
  stripping strange characters.

- Modified Enrique Hernandez's name by getting rid of accent marks.

## Data sources:
- 2016 Batting (2016FanGraphsBatting.csv)
	
	<http://www.fangraphs.com/leaders.aspx?pos=all&stats=bat&lg=all&qual=0&type=8&season=2016&month=0&season1=2016&ind=0&team=&rost=&age=&filter=&players=>

- 2016 Pitching (2016FanGraphsPitching.csv)
	
	<http://www.fangraphs.com/leaderssplits.aspx?splitArr=&strgroup=season&statgroup=1&startDate=2016-3-1&endDate=2016-11-1&filter=IP%7Cgt%7C0&position=P&statType=player&autoPt=true&sort=19,-1&pg=0>

- 2016 League (2016FanGraphsLeague.csv)
	
	<http://www.fangraphs.com/leaders.aspx?pos=all&stats=bat&lg=all&qual=0&type=0&season=2016&month=0&season1=2016&ind=0&team=0,ss&rost=0&age=0&filter=&players=0>

- 2016 Play-by-play and Retrosheet BEVENT software (2016plays.txt)
	
	<http://www.retrosheet.org/game.htm>

	<http://www.retrosheet.org/tools.htm>

	<http://www.retrosheet.org/datause.txt>

## Sources:
- Overall guide and inspiration

   <http://www.hardballtimes.com/10-lessons-i-learned-from-creating-a-baseball-simulator/>

- The Odds Ratio Method

   <http://www.insidethebook.com/ee/index.php/site/comments/the_odds_ratio_method/>

- Python-related sources

	<https://stackoverflow.com/questions/9282967/how-to-open-a-file-using-the-open-with-statement>
	<https://stackoverflow.com/questions/14091387/creating-a-dictionary-from-a-csv-file>
	<https://stackoverflow.com/questions/10712002/create-an-empty-list-in-python-with-certain-size>
	<https://stackoverflow.com/questions/39345995/how-does-python-return-multiple-values-from-a-function>
	<https://stackoverflow.com/questions/4071396/split-by-comma-and-strip-whitespace-in-python>
	<https://stackoverflow.com/questions/34053257/multiple-variables-for-loop-python>
	<https://stackoverflow.com/questions/13784192/creating-an-empty-pandas-dataframe-then-filling-it>
	<https://stackoverflow.com/questions/3162271/get-loop-count-inside-a-python-for-loop>
	<https://stackoverflow.com/questions/6667201/how-to-define-two-dimensional-array-in-python>
	<https://stackoverflow.com/questions/4930404/how-do-get-more-control-over-loop-increments-in-python>
	<https://stackoverflow.com/questions/8244915/how-do-you-divide-each-element-in-a-list-by-an-int>
	<https://www.tutorialspoint.com/python/python_break_statement.htm>
	<https://stackoverflow.com/questions/4265988/generate-random-numbers-with-a-given-numerical-distribution>

- getting a list of keys and a list of values from a dictionary
  (tried to get rid of the total before putting the lists into choice() method, but the way I'm doing doesn't seem to be stable.)
  (list comprehension with a condition doens't work because it removes both total and a result if that result is the only one.)

	<https://www.python.org/dev/peps/pep-3106/>
	<https://docs.python.org/3.6/tutorial/datastructures.html#dictionaries>

- Ways to avoid chain indexing and use multi-axes indexing (df['a']['b'] vs. df.loc['a','b'])

	<http://pandas.pydata.org/pandas-docs/stable/indexing.html#indexing-view-versus-copy>
	<https://stackoverflow.com/questions/41253170/whats-the-alternative-to-pandas-chain-indexing>
	<https://stackoverflow.com/questions/21463589/pandas-chained-assignments>

## Things to be implemented in the future:
There are a lot of things to include in the baseball simulator, but pitcher 
management is the next thing to tackle, since right now the starting pitcher 
completes the entire game.


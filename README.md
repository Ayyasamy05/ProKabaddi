#
# upGrad Pro Hacking League

Pro Kabaddi League is a professional-level kabaddi league that started in 2014. Currently, the League is in its 7th season, which started on 20 July 2019 with the first match between U Mumba and Telugu Titans. The final match will be played on 19 October 2019.The aim of this project is to predict various outcomes at the end of the tournament.

## **Predictions to be achieved**

1.Predict the winner of the tournament.
2.Predict the top team in the points table after the completion of the league matches.
3.Predict the team with the highest points for successful raids.
4.Predict the team with the highest points for successful tackles.
5.Predict the team with the highest super-performance total.
6.Predict the player with the highest SUCCESSFUL RAID percentage.
7.Predict the player with the highest SUCCESSFUL TACKLE percentage.

## **Prerequisites**

1.Any Python Software – to run Python code (Jupyter Notebook used)     
2.Input data to make predictions – Data gathered from below websites

-   https://www.prokabaddi.com/stats
-   https://www.sportskeeda.com/go/pro-kabaddi/stats

3.The below input files are used for this project. Only data related with season 7 pro kabaddi league is used for predictions.

-   Schedule.csv           - This file contains the entire season 7 schedule with winners, unfinished matches will not have winner
-   Playoff.csv            - This file contains the details of playoff matches schedule
-   Raid\_Points.csv        - Raid points of each team
-   Tackle\_Points.csv      - Tackling points of each team
-   Super Raids.csv        - Super raids of each team
-   Super Tackles.csv      - Super tackles of each team
-   All-outs inflicted.csv - All-outs inflicted by each team
-   All-outs conceded.csv  - All-outs conceded by each team
-   Raider details.csv     - Top10 raider details about total raids and successful raids
-   Tackler details.csv    - Top10 tackler details about total tackles and successful tackles

## **Process (How the predictions are made)**

The below mentioned logics are used to make the predictions.

**Predict the top team in the points table after the completion of the league matches**

- Fetch the schedule file with winner details
- Split the schedule file into completed matches, non completed matches
- Predict the outcome of upcoming matches based on earlier results in season 7.
- Combining both the files into single file. Now this combined file will have full schedule with results.
- Calculate number of wins by each team and rank the teams based on the winning points.
- The top ranking team is table topper of league matches

 

**Predict the winner of the tournament.**

- Replacing team names in playoff time table based on the predicted ranking table
- Apply the winner predictions used in the previous tasks. If the number of matches won by teams against each other is same then the total points scored is considered to choose the winner.

**Predict the team with the highest points for successful raids.**

- Find number of matches will be played by each team based on the predicted results
- Calculate the total raid points by taking the average of points scored till now and multiply it with number of matches will be played by each team.

 

**Predict the team with the highest points for successful tackles.**

- Find number of matches will be played by each team based on the predicted
- Calculate the total tackle points by taking the average of points scored till now and multiply it with number of matches will be played by each team.

 

**Predict the team with the highest super-performance total.**

- Fetch the details of super-raids, super-tackles, all-outs inflicted in the tournament and all-outs conceded in the tournament.
- Calculate the Super-performance total using formula:

  _S.P.T. = Total number of super-raids in the tournament +_

  _total number of super-tackles in the tournament +_

  _total number of all-outs inflicted in the tournament -_

  _total number of all-outs conceded in the tournament_

**Predict the player with the highest SUCCESSFUL RAID percentage.**

- Fetch top 10 player details of total raids and successful raids count.
- Calculate the successful raid percentage



**Predict the player with the highest SUCCESSFUL TACKLE percentage.**

- Fetch top 10 player details of total tackles and successful tackles count.
- Calculate the successful tackles percentage.



## **Prediction Results**

1.Winner of the tournament. - **Bengal Warriors**   
2.Top team in the points table after the completion of the league matches. - **Dabang Delhi K.C.**   
3.Team with the highest points for successful raids. - **Bengal Warriors**   
4.Team with the highest points for successful tackles. - **Haryana Steelers**   
5.Team with the highest super-performance total. - **Bengal Warriors**   
6.Player with the highest SUCCESSFUL RAID percentage. - **Pawan Kumar Sehrawat**   
7.Player with the highest SUCCESSFUL TACKLE percentage. - **Fazel Atrachali**   

## **Built With**

- Jupyter Notebook – Software used
- Python – Programming Language used
- csv – Input file format used
- web-scraping – Manually done.

## **Authors**

- **Praful Turanur**  – [_prafulturanur2192@gmail.com_](mailto:prafulturanur2192@gmail.com)
- **Amrutha Shenoy –** [_amritakshenoy3435@gmail.com_](mailto:amritakshenoy3435@gmail.com)
- **Ayyasamy Nataraj**  – [_ayyasamy2301@gmail.com_](mailto:ayyasamy2301@gmail.com)

## **Acknowledgments**

- This project is done as part of upGrad Pro Hacking Challenge.

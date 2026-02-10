### Dataset Documentation

Due to the significant file size (exceeding 300MB), the primary data source is hosted externally. This repository utilizes the **European Soccer Database**.

#### Source Information
The data used in this project is a comprehensive collection of match statistics and player attributes from over 25,000 matches and 10,000 players across various European leagues.

#### Access Link
You can download the original SQLite database file here:
[European Soccer Database on Kaggle](https://www.kaggle.com/datasets/hugomathien/soccer)

#### Data Structure
The database consists of the following relational tables:
* `Country`: European football nations.
* `League`: Professional leagues within those nations.
* `Match`: Match details and outcomes.
* `Player`: Personal information for players.
* `Player_Attributes`: Extensive historical skill ratings (Primary table used in this project).
* `Team`: Information on various clubs.
* `Team_Attributes`: Club-specific performance data.



## Usage Note
After downloading `database.sqlite`, place it in your local `/input/` directory to ensure the scripts reference the data correctly.

![](https://github.com/feini-loves-dape/dape-dashboard/blob/main/images/dape_banner.png?raw=true)

# DAPE NFT Dashboard
Build a dashboard to track twitter follower and opensea floor prices of your favorite nft projects

# Requirements
- MySQL Database or similar
- PHP Server with Cronjobs
- Grafana

# Get started
Setup a MySQL database and import mysql/db.sql including sample entries for DAPE on Twitter and MAYC on OpenSea.

Put all the files from the php/ folder to your webserver.

Edit php\includes\vars.php and enter your database credentials.
Edit php\includes\functions.php and enter your Bearer Token for the Twitter API. Details in the comments.

Setup a cronjob on the files php/php_cronjob_opensea.php and php/php_cronjob_twitter.php.

Install Grafana (i installed it on a raspberry pi, but you can also easily install it on a windows machine) and add your DB in Configuration->Data sources.

Launch Grafana and import the dashboard i prepared for you grafana\Grafana_NFTDashboard.json.

You should be ready to go now!

Discord: feini#2769


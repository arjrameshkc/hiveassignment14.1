# hiveassignment14.1
CREATE DATABASE IF NOT EXISTS CUSTOM_DB;
SHOW DATABASES;
use custom_db;
create table if not exists temperature_data
(
date string,
zipcode int,
temperature int
)
row format delimited
fields terminated by ',';

LOAD DATA LOCAL INPATH '/home/acadgild/downloads/dataset.txt' INTO TABLE temperature_data;

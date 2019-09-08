# Create and use database for Assignment 2

/*create database 607_HW2;
use 607_HW2;*/

# Create table 1 for Movies

create table movies (
movieid int not null auto_increment,
moviename varchar(100) not null,
movieyear int,
primary key (movieid)
);

# Insert values into table 1 - Movies

insert into movies (moviename, movieyear) 
values 		('Spider-man: Far from home', 2019),
			('Avengers: End Game', 2019),
            ('The Lion King', 2019),
            ('Aladdin', 2019),
            ('Shazam!', 2019),
            ('Dark Phoenix', 2019);
            
# Create table 2 for Movie's ratings

create table respondent1 (
ratingid int not null auto_increment,
movieid int not null,
John int not null,
James int not null,
Peter int not null,
Carol int not null,
Steve int not null,
primary key (ratingid),
foreign key (movieid) references movies(movieid)
);

# insert values by Respondents

insert into respondent1 (movieid, John, James, Peter, Carol, Steve)
values		(1, 4, 5, 4, 4, 5),
			(2, 5, 5, 4, 3, 4),
            (3, 3, 4, 4, 4, 5),
            (4, 4, 4, 3, 4, 5),
            (5, 4, 4, 5, 3, 3),
            (6, 3, 3, 4, 4, 4);

# Join both tables for master table

select * from movies
left join respondent1
on movies.movieid = respondent1.movieid;

# ALTER USER 'root'@'localhost' IDENTIFIED WITH MYSQL_NATIVE_PASSWORD BY 'password';


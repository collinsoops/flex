
# Project Title
Design to code  is a simple page created by html, css-flexbox. it also has database.


## Installation

### Requirements

Requirements include:
* HTML
* CSS
* PHP
* SQL 
*APACHE SERVER

check if git is installed and up-to-date
`$ git --version

If its not installed run
visit https://git-scm.com/ and download



#### Install xampp

```
https://www.apachefriends.org


### Setting Up Database

#### Import database

Create the database first
- **Option 1**
    Change user to root
    
    Create database
    
    `$ CREATE DATABASE flex; `

Import database from sql file

Import flex.sql in the files

or create tables

CREATE TABLE `activity` (
  `activity_id` int(11) NOT NULL,
  `activity` varchar(100) NOT NULL,
  `activity_time` datetime NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1;


INSERT INTO `activity` (`activity_id`, `activity`, `activity_time`) VALUES
(1, 'Deployed warkation to production', '0000-00-00 00:00:00'),
(2, 'Deployed Kitetail to staging', '0000-00-00 00:00:00'),
(3, 'Deployed warkflow to staging', '0000-00-00 00:00:00'),
(4, 'Deployed easywire to production', '0000-00-00 00:00:00'),
(5, 'Deployed warkation to production', '0000-00-00 00:00:00');

CREATE TABLE `projects` (
  `project_id` int(11) NOT NULL,
  `repo_name` varchar(30) NOT NULL,
  `url` text NOT NULL,
  `type` text NOT NULL,
  `time` time NOT NULL,
  `address` text NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1;


INSERT INTO `projects` (`project_id`, `repo_name`, `url`, `type`, `time`, `address`) VALUES
(0, 'Warkation', 'www.github.co.ke', '', '12:14:45', 'United states'),
(1, 'Easywire', 'www.github.co.ke', '', '12:14:45', 'United states'),
(3, 'Workflow', 'www.github.io', 'laravel', '00:00:00', 'United States'),
(4, 'Talkslides', 'www.laravel.co.ke', 'Nextjs', '00:00:00', 'United states');



CREATE TABLE `user` (
  `user_id` int(11) NOT NULL,
  `full_name` varchar(30) NOT NULL,
  `email_id` text NOT NULL,
  `password` text NOT NULL,
  `address` text NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1;



INSERT INTO `user` (`user_id`, `full_name`, `email_id`, `password`, `address`) VALUES
(1, 'Debbie Lewis', 'debbi@gmail.com', '1234', 'United States');


ALTER TABLE `activity`
  ADD PRIMARY KEY (`activity_id`);


ALTER TABLE `projects`
  ADD PRIMARY KEY (`project_id`);


ALTER TABLE `user`
  ADD PRIMARY KEY (`user_id`);
COMMIT;




#### Setting up the project on git

To itialize

```
$ git init
```

Clone the project from the repository

```
$ git clone https://github.com/collinsoops/design-to-code-.git
```

The folder structure will be as follows after cloning

```


css
.getignore
README.md
flex.html
flex.php
flex.sql
home-screens.03-constrained-multi-column-xl.png
httpstailwindui_003.png
img.jpg
logo.PNG 
```

Other commands used include:


```
$ git add .
```
```
$ git commit -m "updated files with database"
```
```
$ git status 
```
```
$ git remote add origin https://github.com/collinsoops/design-to-code-.git
```

```
$ git push origin master
```

## Running 

Access the site on browser


### coding style 

-css-flexbox

## Deployment

Add additional notes about how to deploy this on a live system


## Authors

* ** collinsoops** - *Initial work* https://github.com/collinsoops/flex/


## License
no licence

## Acknowledgments

* william



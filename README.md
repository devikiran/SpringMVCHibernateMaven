SpringMVCHibernateMaven
=======================
This project is base sample example of Spring integration with Hibernate using maven
we have used Postgres as our backed db

just run the folowing query in your postgresql db before running the project
CREATE TABLE teams
(
  id serial NOT NULL,
  name character(40),
  rating integer,
  CONSTRAINT teams_pkey PRIMARY KEY (id)
)
WITH (
  OIDS=FALSE
);

if you want to use mysql use the following query 

CREATE TABLE `teams` (
  `id` int(6) NOT NULL AUTO_INCREMENT,
  `name` varchar(40) NOT NULL,
  `rating` int(6) NOT NULL,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB AUTO_INCREMENT=6 DEFAULT CHARSET=utf8;

and also do the necessasary changes in the  application.properties under src/main/resources.

For any queries please feel free to mail me at devikiran90@gmail.com

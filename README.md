

This has 2 parts Django and scrapy projects 

1> django_project is the django project and it has an app called questions.
2> scrapy_project is the scrapy project and has a spider called stackoverflow.

To initiate the crawler in scrapy_project path we have to give 
	$  scrapy crawl Crawler
To run the server we have to give in django_project path
	$  python manage.py runserver
 
 1>	a>Scrapy (Stackoverflow.py) contains the spider(Spider()) which has methods to 
	crawl the required page and the data is stored as items(type:scrapyfield)

	b> The items are loaded to the pipeline where items are processed 
	and then it is saved to the database. The data to be stored are stored in the items 
	which is of the method described by the Django models.

 2>	a> Django Models are created for database(ORM).
    	b> In Views functions are used to get the data from database.
     	c> The display of the data from database is done in the list.html file. 

  


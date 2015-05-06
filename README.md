# Exercise 3

# RDF and SPARQL

3.1 RDF

@prefix foaf: <http://xmlns.com/foaf/0.1/> 

@prefix xsd: <http://www.w3.org/2001/XMLSchema#>

<https://www.facebook.com/jaime.e.ramirez.5>,
	rdf:type foaf:person;
	foaf:Name "Jaime Ramirez"
	foaf:knows <https://www.facebook.com/MichaSubramaniam>, <https://www.facebook.com/pascal.zerzuben>
	foaf:interest <http://de.dbpedia.org/page/Fitness>, <http://dbpedia.org/page/Computer>, 			<http://dbpedia.org/property/mainInterests/soccer> <http://dbpedia.org/property/mainInterests/music>
	foaf:mbox <ramij2@bfh.ch.ch>
	foaf:pastProject <https://github.com/Araucano88/WBTC_2015#exercise-1>
	



3.2 SPQRQL Queries



# Exercise 2

<head>
<title>
Jaime Estéban Ramirez`s Profile
</title>
</head>
<body>

<ul><p><b>Social Media</b></p></ul>
<li> <p about="https://www.facebook.com/jaime.e.ramirez.5">
	jaime is on <a rel="foaf:member" href="http://www.facebook.com">Facebook</a>.</p></li>
<li> <p about="https://instagram.com/j_e_ramirez">
	jaime is on <a rel="foaf:member" href="http://www.instagram.com">Instagram</a>.</p></li>
</ul>

<ul><p><b>Relationships</b></p></ul>
<li> <p about="http://jaimeramirez.ch/relationships">
	My brother <a rel="foaf:knows" href="https://www.facebook.com/robinson.kundert?fref=ts">Robinson</a></p></li>
<li> <p about="http://jaimeramirez.ch/relationships">
	My bestfriend <a rel="foaf:knows" href="https://www.facebook.com/Bitoooor?fref=ts">Victor</a></p></li>
</ul>

<ul><p><b>Interests</b></p></ul>
<li> <p about="http://jaimeramirez.ch/interests">
	jaime is interested in <a rel="foaf:interest" href="http://en.wikipedia.org/wiki/Association_football">soccer</a>.</p></li>
<li> <p about="http://jaimeramirez.ch/interests">
	jaime is playing in <a rel="foaf:interest" href="http://www.fcwabern.ch/">Fc Wabern</a>.</p></li>
<li> <p about="http://jaimeramirez.ch/interests">
	jaime is interested in <a rel="foaf:interest" href="http://en.wikipedia.org/wiki/Music">music</a>.</p></li>
<li> <p about="http://jaimeramirez.ch/interests">
	jaime is interested in <a rel="foaf:interest" href="http://en.wikipedia.org/wiki/Information_technology">Information technology</a>.</p></li>
</ul>

<ul><p><b>Education and work experience</b></p></ul>
<li> <p about="http://jaimeramirez.ch/workexperience/administration">
	jaime is working <a rel="foaf:workplaceHomepage" href="https://ict.swisscom.ch/2014/12/startschuss-fuer-die-campus-ambassadoren/"> Swisscom AG - Campus Ambassador </a>.</p></li>
<li> <p about="http://jaimeramirez.ch/education/university/bachelor">
	jaime is studying <a rel="foaf:education" href="http://en.wikipedia.org/wiki/Business_informatics">Information Systems</a> at <a rel="foaf:interest" href="http://www.bfh.ch/">Bern University of Applied Sciences</a>.</p></li>
</ul>

</body>
</html>

Quellen: https://www.youtube.com/watch?v=N_GpbwMHeMQ 
	https://www.youtube.com/watch?v=xnUVHaPYMlg


---------------------------------------------------------------------------------------------------------------


# Exercise 1
This repository is written in the module Web Technology at Bern University of Applied Science, Bechelor in Business Information Systems.

```What is the tasks of this exercise? ```

- design IRI patterns for a dataspace on the web (own profile)
- describing why the IRI patterns were chosen like this
- explaning in a short summary what "Linked Data" is 

## Design my own IRI patterns

I think that using my name as the domain address is a reasonable option.
Everyone who knows me and want to have information about me can remember my adress because of my name.

I have decided to take a top-level-domain ".ch".
For the hosting I would recommend the Swisscom. Swisscom can guarantee a secure server host. --> Server locacated in Switzerland.

Homepage URI  | Description
------------- | -------------
http://www.jaimeramirez.ch/home  | This is the Landingpage/Startpage. Like we know it all from a Webpage.
http://www.jaimeramirez.ch/about | On this part of the Webside you can find information about me and my life
http://www.jaimeramirez.ch/education http://www.jaimeramirez.ch/education/bfh http://www.jaimeramirez.ch/education/feusi| On this part of the Webside you can finde information about my school career
http://www.jaimeramirez.ch/experciences/swisscom/campus_ambassador http://www.jaimeramirez.ch/experciences/swisscom/it_security_intership | On this part of the Webside you can find information about my work experience. 
http://www.jaimeramirez.ch/interested_in http://www.jaimeramirez.ch/interested_in/hobbies http://www.jaimeramirez.ch/interested_in/sport http://www.jaimeramirez.ch/interested_in/it | On this part of the Webside you can find information about my hobbies and things wich interest me.
http://www.jaimeramirez.ch/contactme | On this part of the Webside you can find any information about me to contact me. It is like an bussines card.
http://www.jaimeramirez.ch/links | On this part of the Webside you found links wich I like to link.

## Design my own IRI patterns other solution
Jaime Ramirez (http://jaimeramirez.ch/)
Education
•	School X (http://jaimeramirez.ch/school/#x)
•	School Y (http://jaimeramirez.ch/school/#y)
Work experience
•	Company A (http://jaimeramirez/company/#a)
•	Company B (http://jaimeramirez/company/#b)
Hobbies
•	Hobby P (http://jaimeramirez/hobbies/#p)
•	Hobby Q (http://jaimeramirez/hobbies/#q)
•	Hobby R (http://jaimeramirez/hobbies/#r)


# What is Linked Data? - by Jaime
Even the children in our time have a basic technical experience, so I hope that will be understandable for them. 

Linked data is based on raw data, which exists in the web. Raw data could be a birthday, an address, a name and so on. Linked data however, relates the raw data together and give the raw data a sense. As an Example, if the name is relate to an address and a birthday it is no longer just a name, instead it is a person with a defined birthday and an address. This little example could be expanding to further data (respectively persons, places, things and so on) and properties. 

# What is Linked Data? from the internet

Imagine you’re in a huge building with several storeys, each with an incredible large amount of rooms. Each room has tons of things in it. It’s utterly dark in that building, all you can do is walk down a hallway till you bang into a door or a wall. All the rooms in the buildings are somehow connected but you don’t know how. Now, I tell you that in some rooms there is a treasure hidden and you’ve got one hour to find it.

Here comes the good news: you’re not left to your own resources. You have a jinn, let’s call him Goog, who will help you. Goog is able to take you instantaneously to any room once you tell him a magic word. Let’s imagine the treasure you’re after is a chocolate bar, and you tell Goog: “I want Twox”. Goog tells you now that there are 3579 rooms where there is something with “Twox” in there. So you start with the first room Goog suggests to you, and as a good jinn he of course takes you there immediately; you don’t need to walk there. Now you’re in the room you put everything you can grab into your rucksack and get back outside (remember, you can’t see anything, in there). Once you are outside the building again and can finally see what you’ve gathered you find out that what is in your rucksack is not really what you wanted. So, you have to get back into the building again and try the second room. Again, and again till you eventually find the Twox you want (and you are really hungry now, right?).

Now, imagine the same building but all the rooms and stairs are marked with fluorescent stripes in different colours, for example a hallway that leads you to some food is marked with a green stripe. Furthermore, the things in the rooms have also fluorescent markers in different shapes. For example, Twox chocolate bars are marked with green circles. And there is another jinn now as well- say hello to LinD. You ask LinD the same thing as Goog before: “I want Twox” and LinD asks you: do you mean Twox the chocolate bar or Twox the car? Well, the chocolate bar of course, you say and LinD tells you: I know about 23 rooms that contain Twox chocolate bars, I will get one for you in a moment.

How can LinD do this? Is LinD so much more clever than Goog?

Well, not really. LinD does not understand what a chocolate bar is, pretty much the same as Goog does not know. However, LinD knows how to use the fluorescent stripes and markers in the building, and can thus get you directly what you want.

You see. It’s the same building and the same things in there, but with a bit of a help in forms of markers we can find and gather things much quicker and with less disappointments involved.

In the Linked Data Web we mark the things and hallways in the building, enabling jinns such as LinD to help you to find and use your treasures. As quick and comfortable as possible and no matter where they are.

# Reference List
- https://webofdata.wordpress.com/2010/05/20/linked-data-for-dummies/ (24.04.2015)
- https://www.youtube.com/watch?v=4x_xzT5eF5Q (24.04.2015)


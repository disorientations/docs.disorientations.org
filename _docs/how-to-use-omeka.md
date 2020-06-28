---
tags: docs, how-to
---

# How to use Omeka

* Naming convention
    * What it says on the title
* Place
    * For now Google the location of the college and enter city and state
    * Later we can used linked data
* Class
    * use "Document"
    * for the future, examine if there's a better class for our materials

---

## Emma's notes from 6/22

#### two platforms for archiving
* collective access (more robust archival tool)
* omeka is an alternative comes out of the digital humanities world
#### omeka
* designed around collections of items
* omeka classic: web publishing platform
* decided to fork it; still maintain omeka classic 
* we use omeka s, new version
* pretty well designed and user friendly
* variation and s and classic is you can store any number of diff collections in s and you can host different sites
* we can catalog other types of student activism, same set of items with different websites, own theme, url, etc. (can branch off!)
* git hub theme (features/theme)

#### omeka core concepts
* everything is called a resource
* items are pages on the site (eg: /item/3)
    * within the item, the media is the pdf that loads
		* item and media are not the same thing; you can have an item that has no media
		* media will have different id
		* you can attach multiple media to one item and categorize them (eg: screen media and print media, low qual and high qual)
		* has many relationship between items and media
		* media must be associated with item, but not vice versa
		* there's a plugin that automatically extract text (not great) 
* dublin core: schema of vocab terms to describe digital and [..] resources; a language of standardized metadata terms (eg: title, body, school, date)
    * standardized archival terms (eg: different kinds of dates, different relations, [referenced by, replaced by, version of])
    * most of it blank for now
    * we use title, date (dcterms: date), as well as dublin core spatial
    * if we wanted to port, we can port dublin core as a schema and map over things properly
	* extract text as a different vocab/taxonomy
	* we can develop a taxonomy (eg: campaign, issue, person)
	* omeka is relational
		* under "relation", you can relate to text, or an omeka resource, link (to item, item sets, media), you can link to multiple things
	* mapping (drop a pin on a map)
	* item sets: powering university categorization
		* items on the right hand side
		* currently: institution name is stored as an item set
#### unused
* we're not really using resource tmeplates (can be used later when with a taxonomy, more later)
* not really using other vocabs besides defaults
	
#### other cool features
* batch actions (eg batch editing)
* csv import by omeka team and daniel
    * has documentation
    * can import item sets or items
    * can comment + check log! can be destructive, ask questions
    * eg: importing two column csv w title and class
        * map title to dublin core title
        * map class to eg: collections, 
        * public
        * owned by 
        * advanced settings > action > you can append, reives, update, delete, etc.
            * check the docs for what they mean
            * create: new resoure for each row (duplicates)
            * append: find by identifier, 
            * revise: replace unless empty
            * replace: remove and (??)
	* right now: spreadsheet is messy, in the future shared google sheet folder (imports from a given date, main spreadsheet)
	* other plugins and api to get data out
	* if we want a project where people can upload and update, we can get data back out of omeka

* adding new item
    * resource template > base resource (can batch edit them in thef uture for unused fields) -* need this for fields!!
    * class: item (bib ontology) documnet, examnine if better class
    * title: copy title from the cover (add clarification if needed)
    * date: year of publication
    * relation: TBD? (not currently in use, but just showing that you can link items to eachother)
    * add to item set for corresponding university/disorientation group so it can show up on front end
    * no convention for uploading media for now
* scalar: creating webs out of a book, not really an archival tool, can be used for that (history of computing)
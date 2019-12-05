### OPEN CORPORATE FACTS / scripts & data
-------------------

This is a repo where we could gather scripts and copies of datasets

The Python notebooks scripts in the repo aim to request the API platform instance put in place by Leonard 
so it is possible to rebuild the datasets and reuse them for other purposes

The scripts are storing json as json files (and csv files soon ?) to the corresponding folders in `/datasets`
The datasets arre split into chunks corresponding to a quantity oif n pages scraped


----------
#### OCF sources 

- OCF official website : [http://opencorporatefacts.fr](http://opencorporatefacts.fr)

- OCF API Platform : 
	- [http://opencorporatefacts.fr/api/corporates?id=<`internal_id`>&CompanyNumber=<`sirene_number`>&page=<`page_number`>](http://opencorporatefacts.fr/api)
	- [http://opencorporatefacts.fr/api/compte_de_resultats?Corporate=<`sirene_number`>&page=<`page_number`>](http://opencorporatefacts.fr/api)

- COMPANIES by CQuest : [http://api.cquest.org/company/<`sirene_number`>](http://api.cquest.org/company/832277370)

- OCF on Code For France : [https://codefor.fr/processes/opencorporatefacts](https://codefor.fr/processes/opencorporatefacts)


------------
#### TEAM

- Leonard 
- JPy 


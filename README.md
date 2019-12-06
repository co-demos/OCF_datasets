### OPEN CORPORATE FACTS / scripts & data
-------------------

This is a repo where we could gather scripts and copies of OCF datasets

The Python notebooks scripts in the repo aim to request the API platform instance put in place by Leonard, get the JSON and save them into .json files, 
so it is possible to rebuild the datasets and reuse them for other purposes...

The scripts are storing the json files (and csv files soon ?) to the corresponding folders in `/datasets`
The datasets arre split into chunks corresponding to a quantity oif n pages scraped : 

- the corporation data in `./datasets/corporations/`
- the account results in `./datasets/account_results/`

----------
#### notebooks

to run the notebooks just open this foldeer and run : 

```bash
jupyter notebook
```

(you need jupyter to do so indeed)

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
- Julien : [JPy](https://github.com/JulienParis)  


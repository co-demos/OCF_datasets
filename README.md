### OPEN CORPORATE FACTS / scripts & data
-------------------

This is a repo where we could gather scripts and copies of OCF datasets

The Python / Jupyter notebooks scripts in the repo aim to request the API platform instance put in place by Leonard, get the JSON and save them into .json files, so it is possible to rebuild the datasets and reuse them for other purposes...

The scripts are storing the json and csv files to the corresponding folders in `/datasets`.

The datasets are split into chunks corresponding to a quantity of n pages scraped : 

- the "corporations" data in `./datasets/corporations/`
- the "account results" data in `./datasets/account_results/`


Note :

For compatibility purposes the `.csv` files created use a tab (`|`) as separator...

----------
#### install jupyter notebooks

You can install all the notebooks dependencies following those steps : 

```bash
# install python virtual env
pip install virtualenv
virtualenv venv

# activate virtual env
source venv/bin/activate

# install dependencies in venv
pip install python-dotenv
# or
pip install -r requirements.txt

# install a kernel of a jupyter notebook in venv
ipython kernel install --user --name=venv

``` 

For some notebooks you'll need to load and access variables stored in a hidden/ignored file `.env`
So just create this file containing those secret variables by copying the `example.env` file and rename it `.env`

Or type :

```bash
touch .env
# or
nano .env
``` 


to run the notebooks just open this folder and run : 

```bash
jupyter notebook
```

(you need jupyter to do so indeed)



----------
#### notebooks 

There are several notebooks we used to get the data back from APIs, copy it to local files, or even send it back to other services : 

- get data from Leonard's API Platform : `load OCF data to file-TEST 3.ipynb`
- split big files into several files : `split_big_json_files.ipynb`
- load files into Pandas and play with it / export them as csv / insert docs to mongo DBs : `JSON files to API or DB.ipynb`

----------
#### OCF sources 

- OCF official website : [http://opencorporatefacts.fr](http://opencorporatefacts.fr)

- OCF API Platform : 
	- [http://opencorporatefacts.fr/api/corporates?id=<`internal_id`>&CompanyNumber=<`sirene_number`>&page=<`page_number`>](http://opencorporatefacts.fr/api)
	- [http://opencorporatefacts.fr/api/compte_de_resultats?Corporate=<`sirene_number`>&page=<`page_number`>](http://opencorporatefacts.fr/api)

- COMPANIES by CQuest : [http://api.cquest.org/company/<`sirene_number`>](http://api.cquest.org/company/832277370)

- OCF on Code For France : [https://codefor.fr/processes/opencorporatefacts](https://codefor.fr/processes/opencorporatefacts)


------------
#### inspirations / ressources 

- ENTHIC project : [http://api.enthic.fr/documentation/index.html](http://api.enthic.fr/documentation/index.html) and their [github](https://github.com/phe-sto/enthic)


------------
#### TEAM

- Leonard : [Leonarf](https://github.com/leonarf)
- Julien : [JPy](https://github.com/JulienParis)  


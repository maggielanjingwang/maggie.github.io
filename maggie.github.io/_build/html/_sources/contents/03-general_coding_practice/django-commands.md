# Django Commands with Database Configurations

### 1. makemigrations
To include the app in our project, and let Django knows to include new app we add it. Let’s run command:
```
$ python manage.py makemigrations
```
You should see something similar to the following:
```
Migrations for 'polls':
  polls/migrations/0001_initial.py
    - Create model Question
    - Create model Choice
```


### 2. Migrate
Some of these applications make use of at least one database table, though, so we need to create the tables in the database before we can use them. To do that, run the following command:
```
$ python manage.py migrate
```

### 3. runserver
Let’s verify your Django project works, run the following commands:
```
$ python manage.py runserver
```
You’ll see the following output on the command line:
```
Performing system checks...

System check identified no issues (0 silenced).

You have unapplied migrations; your app may not work properly until they are applied.
Run 'python manage.py migrate' to apply them.

August 16, 2022 - 15:50:53
Django version 4.1, using settings 'mysite.settings'
Starting development server at http://127.0.0.1:8000/
Quit the server with CONTROL-C.
```

### 4. runscript
##### Registry Import Scripts

Script to import AHA GWTG Heart Failure data into the database using the Dask library.
To run this script, type the following into the terminal:

```
$ python manage.py runscript import_REGISTER_NAME_csv --script-args input_csv='path/to/csv' site_csv='path/to/csv' start_row='row_num'

```

```{seealso}
    input_csv (str): Path to main data csv.
    site_csv (str): Path to site data csv.
    start_row (int): Row number to start importing from. Using this argument assumes that the site
        data has already been imported into the database and does not need to be deleted in order 
        to avoid cascading record deletions. Should only be used when there was an interruption with
        the uploading process and the user would like to start from a specific row instead of reuploading
        the entire main records again.
    
    Note: there have only one empty space between input_csv and site_csv  
```

#### Registry Export Scripts
Script to export AHA GWTG Heart Failure data from database to a CSV
To run this script, type the following into the terminal:
```
$ python manage.py runscript export_REGISTER_NAME_csv --script-args export_csv=csv_root_path
```
```{seealso}
Export_csv is the path to storage export csv.
```

#### Verify import&export data
Describe functions of import and export generally, then more into specifics for each registry Format of the command and arguments
To run this script, type the following into the terminal:
```
python scripts/verify_cad_import_export.py
```

### 5. show_urls
```
$ python manage.py show_urls
```

### 6. shell
let’s hop into the interactive Python shell and play around with the free API Django gives you. To invoke the Python shell, use this command:

```
$ python manage.py shell
```


###  7. Export to .csv or .sas7bdat
Admin export page
User files page
Internal process of how it works

Custom Permissions
How to configure
Structure

Custom Admin Site
How to configure
Structure


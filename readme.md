# FastAPI template.
This template uses FastAPI to create CRUD operations to a MongoDB database.
This project only takes care of the backend part of a project.


# Steps to create this project from scratch locally.
If you don't want to clone this project, here are the steps to create it by your self.


	1. Create new folder.
	2. From terminal in the project folder, open VS Code (code .)
	3. Create root level requirements.txt, and add: 
		fastapi == 0.65.1
		uvicorn == 0.14.0
		motor == 2.4.0
	4. intall vitual environment (if not already installed)
		a. pip install pipenv
	5. activate virtual environment (I can do it from the VS code terminal)
		a. pipenv shell 
	6. install the requierments (the file I created before)
		pipenv install -r requirements.txt
		• The requirements shoud install everything, but if errors, you may need to install : (if so, reset terminal and VS code)
		pip install fastapi 
		pip install uvicorn
	7. create 5 files a root level: (the code is later in this secction)
		.env
		database.py
		main.py
		model.py
		.gitignore
	8. run server
		uvicorn main:app --reload 
		reload mode let me see all the changes on the file with out reloading it
	9. view the server
		http://127.0.0.1:8000
		http://127.0.0.1:8000/docs   (swagger view)
		http://127.0.0.1:8000/api/tasks

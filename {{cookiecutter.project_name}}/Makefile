TARGET={{cookiecutter.project_name}}.zip

all: virtualenv
	./virtualenv/bin/pip install -r ./requirements.txt
	zip ${TARGET} main.py
	cd ./virtualenv/lib/python2.7/site-packages && zip -r ../../../../${TARGET} *

virtualenv:
	virtualenv virtualenv

clean:
	rm -rf virtualenv
	rm -rf ${TARGET}.zip

 

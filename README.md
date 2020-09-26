# Probability Distribution Package Uploaded in PyPi
PyPi is repository in which python packages are stored. This is an exercise to build the python package and store it in PyPi. PyPi has two repositories: pypi.test.org and pypy.org. Accounts must be opened in both separately.

Table of Content

1. Files 
2. Upload Package
3. Instllation

1) Files

Package should be placed in a folder with the following folders and files:

   i) A folder with the name of your package that contains    
      
      a) the Python code that makes up the package
      b) a README.md file
      c) an __init__.py 
      d) license.txt
      e) setup.cfg

   ii) setup.py file
   
2) Upload Package

Follow follwing steps to upload the package:

    i) python setup.py sdist
   
    This command will create extra folder "dist" that contains *.tar.gz file
   
    ii) Install twine:
   
       pip install twine
       
    iii) Upload to the pypi test repository
    
          twine upload --repository-url https://test.pypi.org/legacy/ dist/*
          
          pip install --index-url https://test.pypi.org/simple/ prob-dist-ap
          
    iv)Upload to the pypi repository
    
            twine upload dist/*
            
 3) Installation
            
     The uploaded package cab be installed using 
       
           pip install prob-dist-ap





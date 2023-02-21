# CS421-project2: Python2Vec

## Abstract ##
This project involved implementing a Python2Vec model by training a Word2Vec model with python code.  I applied the Word2Vec model to source code in order to create my own verison, Python2Vec.  In this project, I created several Jupyter Notebooks in which I mined public software repositories for Python code.  I then cleaned my data and trained a Word2Vec model with the source code I collected from the repositiories. I then assesed the model I created and used it to determine the similarity of identifiers in code.  In doing so, I successfully practiced the basics of mining software repositories and data cleaning and tested my model with real-life data to check the similarity of identifiers in code.


## Results ##
After naming each python file in the chosen matplotlib, scikit-learn, and scipy repos, in python_files.txt, I pulled code from those python files, and created a mass text file: alltext.txt.  This file, which is made up of 7302 lines and 59 tokens, was used to create my model using gensim.models.Word2Vec with a window size of 10 and a min_count of 2. 


## Discussion ##
I determined the following similarities of identifiers in code mined from the repositories I chose:
<p><img width="435" alt="Screen Shot 2023-02-21 at 10 13 46 AM" src="https://user-images.githubusercontent.com/30237570/220384031-8adf535d-e30b-47bb-ae55-1b13ba03b886.png"></p>
<p><img width="537" alt="Screen Shot 2023-02-21 at 10 13 53 AM" src="https://user-images.githubusercontent.com/30237570/220384095-c829cfcd-407a-4b72-b3a0-8a56f026b146.png">
 </p>
<p> We can see that 'for' is deemed most similar to 'in', which makes sense in the context of loops and ranges.  'If' is deemed most most similar to 'in', which makes sense in the context of searching for an item within something, like a specific file in a folder.  'Setup' and 'sys', are, as expected, very similar: 99%, as are 'from' and 'import'and 'scikit' and 'scipy'.  Itested some other tokens to demonstrate relationships between identifiers in this model.</p> 


## Extensions ##


## References/Acknowledgements ##
<p>Naser Al Madi</p>
https://www.geeksforgeeks.org/python-list-files-in-a-directory/

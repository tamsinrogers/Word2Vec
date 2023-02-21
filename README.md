# CS421-project2: Python2Vec

## Abstract ##
This project involved implementing a Python2Vec model by training a Word2Vec model with python code.  I applied the Word2Vec model to source code in order to create my own verison, Python2Vec.  In this project, I created several Jupyter Notebooks in which I mined public software repositories for Python code.  I then cleaned my data and trained a Word2Vec model with the source code I collected from the repositiories. I then assesed the model I created and used it to determine the similarity of identifiers in code.  In doing so, I successfully practiced the basics of mining software repositories and data cleaning and tested my model with real-life data to check the similarity of identifiers in code.


## Results ##
After naming each python file in the chosen matplotlib, scikit-learn, and scipy repos, in python_files.txt, I pulled code from those python files, and created a mass text file: alltext.txt.  This file, which is made up of 7302 lines and 59 tokens, was used to create my model using gensim.models.Word2Vec with a window size of 10 and a min_count of 2. 


## Discussion ##
I determined the following similarities of identifiers in code mined from the repositories I chose:
<p><img width="369" alt="Screen Shot 2023-02-21 at 9 59 14 AM" src="https://user-images.githubusercontent.com/30237570/220380197-46cb2876-5db6-411e-967c-e2c1afa7eed3.png"></p>
<p> We can see that 'for' is deemed most similar to 'in', which makes sense in the context of loops and ranges.  'If' is deemed most most similar to 'in', which makes sense in the context of searching for an item within something, like a specific file in a folder.  'Setup' and 'sys', are, as expected, very similar: 99%, as are 'from' and 'import'and 'scikit' and 'scipy'.</p> 


## Extensions ##


## References/Acknowledgements ##
<p>Naser Al Madi</p>
https://www.geeksforgeeks.org/python-list-files-in-a-directory/

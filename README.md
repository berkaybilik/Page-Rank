# Page-Rank
An Implementation of Page Rank Algorithm to Rank Wikipedia Pages

Please put the .mtx file and the notebook in the same directory and change the file for the .mtx file in the code. 

More about the web-wikipedia2009.mtx:
  - The second line contains the dimensions of the matrix that represents the network of Wikipedia pages.
  - Entry (i,j) of this matrix represents the number of links going from the Wikipedia page that is indexed with i to the Wikipedia page that is indexed with j.
  - The rest of the file can be thought of as a dictionary {i:n} where i is a Wikipedia page's index and n is the number of links coming into that page from other Wikipedia pages. If an index is ommitted, it means that there are 0 links coming into that page.
  - The dimensions of the matrix is very large and it is infeasible to store the matrix in its raw form in the memory. So, in the code, sparse matrices are utilised to take advantage of the fact that this matrix is made up of many zeroes.
  - Unfortunately, I couldn't find how the page indexing was done, so I do not know what Wikipedia page was ranked the highest.

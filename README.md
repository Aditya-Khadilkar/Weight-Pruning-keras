# Weight Pruning keras
<h1>Train a dense network and make it sparse by setting the smallest "n%" weights or nodes to zero</h1>
<body>
<p> I have trained a dense fully connected neural network in mnist dataset.<br>
  Then in the first function (prunew) we take a single weight matrix and the % pruning to be done.<br> 
  From the size we find out the number of weights to be pruned (<b>N</b>).<br>
  we create a copy of the given matrix. We then scan throught the copy matrix and find the lowest N absolute values of and set them to 0.<br>
  once the for loop is complete we return the copy.<br>
</p>
<p>
  In this function we make a get a sigle matrix and % nodes to be pruned.<br>
  Make a vector. Calculate the f2 norm of each column and append it to the vector.<br>
  copy the vector, and sort the copy. the amongst the size of the vector find what number is n%?<br>
  get the nth element.<br>
  if vector<br>
  if element > nth element == 1<br>
  else 0<br>
  then multiply weight matrix X vector<br>
  we now have the node pruned matrix.<br>
  compile it into a copy of the model and test for accuracy.<br>
  </body>
  <h1> WHY TO DO THIS?</h1>
  <h3> Accuracy shoots up after retraining!<br></h3>
  <h2>I got 90 % accuracy on the orignal model after pruning it rose to <b>99 %</b></h2><br>
  I have tried multiple pruning percentages to see node pruning accuracy, weight pruning accuracy, and retraining accuracy for both.<br>
  <br>
  <h4>Heres the graph:</h4>
  ![image](https://user-images.githubusercontent.com/35966791/57179613-320acc00-6e9d-11e9-8725-3046aaa558b4.png)
  
  
  

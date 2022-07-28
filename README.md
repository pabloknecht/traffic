# AI50 Traffic experimentation process

To find the rusults shown in the video (0.96 of accuracy) I implemented first a similar version of the CNN presented in class and implemented the following different strategies which improoved the accuracy:
- Increasse the number of neurons. With 172 neurons (4 times the number of road signs) seams to work really well. Adding many more neurons appears to degrade a little the accuracy.
- Increase the number of hiden layers to 3 improoved the accuracy. Increasing any futher had no significant effect.
- Reduce the dropout in the last hidden layer from 0.5 to 0.35 seams to help a little. Increasing it degrade the accuracy.
- The last thing I did was to add another convolution layer after the max pooling and using another max pooling after that. I think it helped to eliminate some unuseful details from the data. This improoved the accuracy from 0.95 to 0.96, the maximum I've got.

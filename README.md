# Synthesize English text using Harry Potter book and RNN
In here I haved trained a RNN to synthesize English text character by character. I have trained a vanilla RNN with outputs, using the text from the book The Goblet of Fire "goblet_book.txt" which is retrievable [Accessed last: 2020-12-02] from here: https://kth.instructure.com/courses/5546/files/906616/download?download_frd=1

I have used the optimization AdaGrad as variation of SGD and the code contains the following elements: 
- <b>Preparing Data</b>: Read in the training data, determine the number of unique characters in the text and set up mapping functions - one mapping per each character to a unique index and another mapping each index to a character.
- <b>Back-propagation</b>: The forward and the backward pass of the backpropagation algorithm for a vanilla RNN to efficiently compute the gradients.
- <b>AdaGrad</b> updating my RNN's parameters.
- <b>Synthesizing</b> text from my RNN: Given a learnt set of parameters for the RNN, a default initial hidden state h0 and an initial input vector, x0, from which to bootstrap from then I have written a function that generates a sequence of text.

# Result

![](https://github.com/alexanderbea/Synthesize-English-text-using-Harry-Potter-book-and-RNN/blob/main/Images/Figure%201.PNG)

# TV Script Generation (Project 3)

In project 3, I generated Simpsons TV scripts by building a Recurrent Neural Network. The network uses a Word2Vec embedding model, in which words are encoded as sequential integers that are used as indices into the corresponding embedding. These are passed into a single hidden layer of ~200 LSTM cells which keep track of the ~30 words it has seen prior. The LSTM output is fed to a fully connected layer which predicts the next word. The network encodes the loss from what the original script had as its next word. By tuning the hyperparameters, the network was able to get a very small loss after a hundred epochs, and it managed to generate very nice Simpsonisms. Here's one example:

moe_szyslak: you heard 'im, fleabag. get outta my bar, you're unsanitary.
moe_szyslak: oh, how precious. the cat's sittin' in my dinner.
moe_szyslak: no, the ocean. once you get twelve miles out, there's no laws at all. that's where you all their names written street, but then when i catch you, i'm going to pull out your eyes and shove 'em up your family and friends.
moe_szyslak:(displeased chuckle) who are you, sweetheart, the health inspector?
man_at_bar: no, but i am.
moe_szyslak: uh... what am i lookin' at? i don't see nothin'. i'm gonna stop looking soon... what... what? what? what are you, the person that called nasa yesterday?
homer_simpson:(with crowd) impeach churchill!

Not only did the network pick up on appropriate grammar rules, but it also picked vocabulary that sounds quite plausible to be a line from one of the Simpsons characters. It's fun to see what it produces

I found this project to be very straightforward from the examples shown in the lessons. The only tricky part was generating the mini batches. Finding the right numpy operations that could generate the appropriate data shape was tough, but I finally got the right ideas after lurking in the forums. Also, as in project 2, the fully connected layer benefited from having a small standard deviation of 0.1, which improved the training loss substantially. 

It's all in the hyperparameters; it's all in the hyperparameters...

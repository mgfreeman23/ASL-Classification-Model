# ASL-Classification-Model
Mid-semester project associated with USC Center for AI for Society Club

Malina Freeman

mgfreema@usc.edu

Note: I completed this project in addition to the other, so this README won't follow the same extensive outline of the other project.

##### Intro
This project aims to build on the ResNet model for image classification to apply it to the task of classifying images of American Sign Language letters (as well as a few symbols including space, delete, and nothing). This included 29 different classes and a dataset from Kaggle found at {https://www.kaggle.com/dsv/29550}.

##### Process and Performance
I spent a lot of time getting the dataset into a usable format. Initially, it contained around 90,000 files. This was not feasible for me to use with Google Drive on my PC, so I trimmed the data extensively but kept enough images such that the model would still have a significant training set. Using a version of ResNet, I fine-tuned this neural network to work for my specific task. The training process took over half an hour each time. Perhaps this could be adjusted by experimenting with different epochs, batch sizes, or variations of ResNet. Ultimately, the model performed very well on both validation and testing data. The testing data accuracy was 100% with an F1-score of 1.000, although there are some caveats to these.

##### Next Steps
The model performs shockingly well because there is only one image for each class in the test set: a grand total of 29 images. Next steps would be to expand the test set and find more real-world images so that I could get better performance metrics. I also think the training data itself should be expanded. The vast majority of symbols are made in front of what seems to be a whiteboard (very plain background) with a lighter skin-toned hand. It would be better representation to have a wide range of skin tones making the symbols, so the classification will work for all skin tones and not just lighter ones. Also, it would be useful to include symbols being made in front of more distracting backgrounds. This would train the model to focus on the important part of the image and not get distracted by the background; therefore, it would work better in real-world applications.

#### Applications
A model like this could promote broader communication with the ASL community. People could potentially use an app to translate ASL users' signs into understandable words in real time. This could help decrease the communicate barrier between verbal language speakers and visual signers. Technology like this could also likely be implemented into ASL classrooms to enhance students' learning experiences. 



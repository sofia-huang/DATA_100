## Data Science Reflection 3
### Applications in Astronomy

Astronomy deals with an astronomical amount of data and data science has drastically improved astronomers’ ability to study the universe. There has been a shift in the way that data has been collected and now the skies are accessible to everyone. Data collection used to be very individual as each scientist had to collect their own data on whatever they were interested in. But now, organizations have been created, such as the Sloan Digital Sky Survey (SDSS), that image and map “larger portions of the skies and wider ranges of wavelengths of light; collecting data on more events, objects, and touching more corners of the sky through larger telescopes and better light detectors.” This data is free to the public so that anyone can study and learn from them. By providing data to the world, researchers can spend more time analyzing rather than collecting data. 

The increase in data available is an opportunity to use data science methods, like machine learning, to filter and find meaningful connections within the data. By being able to observe the sky at consistent intervals and different wavelengths, researchers are able to discover any abnormalities and create “a more comprehensive image of our skies.” However, having more data leads to more problems. Some telescopes capture up to 30 terabytes of data in a night (a large portion of it being noisy or meaningless). Being able to build an infrastructure to store these massive amounts of data is difficult and expensive.

One famous enigma of astronomy is dark energy. This is the mysterious force that is causing the universe to expand at an increasing rate rather than slowing down. One way that astronomers try to understand dark energy is through supernovas. These are powerful stellar explosions. In order to sift through telescope images of the sky in an efficient way, aka not by hand, is using machine learning. 

Dessa created a project called space2vec that automated the image analysis process by using an algorithm called Autoscan, a random forest model<sup>1</sup> . By using this model, “researchers were able to reduce the number of images astronomers had to look at by a factor of 13.4.” To put this in perspective, if astronomers had to classify 1 million images, using Autoscan would save over 16 working days. 

Taking this to the next step, Dessa decided to try applying a deep learning technique to limit the amount of time researchers needed to spend feature engineering<sup>2</sup>. Using CNNs (see last reflection for explanation) allows the feature engineering process to be completely skipped as the image data is fed to the algorithm and it learns the features itself. They put a threshold on the algorithm of 0.06 which basically forces the model to come to a decision. This resulted in a false discovery rate of only 12%. The final CNN algorithm set a new world standard and beat all previous random forest models. It saves 20 days of work not even including the time and astronomers needed for feature engineering. 

In conclusion, machine learning in astronomy is a relatively new concept and there hasn't been much research looking into it. However, there is so much potential since there is such a vast amount of data that needs to be sifted through and analyzed to be able to be studied. Hopefully in the coming years, machine learning and AI will be incorporated more into this field and there will be some cool, new discoveries.

 <sup>1</sup>A supervised learning algorithm that combines multiple decision trees, from randomly selected features instead of the best possible ones, to create the final model.

 <sup>2</sup>The process of transforming raw data into features that better represents the underlying structure of the data and improves the model performance. (Requires aid from experts to know what parts will help solve problem)
 
----------
### Works Cited

Alonso, Anna. “The State of Data in Astronomy.” Dataiku Blog. Dataiku, December 3, 2018. https://blog.dataiku.com/the-state-of-data-in-astronomy. 

Dessa. “How 3 Engineers Built a Record-Breaking Supernova Identification System with Deep Learning.” Medium. Dessa News, September 14, 2020. https://medium.com/dessa-news/space-2-vec-fd900f5566. 

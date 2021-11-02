
# Neurosity-Crown-Anxiety-Panic-Biomarker
A predictor that outputs an anxiety/panic score using data from the Neurosity Crown

## What is this?
The Neurosity Crown is an affordbale, high grade EEG device with open APIs. See: https://neurosity.co/

I suffer from Agoraphobia with Panic Disorder. This means that I experience a Panic Attack when in situations where I feel trapped, I'm too far away from home, as a passenger in a car, and other situations. 

Read more here: https://www.mayoclinic.org/diseases-conditions/agoraphobia/symptoms-causes/syc-20355987

I would like to come up with a perdictor for anxiety/panic. Note that these may be two different distinct biomarkers, I'm not too sure, yet.

## What existing research is available?

I've found this so far, **_In-vivo_  EEG Changes During A Panic Attack in a Patient With Specific Phobia** https://www.journalmc.org/index.php/JMC/article/view/532/266

https://www.researchgate.net/profile/James-Reilly-20/publication/221757678_Using_pre-treatment_electroencephalography_data_to_predict_response_to_transcranial_magnetic_stimulation_therapy_for_major_depression/links/5a16df534585155c26a762d2/Using-pre-treatment-electroencephalography-data-to-predict-response-to-transcranial-magnetic-stimulation-therapy-for-major-depression.pdf

https://arxiv.org/ftp/arxiv/papers/2010/2010.11667.pdf

https://towardsdatascience.com/using-machine-learning-to-categorise-eeg-signals-from-the-brain-to-words-728aba93b2b3

https://towardsdatascience.com/using-brain-computer-interfaces-eeg-signals-to-classify-emotions-ca3e81096a5b

I'm early on and I'm still doing research.

It seems as if the existing biomarkers for Focus and Calm are based on Gamma and Alpha readings currently, with rumors of scoring being taliored per invididual.

## How could this be accomplished?

I was thinking about end user reporting, likely a anxiety scale of 1-10 that a user can press buttons to timestamp that would be stored along with the time series data from the Crown headset. Such can be fed into an ML model to train a perdictor.

I've also been looking at the Oura Ring 3 and their readiness, sleep and other scoring (they have an API available). An important metric may be heart rate variability for general stress, and of course, heart rate.

It could be, ideal, eventually to have sensor fusion to take in other biomarkers, such as Apple Watch data, realtime blood gloucose monitoring, and other TBD datasources to enhance the model.

## What is the ultimate goal?

I personally would love to build some sort of application that could provide realtime coaching and feedback as people recover from anxiety disorders, especially agoraphobia. Personally, I'm likely going to end up using this project to learn fullstack NodeJS and dive into biohacking and to have something to do as I do my own exposure therapy. I beat agoraphobia once by building my own self driving car and getting 10,000 miles in, having that project to get outside and do something is always good.

A first application may be something as simple as logging EEG data along with GPS data and other metrics while driving to see if I can quantify anxiety/panic programmatically.

Maybe an app can be written to notify the user when to do breathing exercises, use coping skills when anxiety is detected so the user can take a moment to calm down before getting to a panic stage. People who suffer are usually too caught up in the moment to remember to do relaxation techniques.

I think something like this could also be useful in a therapy setting, therapists can gauge real world metrics as to how therapy is working, what specific things work, and what doesn't. Often, progress can be slow enough for the user not to realize they are getting better, or worse, and having some factual feedback can be encouraging over time, like a gamification of exposure therapy, healing.

## Next steps

I'm going to purchase a Crown device and start hacking. I'm also going to have to think about how to ground truth and either train a model, or write a detector somehow.

This would look like shoving a bunch of bio data into ML and doing feature importance to see which sort of data is useful, then refining from there. See https://cloud.google.com/automl-tables/docs/explain

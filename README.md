Team code repository for image caption task
-------

# Setting up the data path
  
Use link to point to the data directory

    ln -s [the-path-to-data] data
    
Now the relative path of training, validation, testing data (with annotations) should be like:

    data/ai_challenger_caption_train_20170902/caption_train_images_20170902/*.jpg
    data/ai_challenger_caption_train_20170902/caption_train_annotations_20170902.json

    data/ai_challenger_caption_validation_20170910/caption_validation_images_20170910/*.jpg
    data/ai_challenger_caption_validation_20170910/caption_validation_annotations_20170910.json

    data/ai_challenger_caption_test1_20170923/caption_test1_images_20170923/*.jpg

# Generate the tfrecord files

If there are no `TFRecord_data` in directory `data`, it is likely the the tfrecord files are not 
generated yet, run the script (after setting up the data path):

    bash scripts/build_tfrecords.sh

to create the tfrecord files. It may take 20-30 minutes to create all the files.

# Training 

# Validating

# Testing

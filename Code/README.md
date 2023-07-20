# Steps to Implement the Lip_Sync_Using_Wav2Lip Notebook

## Setup Wav2Lip 
Installing the dependencies and download the pretrained models. To do this run the first cell of the notebook.

## Select Video (Upload from local drive or Gdrive)
The second cell of the notebook will allow you to select a video from your local drive or from your google drive. The video will be uploaded to the colab environment and will be stored in the `sample_data` folder.

## Select Audio (Record, Upload from local drive or Gdrive)
The third cell of the notebook will allow you to record audio from your microphone, select an audio file from your local drive or from your google drive. Make sure the audio you upload is in '.wav' format. The audio will be uploaded to the colab environment and will be stored in the `sample_data` folder.

## Start Lip Syncing and Preview the Result
The fourth cell of the notebook will start the lip syncing process. To get the optimum result I used `top pad=10`, `bottom pad=0'`, `left pad=10`, `right pad=0`, `resize_factor=2` and `nosmooth=True`. It should take 1-2 minutes to generate the results. The result will be stored in the `Wav2Lip/results` folder.

 ##### Tips for better results:
- Experiment with the `--pads` argument to adjust the detected face bounding box. Often leads to improved results. You might need to increase the bottom padding to include the chin region. E.g. `--pads 0 20 0 0`.
- If you see the mouth position dislocated or some weird artifacts such as two mouths, then it can be because of over-smoothing the face detections. Use the `--nosmooth` argument and give it another try. 
- Experiment with the `--resize_factor` argument, to get a lower-resolution video. Why? The models are trained on faces that were at a lower resolution. You might get better, visually pleasing results for 720p videos than for 1080p videos (in many cases, the latter works well too). 
- The Wav2Lip model without GAN usually needs more experimenting with the above two to get the most ideal results, and sometimes, can give you a better result as well.

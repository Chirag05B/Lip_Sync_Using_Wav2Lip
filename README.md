# Lip_Sync_Using_Wav2Lip
 
In this project i have used the Wav2Lip model to lip sync a video with an audio. 
I then evaluated the performance of the model using the LSE-D and LSE-C metrics. The LSE-D metric is used to evaluate the lip sync performance of the model when the audio and video are from the same speaker. The LSE-C metric is used to evaluate the lip sync performance of the model when the audio and video are from different speakers. The LSE-D and LSE-C scores are calculated using the SyncNet model.

Prerequisites
-------------
- `Python 3.6` 
- ffmpeg: `sudo apt-get install ffmpeg`
- Install necessary packages using `pip install -r requirements.txt`
- Face detection [pre-trained model](https://www.adrianbulat.com/downloads/python-fan/s3fd-619a316812.pth) should be downloaded to `face_detection/detection/sfd/s3fd.pth`. Alternative [link](https://iiitaphyd-my.sharepoint.com/:u:/g/personal/prajwal_k_research_iiit_ac_in/EZsy6qWuivtDnANIG73iHjIBjMSoojcIV0NULXV-yiuiIg?e=qTasa8) if the above does not work.

## Quick Guide
1. Create video file named `input_video.mp4`. Please check `Inputs/` folder for the input video I used.
2. Create audio file named `input_audio.wav`. Please check `Inputs/` folder for the input audio I used.
3. Both file have to be of similar length.
4. Target face in the input_video.mp4 must be "detectable" in all video frames.
5. Make sure you use correct file extension (.mp4 and .wav)
6. Wav2Lip does not like very long and high resolution videos. Try to keep the video length under 30 seconds(max 60 seconds) and resolution under 720p(max 1080p).
7. The code and evaluation code should be run on defferent environments as there can be a version mis-match issue.

Code
----------
Please check the `Code/` folder for the instructions.


Evaluation
----------
Please check the `evaluation/` folder for the instructions.
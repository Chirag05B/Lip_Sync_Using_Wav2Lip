# Lip_Sync_Using_Wav2Lip
 
Prerequisites
-------------
- `Python 3.6` 
- ffmpeg: `sudo apt-get install ffmpeg`
- Install necessary packages using `pip install -r requirements.txt`. Alternatively, instructions for using a docker image is provided [here](https://gist.github.com/xenogenesi/e62d3d13dadbc164124c830e9c453668). Have a look at [this comment](https://github.com/Rudrabha/Wav2Lip/issues/131#issuecomment-725478562) and comment on [the gist](https://gist.github.com/xenogenesi/e62d3d13dadbc164124c830e9c453668) if you encounter any issues. 
- Face detection [pre-trained model](https://www.adrianbulat.com/downloads/python-fan/s3fd-619a316812.pth) should be downloaded to `face_detection/detection/sfd/s3fd.pth`. Alternative [link](https://iiitaphyd-my.sharepoint.com/:u:/g/personal/prajwal_k_research_iiit_ac_in/EZsy6qWuivtDnANIG73iHjIBjMSoojcIV0NULXV-yiuiIg?e=qTasa8) if the above does not work.

## Quick Guide
1. Create video file named input_video.mp4
2. Create audio file named input_audio.wav
3. Both file have to be of similar length
4. Target face in the input_video.mp4 must be "detectable" in all video frames
5. Make sure you use correct file extension (.mp4 and .wav)
6. Wav2Lip does not like very long and high resolution videos. Try to keep the video length under 30 seconds(max 60 seconds) and resolution under 720p(max 1080p).

Code
----------
Please check the `Code/` folder for the instructions.


Evaluation
----------
Please check the `evaluation/` folder for the instructions.
# COGNIMUSE-HDF5
Build COGNIMUSE HDF5 file for video summarization.

The COGNIMUSE HDF5 file contains seven groups, one for each 30 minute video. Each group contains seven keys: n_frames, features, the frame rate
of each video (frames per second (fps)), change_points, n_steps, picks, and the ground truth summary of each video, gt_summary. We first downsampled the
movie segments to 2 fps, from 25 fps, using FFmpeg and to extract the representation of the frame features, we first convert each video to video frames, we extract its features and its change points, and we create the HDF5 file with the ground truth summary, as well as the rest of the keys.

## Main dependencies

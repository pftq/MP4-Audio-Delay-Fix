# MP4-Audio-Delay-Fix
Fixes the ~20ms audio delay in MP4s exported by Adobe and other software due to missing metadata.  Doesn't re-encode the MP4, simply adds some metadata to the existing file.

Download here: https://github.com/pftq/MP4-Audio-Delay-Fix/releases/tag/20261103

You may also find these useful:
- Video Debanding (fixes quality issues with repeat re-processing/compression) https://github.com/pftq/Video-Debanding
- Video Compare (to check export errors, differences, etc) https://github.com/pftq/Video-Compare
- Video Frame Sync (syncing 2 files that drift out of sync) https://github.com/pftq/Video-Frame-Sync
- Video Color Match (correcting color grading drift) https://github.com/pftq/VideoColorMatch

The issue has long been documented for Adobe in particular but never fixed.  The problem appears to be that the AAC audio spec requires metadata to indicate where the audio actually starts, but Adobe doesn't supply it.  This tool simply adds it in.
- https://community.adobe.com/questions-729/audio-out-of-sync-when-exporting-h-264-1421574
- https://community.adobe.com/questions-729/20-milliseconds-delay-1402050

<img width="607" height="470" alt="image" src="https://github.com/user-attachments/assets/7cffee25-2fc6-42bd-a8d7-3c478d8608df" />

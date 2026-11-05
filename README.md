# MP4-Audio-Delay-Fix
Fixes the ~20ms audio delay in MP4s exported by Adobe and other software due to missing metadata.  Doesn't re-encode the MP4, simply adds some metadata to the existing file.

Download here: https://github.com/pftq/MP4-Audio-Delay-Fix/releases/tag/20261103<br>
You may also find these useful (one-click to download all [here](https://drive.google.com/drive/folders/1nvQFC5uwsZlf-82LuskCP-qut9xHw-lt?usp=sharing)):\
• [Video Debanding](https://github.com/pftq/Video-Debanding) (fixes quality issues with repeat re-processing/compression)\
• [Video Compare](https://github.com/pftq/Video-Compare) (to check export errors, differences, etc)\
• [Video Frame Sync](https://github.com/pftq/Video-Frame-Sync) (syncing 2 files that drift out of sync)\
• [Video Color Match](https://github.com/pftq/VideoColorMatch) (correcting color grading drift)\
• [Screencaps Generator](https://github.com/pftq/Screencaps-Generator) (smart screencaps selection + gallery grid sheet)

The issue has long been documented for Adobe in particular but never fixed.  The problem appears to be that the AAC audio spec requires metadata to indicate where the audio actually starts, but Adobe doesn't supply it.  This tool simply adds it in.
- https://community.adobe.com/questions-729/audio-out-of-sync-when-exporting-h-264-1421574
- https://community.adobe.com/questions-729/20-milliseconds-delay-1402050

<img width="607" height="470" alt="image" src="https://github.com/user-attachments/assets/7cffee25-2fc6-42bd-a8d7-3c478d8608df" />

Credits:
- Python, application runtime
- Tcl/Tk, user interface
- PyAV / FFmpeg, media inspection and audio decoding
- PyInstaller, Windows executable packaging

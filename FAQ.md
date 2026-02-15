# FAQ - Frequently Asked Questions

[简体中文](./FAQ_CN.md) | **English**

## 🏠 General / 基础问题

**Q: Is it free?

A: No. It's cheaper than lunch.?**  


**Q: Do I need to install Python or FFmpeg?**  
A: No Python needed (standalone exe). **FFmpeg required** - download from https://github.com/BtbN/FFmpeg-Builds/releases.


**Q: Windows versions supported?**  
A: 64-bit Windows 10-WIN 11 . Not tested on Win8.1.

## 🔧 Technical / 技术问题

**Q: What is "mux/stream copy" (-c copy)? Why no re-encoding?**  

A: **Mux = combine audio/video/subtitle tracks into one file without quality loss or slowdown**. `-c copy` copies raw streams (like copying files). **Limitations**:  
- Only works if formats match (e.g., MP4 audio must be AAC).  
- Won't fix sync issues, cut clips, or convert formats.  
- Use "Re-encode" mode for incompatible files (slower, possible quality loss).

The software's parameter copying feature operates at lightning speed without compromising audio or video quality. However, this efficiency inherently limits its rapid splitting function from achieving perfect keyframe alignment. Achieving flawless splits requires re-encoding.



**Q: Error: "Could not find FFmpeg"**  

A: extract FFMPEG, Click on "Browse" to navigate to the FF directory you have extracted, locate bin\ffmpeg.exe, and simply click to open it.
![Main Interface](./screenshots/FddsF-2.jpg)


**Q: MKV output larger than input?**  

A: MKV containers add metadata overhead, but MKV offers the best compatibility.


**Q: Subtitle not showing?**  

A: Select SRT/ASS as subtitle track. MKV supports external subs; MP4 needs burn-in (re-encode).BTW,The graphic subtitles for Blu-ray (PGS) cannot be included in files with MP4 format. The copy function of this tool cannot make it a valid SRT file for the text.


**Q: What's the difference between "soft subtitles" and "burned-in subtitles"? Why doesn't your software offer burning?**

A: Soft subtitles attach the subtitle file to the video file. Burning subtitles renders them directly into the video frame (hard-coded subtitles).
Burning requires re-encoding the video, which conflicts with the "fast + lossless" goal of the -c copy option.


**Q: Why does adding SRT to MP4 fail?**

A: SRT (SubRip) is not an officially supported subtitle format for MP4. It typically needs conversion to mov_text to function as a subtitle track within MP4.


**Q: Why does Windows/antivirus flag the exe as malicious?**

A: Numerous users have reported in Python's official issues that onefile/new versions are falsely detected by VirusTotal/Defender. This tool does not upload files and operates offline. I am currently submitting reports on these antivirus false positives.

## 💰 License / 授权

**Q: How to activate after purchase?**  

A: Open the software's "About" section to view the serial number.


**Q: Refund policy?**  

A: 7-day money-back if not working on your PC.


## ⚔️ Comparison / 与其他工具对比

**Q: Why not free like MKVToolNix?**  

A: MKVToolNix = CLI/GUI for pros. **This tool: drag-drop simple, This little tool is extremely simple to operate and the fastest. Windows-optimized**. Saves hours vs command line.


**Q: Better than Shutter Encoder?**  

A: Yes for pure mux (faster, no extra features bloat). Shutter good for convert; this for lossless mux.


**Q: Is there a trial version available?**  

A: trial version software is currently being prepared.10 successful exports. Each file must not exceed 1GB (1024MB).

## 📧 Need Help?
Email: your-email@example.com |
[Changelog](./CHANGELOG.md)

---
Last updated: 2026-02-13

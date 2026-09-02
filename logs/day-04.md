# Day 04: Sept 02, 2026 — HTML Audio & Video Elements

### 📝 Today's Progress
Completed the theory module on **Working with Audio and Video Elements**. Learned how native HTML tags handle media playback without external plugins.

### 💡 Key Takeaways

**1. `<audio>` Element**  
Embeds sound files. Adding `controls` provides play/pause buttons, and `<source>` specifies the file path and format:

```html
<audio controls>
  <source src="audio.mp3" type="audio/mpeg" />
  Your browser does not support the audio element.
</audio>

# EP Release Template

A modern, responsive web template for music EP/album releases featuring a liquid metal aesthetic, password-protected tracks, and video integration.

## Features

- 🎥 Animated background with customizable video
- 🔒 Password-protected track access
- 📱 Fully responsive design
- ✨ Modern UI with metallic effects and animations
- 🎵 Featured video section
- 📋 Track list with video links
- 🌐 YouTube video integration

## Quick Start

1. Clone or download this template
2. Replace `bg-vid.mov` with your background video
3. Open `EP.release.html` in a text editor
4. Customize the following elements:
   - Replace `[Artist Name]` with your artist name
   - Update video IDs and track titles
   - Change the password (default is 'love')

## Customization Guide

### Background Video

The template uses a background video with 10% opacity. To change the video:
```html
<video class="background-video" autoplay loop muted playsinline>
    <source src="bg-vid.mov" type="video/mp4">
    Your browser does not support the video tag.
</video>
```
- Replace `bg-vid.mov` with your video file
- Supported formats: MP4, WebM, Ogg
- Recommended: Short loop (15-30 seconds) for better performance

### Featured Video

Update the featured video section:
```html
<div class="featured-video">
    <h2>Featured Video: Song Title One</h2>
    <iframe src="https://www.youtube.com/embed/VIDEO_ID" allowfullscreen></iframe>
</div>
```
- Replace `VIDEO_ID` with your YouTube video ID
- Update the title to match your featured track

### Track List

Customize the track list section:
```html
<div class="track">
    <h3>1. Song Title One</h3>
    <a href="https://www.youtube.com/watch?v=VIDEO_ID" class="video-link" target="_blank">Watch Music Video</a>
</div>
```
For each track:
1. Update the track number and title
2. Replace `VIDEO_ID` with the corresponding YouTube video ID
3. Add or remove tracks as needed

### Password Protection

The default password is 'love'. To change it, modify the JavaScript section:
```javascript
function unlockContent() {
    const password = document.getElementById('password').value;
    if (password === 'love') { // Change 'love' to your desired password
        document.querySelectorAll('.locked').forEach(track => {
            track.classList.remove('locked');
        });
    }
}
```

### Styling

The template uses a dark theme with metallic accents. Main colors:
- Background: `#0a0a0a` (dark)
- Text: `#d4d4d4` (light)
- Accent: `#9696ff` (metallic blue-purple)

To modify the styling, edit the CSS variables in the `<style>` section.

## Browser Compatibility

- Chrome (recommended)
- Firefox
- Safari
- Edge
- Opera

## Mobile Support

The template is fully responsive and includes:
- Viewport meta tag for proper scaling
- Mobile-friendly video playback
- Responsive grid layout
- Touch-friendly interface

## Performance Tips

1. Optimize your background video:
   - Compress to reduce file size
   - Keep duration short (15-30 seconds)
   - Consider resolution vs. file size
2. Use optimized images for thumbnails
3. Minimize the number of embedded videos

## License

This template is free to use for both personal and commercial projects. Attribution is appreciated but not required.

## Support

For questions or customization help:
1. Check the HTML comments for guidance
2. Review the CSS classes for styling options
3. Consult YouTube's embedding documentation for video integration

---

Made with ❤️ for musicians and creators 
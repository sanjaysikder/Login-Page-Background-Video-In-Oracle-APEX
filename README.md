# Oracle APEX Login Page Background Video

This guide will show you how to add a background video to the login page in an Oracle APEX application. By following these steps, you can make your login page more dynamic with a custom video background.

## Steps

### 1. Login Page Configuration
Make sure you are using a custom login page. If you're using the default login page, switch to a custom page.

### 2. Add the Video to Your Page
You can either host the video on your server or use an external video hosting service like YouTube or Vimeo. For this guide, we assume the video file is hosted somewhere or uploaded to APEX static files.

### 3. Add the HTML and CSS to Your Login Page
- Go to your **Login Page** (or create a new page) in APEX.
- Edit the page attributes and navigate to the **"Custom CSS"** section to add the required styles.

### 4. Customizing the Background Video with HTML
- Open **Page Designer** and go to the **"HTML Header"** section under your login page.
- Insert the following HTML code in the HTML Header section:

```html
<div class="background-video-container">
  <video autoplay muted loop id="background-video">
    <source src="https://www.example.com/path/to/your/video.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
</div>
```

### 5. Add the Required CSS

- Add below css code on Page Inline (Page > Inline):

```css code

.background-video-container {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: -1;
    overflow: hidden;
}

#background-video {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

```


## Thank You
## Sanjay Sikder

You can connect with me on [LinkedIn](https://www.linkedin.com/in/sanjay-sikder/)!


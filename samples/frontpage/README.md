# Frontpage - Using FSI TouchZoom & Single Source Imaging

This readme describes how the front page example is achieved using _FSI TouchZoom_ and _Single Source Imaging_ from _FSI Server_.

# Using TouchZoom

To display all images with TouchZoom, you only need to add the following script
to the head of your website:

```html
<script
  src='https://docs.neptunelabs.com/fsi/viewer/applications/touchzoom/js/fsitouchzoom.js'
</script>
```

In our example, this is done through the framework, but you can see that the script is loaded when the page is compiled.

This ensures that FSI TouchZoom is loaded and all images are displayed at the correct resolution for the current zoom level.
This ensures sharp images on mobile devices.
You can also see this when you resize your browser window or switch between different displays.

You can also set different parameters by using an `<fsi-touchzoom>` tag, which is what we have done here:

```html
<fsi-touchzoom style="display:none" useDevicePixelRatio="true" debug="true"></fsi-touchzoom>
```

## Testing with examples from your own server

To test the examples with images from your own [FSI Server](https://www.neptunelabs.com/fsi-server/), please first copy the env.yml.dist file to env.yml and adapt the file, then restart the main demo again.

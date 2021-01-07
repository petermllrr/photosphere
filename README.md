# Photosphere Web Viewer

Example implementation of Damien Sorel's [Photo Sphere
Viewer](https://photo-sphere-viewer.js.org/). See a live example at
[photosphere.petermueller.io](https://photosphere.petermueller.io).

To embed a 360 degree image, first link the required libraries in the header of
your html document:

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/photo-sphere-viewer@4/dist/photo-sphere-viewer.min.css" />
<script src="https://cdn.jsdelivr.net/npm/three/build/three.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/uevent@2/browser.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/photo-sphere-viewer@4/dist/photo-sphere-viewer.min.js"></script>
```

Next, add this JavaScript snippet. The `container` is the element in which the
image will be rendered, the `panorama` is the image.

```html
<script>
    var viewer = new PhotoSphereViewer.Viewer({
        container: document.querySelector('#viewer'),
        panorama: 'img/PXL_20201209_153211859.PHOTOSPHERE.jpg'
    });
</script>
```

The the
[index.html](https://github.com/petermllrr/photosphere/blob/main/index.html)
file for an example.

Full documentation at
[photo-sphere-viewer.js.org](https://photo-sphere-viewer.js.org/).
# Photosphere Web Viewer

Example implementation of Damien Sorel's [Photo Sphere
Viewer](https://photo-sphere-viewer.js.org/). See a live example at
[photosphere.petermueller.io](https://photosphere.petermueller.io).

1. To embed a 360 degree image to your website, add the required dependencies to
the `<head>` of your html file:

    ```html
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/photo-sphere-viewer@4/dist/photo-sphere-viewer.min.css" />
    <script src="https://cdn.jsdelivr.net/npm/three/build/three.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/uevent@2/browser.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/photo-sphere-viewer@4/dist/photo-sphere-viewer.min.js"></script>
    ```

2. Create a `div` container in which the image will be rendered. Give it a
unique id (for example `"viewer"`) and a defined size.

    ```html
    <div id="viewer"></div>
    ```

3. After this `<div>` element, add the following JavaScript code:

    ```html
    <script>
        var viewer = new PhotoSphereViewer.Viewer({
            container: document.querySelector('#viewer'),
            panorama: 'img/PXL_20201209_153211859.PHOTOSPHERE.jpg'
        });
    </script>
    ```
    `container`: ID of the container element created earlier.  
    `panorama`: relative url to the panorama image.

See the
[index.html](https://github.com/petermllrr/photosphere/blob/main/index.html)
file for an example.

Full documentation at
[photo-sphere-viewer.js.org](https://photo-sphere-viewer.js.org/).
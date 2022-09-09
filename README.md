# IIIF Images

Collection of static level 0 images

## How to add an image?

### Scenario 1: images are 'locked' in an institutional zoom viewer

#### Step 1: Get high-res image
- Install [Dezoomify](https://dezoomify.ophir.dev/) Firefox extension
- Navigate to the item's landing page
- Open the viewer
- Activate the add-on
- Click 'Dezoomify!'
- Save image locally after download has completed
- Convert png to jpg without compression
  - ImageMagick command: `convert -quality 100 filename.png filename.jpg`

#### Step 2: Create IIIF derrivative
- [IIIF Tiler](https://github.com/glenrobson/iiif-tiler)
- Change info.json `@id`
  - Path: `https://theberlage.github.io/iiif-images/[subfolder]\[image-folder]` 

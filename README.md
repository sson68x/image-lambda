# LAB 17

## Project: AWS: S3 and Lambda

### Author: Simon Son

### Problem Domain

* Create an S3 Bucket with “open” read permissions, so that anyone can see the images/files in their browser
* A user should be able to upload an image at any size, and update a dictionary of all images that have been uploaded so far
* When an image is uploaded to your S3 bucket, it should trigger a Lambda function which must:
  * Download a file called “images.json” from the S3 Bucket if it exists
  * The images.json should be an array of objects, each representing an image. Create an empty array if this file is not present
  * Create a metadata object describing the image
    * Name, Size, Type, etc.
* Append the data for this image to the array
* Upload the images.json file back to the S3 bucket

### Links and Resources

* [GitHub](https://github.com/sson68x/image-lambda/pull/2)
* [AWS S3](https://lab17-upload-image.s3.us-west-2.amazonaws.com/images.json)
* [Class Demo](https://github.com/codefellows/seattle-javascript-401d47/tree/main/class-17)

### Setup

#### `.env` requirements (where applicable)

* N/A

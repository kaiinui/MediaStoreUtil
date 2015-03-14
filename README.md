# MediaStoreUtil

An Android MediaStore (Images &amp; Videos) manipulation utility aimed at easier use especially for iOS developers.

```java
// A data class that represents Images

class Image {...}

// Retrieve all images.

final List<Image> medias = MediaStoreUtil.getAllImages(context);

// Get an image from a cursor.

final Image image = MediaStoreUtil.imageFromCursor(cursor);

// Get the bitmap of an image.

final Bitmap bitmap = image.getBitmap();

// Get URI representation of an image.

final Uri uri = image.getUri();

// Show an image using Picasso library.

Picasso.with(this).load(image.getUri()).into(imageView);
```

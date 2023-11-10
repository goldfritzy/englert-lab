# Image Types

Increasing the efficiency of loading times on the website is crucial in maintaining user engagement and ease of use. Therefore, one of the easiest ways to reduce loading times on each individual webpage is to favour more efficient file types, chiefly among them, the WebP image standard.



According to the Google, the creators and maintainers of the WebP image standard:

WebP is a modern **image format** that provides superior **lossless and lossy** compression for images on the web. Using WebP, webmasters and web developers can create smaller, richer images that make the web faster.

WebP lossless images are [26% smaller](https://developers.google.com/speed/webp/docs/webp\_lossless\_alpha\_study#results) in size compared to PNGs. WebP lossy images are [25-34% smaller](https://developers.google.com/speed/webp/docs/webp\_study) than comparable JPEG images at equivalent [SSIM](https://en.wikipedia.org/wiki/Structural\_similarity) quality index.

Lossless WebP **supports transparency** (also known as alpha channel) at a cost of just [22% additional bytes](https://developers.google.com/speed/webp/docs/webp\_lossless\_alpha\_study#results). For cases when lossy RGB compression is acceptable, **lossy WebP also supports transparency**, typically providing 3× smaller file sizes compared to PNG.

Lossy, lossless and transparency are all supported in **animated WebP images**, which can provide reduced sizes compared to GIF and APNG.



## Creating WebP images

Convert your favorite collection from PNG and JPEG to WebP by downloading the precompiled `cwebp` conversion tool for [Linux, Windows or macOS](https://developers.google.com/speed/webp/docs/precompiled).



Once cwebp is installed, all you need to do is enter the following command in a terminal:

```
cwebp [Original Image Name].jpg -q [INTEGER] -o [New Image Name].webp && rm -rf [Original Image Name].jpg
```

Breaking this command into its individual constituents:

`cwebp` calls the command and allows your command processor to accept the next string of arguments

`[Original Image Name].jpg` is the original image. Note the image type does not have to be a JPEG. The cwebp binary accepts multiple image types such as `.jpg, .jpeg, .png`, to name a few.

`-q [INTEGER]` sets the "quality" of the output image. This is because we will be using lossy compression for these images. Typically, you can safely set your quality anywhere between 60-80 without any noticeable difference. When I was creating this website, I used 80 as my integer value.&#x20;

{% hint style="info" %}
Remember, the lower the quality (and therefore the more lossy compression), the lower the overall file size will be! Lower file sizes = faster load times!

The point of optimisation is all about finding a balance between quality and speed, so feel free to play around with varying integer quality types to find what works best for each image.
{% endhint %}

`-o [New Image Name].webp` will be the output of the new webp file. Typically, I keep the file names the same (for example, if I were to convert Dr. Englert's headshot from a jpeg to a webp, I would keep the image name `jenglert` the same).

`&& rm -rf [Original Image Name].jpg` deletes the old file, as we don't need it anymore.



All together, here is an example that I used for converting individuals' headshots to webp. I'll start at the root directory of the website and show the entire output from the command line.



```bash
$ pwd 
/GitHub/englert-lab
$ cd images/members
$ cwebp jenglert.jpg -q 80 -o jenglert.webp && rm -rf jenglert.jpg 
Saving file 'jenglert.webp'
File:      jenglert.jpg
Dimension: 3600 x 2400
Output:    142722 bytes Y-U-V-All-PSNR 51.83 53.98 53.99   52.43 dB
           (0.13 bpp)
block count:  intra4:       6102  (18.08%)
              intra16:     27648  (81.92%)
              skipped:     12553  (37.19%)
bytes used:  header:            251  (0.2%)
             mode-partition:  36815  (25.8%)
 Residuals bytes  |segment 1|segment 2|segment 3|segment 4|  total
    macroblocks:  |       1%|       3%|       8%|      88%|   33750
      quantizer:  |      27 |      27 |      24 |      19 |
   filter level:  |       8 |      12 |      37 |      30 |
$
```

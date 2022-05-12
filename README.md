Steganography Online

Since I wanted to look into steganography for some time, this is a small project dedicated to steganography.

It provides functionality to encode a message in an image and to decode the message from the image.


The User chooses an image, the image data is then normalized, meaning that each RGB value is decremented by one if it is not even. This is done for every pixel in the image.

Next the message is converted to a binary representation, 8 Bits per character of the message. This binary representation is then applied to the normalized image, 3 Bit per pixel. This concludes, that the maximal length of a message hidden in an image is:

Since the image was normalized, we now know that an even r, g or b value is 0 and an uneven is a 1. And this is how the message is decoded back from the image.

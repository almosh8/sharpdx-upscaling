# This repository demonstrates how image upscaling works in SharpDX library.

## Example using Matrix.Scaling

```C#
var scaleWidth = 2.0F;
var scaleHeight = 2.0F;
var transformMatrix = Matrix3x2.Scaling(scaleWidth, scaleHeight);
d2dContext.Transform = transformMatrix;
```

## Results of upscaling

### Original image 600x800
![Input](https://user-images.githubusercontent.com/106275943/193568783-61c29ab1-3e35-4cd7-b4da-f55927d31cf3.png)
### Upscaled image 1200x1600
![Output](https://user-images.githubusercontent.com/106275943/193568983-f6546e93-8ad6-49c0-a7ea-6001ec943df7.png)
### What happens if you only change image size and don't apply upscaling(empty space colored grey for contrast)
![Output without upscale](https://user-images.githubusercontent.com/106275943/193571032-775e8727-4ad9-4831-905e-fa60328f6bb8.png)



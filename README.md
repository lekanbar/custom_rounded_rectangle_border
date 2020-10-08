# Custom rounded rectangle border

A simple package for drawing custom shape borders with full control on how you want the sides to be
rendered.

It simply addresses an open Flutter issue where an error is thrown when you try to set a
borderRadius and border at the same time, see open issue below:
[Support non-uniform Borders with a non-zero borderRadius](https://github.com/flutter/flutter/issues/12583)

## Sample Usage
```
Container(
    decoration: ShapeDecoration(
    shape: CustomRoundedRectangleBorder(
      borderRadius: BorderRadius.only(
          bottomLeft: 5.0,
          bottomRight: 5.0),
      leftSide: BorderSide(
          color: Colors.black),
      bottomLeftCornerSide: BorderSide(
          color: Colors.black),
      rightSide: BorderSide(
          color: Colors.black),
      bottomRightCornerSide: BorderSide(
          color: Colors.black),
      bottomSide: BorderSide(
          color: Colors.black),
    ),
),)
```

## Flutter
For help getting started with Flutter, view our 
[online documentation](https://flutter.dev/docs), which offers tutorials, 
samples, guidance on mobile development, and a full API reference.

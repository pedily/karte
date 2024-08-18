# Karte

The following text describes the goals of this project. It's not done, yet!

This web component should help when embedding map-like content onto a web page. It takes
care of panning/zooming functionality and supports "staying on target" when the element is
resized. A target can be either a point (the point in the center) or a rectangular area.
The API supports a "go to" functionality that supports both a point and an area as a
reference, both with "pixel coordinates". When a target point is set via the API, the view
will pan so that point is centered in the element. The zoom will not adjust (although
that's configurable in the API options). When a target area is set via the API, the view
will pan to the center of that area. If the area is "larger" than the element size, it
will also zoom until all content in the rect is visible. When the element gets resized and
a point or area is focused, that point or area will be refocused after the resize. Manual
interaction with mouse/touch will always override automatic pan/zoom functionality.

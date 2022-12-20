## So you want to Build a Pooly... Or some Pixel Pooly Parts
### A How-To
---

**Table of Contents**
- [TLDR](PoolyBuilder.md#tldr)
- [Layer Composition](PoolyBuilder.md#swooping-into-the-details)
- [How to Make an SVG into "Pixels"](PoolyBuilder.md#swooping-into-the-details)
- [Using the Wire Frame](PoolyBuilder.md#using-the-wire-frame)
- [What's Next](PoolyBuilder.md#whats-next)

---

#### **TLDR:**
A 320px x 320px SVG Wire Frame with examples is [here](pixel-pooly-assets/SVG/PoolyWireFrame.svg).

When compiling the NFT the Layers compile in the following order:
0. [Background](PoolyBuilder.md#0. Background)
1. [Body](PoolyBuilder.md#1. Body)
2. [Head](PoolyBuilder.md#2. Head)
3. [Lower Body](PoolyBuilder.md#3. Lower Body)
4. [Left Arm](PoolyBuilder.md#4. Left Arm)
5. [Right Arm](PoolyBuilder.md#5. Right Arm)
6. [Head Accessory](PoolyBuilder.md#6. Head Accessory)
7. [Face Accessory](PoolyBuilder.md#7. Face Accessory)
8. [Body Accessory](PoolyBuilder.md#8. Body Accessory)
9. [Lower Body Accessory](PoolyBuilder.md#9. Lower Body Accessory)
10. [Left Wing Accessory](PoolyBuilder.md#10. Left Wing Accessory)
11. [Right Wing Accessory](PoolyBuilder.md#11. Right Wing Accessory)

Pixel Pooly is currently fairly low resolution. To simulate this each Pooly pixel is actually a 10px x 10px square. This is resolution is not required, you can utilize any pixel resolution that works for you.

---
#### **Swooping into the Details**

You'll find a 320px x 320px SVG file with a Wire Frame and Pixel Pooly Examples in this repo:
[Wire Frame](pixel-pooly-assets/SVG/PoolyWireFrame.svg)
This Wire Frame includes a series of examples for some of the traits. It should also be noted that each Pooly pixel is actually 10px x 10px, so a higher resolution image can be created in this 320px x 320px framework.

#### The Layer Composition
##### 0. Background
The background just needs to a 320px x 320px square. Take heed to utilize the other parts of the Wire Frame to ensure any important parts of the background image aren't hidden behind Pooly.

##### 1. Body
In the Wire Frame this is represented by 1-BodySpace.
The body layer is usually just a rectangle at the bottom center of the frame, this is the first layer as it will have most of the other layers *attach* to it.
If a shirt or some other full torso design is being developed, it would also be designed as a Body Layer.

##### 2. Head
In the Wire Frame this is represented by 2-HeadSpace
The head layer a large trait and can come in a variety of shapes, but should fill most of the center of the frame.
The head usually has a pair of eyes, beak, and a craw.
There is one location in the beak needs to be in contact with as some traits interact with this location (bubble pipe). This space is outlined in red dashes on the Wire Frame called MouthConnector.

##### 3. Lower Body
In the Wire Frame this is represented by 3-BodyLowerSpace
This layer is utilized for feet, but like many of the layers, creativity dictates it could be utilized for a number of things.
Make a nest that Pooly is sitting in, turn Pooly into a serpent birb, give Pooly a branch to sit on, or something else.

##### 4. Left Arm
In the Wire Frame this is represented by 4-LeftWingSpace
For Pooly this is the Wing layer, but it could contain any arm-like variation. Because it can be anything arm-like the Wire Frame offers a generous space. A Pixel Pooly wing is also included as 10-LeftWingAccSpace.
How the wing attaches to the body is outlined in the red dashes to the side of the body in Wire Frame called LeftWingConnector.
Any arm-like trait should connect to the body through some segment in this LeftWingConnector

##### 5. Right Arm
In the Wire Frame this is represented by 5-RightWingSpace
All the notes for the Left Arm apply to the Right Arm. The red dashed segment for the connection point in RightWingConnector. And a Pixel Pooly wing wire frame is 11-RightWingAccSpace

##### 6. Head Accessory
In the Wire Frame this is represented by 6-HeadAccSpace
This layer is composed of hats or things that should go above the head.
**Hats** should generally cover the top segments pixels of Pooly's head. This section is outline in red dashes in the Wire Frame and called HatConnector.
It's optional to have the hat cover some or all of the craw.
As always it's semi-optional to stay within the bounds of the Wire Frame for the Head Accessory. Traits like Judges Wig or Egghead, go beyong the boundary of the Wire Frame. Creativity is king.

##### 7. Face Accessory
In the Wire Frame this is represented by 7-FaceAccSpace. This part of the wireframe will be purple with associated face parts, this is so you can plan your face accessories around the different known/common face structures.
This layer is composed of glasses/monocles, mouth parts, or things that can generally be applied to the face.
**Glasses/Monocles** could cover the eyes, or fit elsewhere (down the beak, top of head over a hat, etc.).
**Mouth Parts** need to originate from a single point on the right corner of the Pooly beak, this is outlined in red dashes in the wire frame as MouthConnector.

##### 8. Body Accessory
In the Wire Frame this is represented by 8-BodyAccSpace. This wire frame is also purple, but is effectively the same as the body.
This layer is for anything that would go over the top of a body like necklaces or a sweatshirt.
It should be noted this is another area to state that creativity is king, items like Floaties are a Body Accessory so the wings/arms could still hold something and go on either side of the body.

##### 9. Lower Body Accessory
In the Wire Frame this is represented by 9-LowerBodyAccSpace. This wire frame is the same as the Lower Body frame.
This layer has not yet had a trait built. This area could contain tiny pooly pets, branches, etc. Another instance of creativity is king.

##### 10. Left Wing Accessory
In the Wire Frame this is represented by 10-LeftWingAccSpace. This wire frame is a purple wire frame to show where the wing is.
This is usually an item being held or doing something.
It does not always need to be the wing, it could be some item next to Pooly or something else.
However, it should be noted that some of the traits can have a wing open or tucked, or we may have other arm-like traits.

##### 11. Right Wing Accessory
In the Wire Frame this is represented by 11.RightWingAccSpace. This wire frame is a purple wire frame to show where the wing is.
Notes from the Left Wing Accessory also apply here.

##### 12. Signal Layer
This layer cannot be contributed to as a trait layer. It remains transparent until there is a need for the Friends of Pooly to take action. This layer acts as a temporary signal layer so all NFTs display the same image for a period of time. This way we are all showing support together.

#### How Does an SVG become Pixels
Yes the V in SVG is for Vector, yes Pixel Pooly is blocky pixels. To do this there's a few steps to set up in your SVG editor. The first set of Pixel Pooly's were designed in Inkscape so the following explanation will utilize terminology from Inkscape.
- The SVG canvas should be 320 x 320 with the units set to pixel,
- For visual ease a grid should be turned on,
- The grid could have spacing of 10 pixels by 10 pixels, this gives the image a total of 32 "pixel" by 32 "pixel" look and feel,
- Snapping to the grid should also be turned on so each pixel is entire filled by the objects in the image and that they align correctly,
- Once the image is designed, objects of the same color in the image should be combined and converted to paths,
  - Note: combining objects will require some planning to ensure the image is layered appropriately.

#### Using the Wire Frame
The [Wire Frame](pixel-pooly-assets/SVG/PoolyWireFrame.svg) for Pixel Pooly has a lot of groups and layers in the SVG.
Some of these groups contain layers that are examples to experiment with and see how the layers for building a Pooly work.
Each example layer should start with a number, this indicates the layer that trait is in the [Layer Composition](PoolyBuilder.md#swooping-into-the-details).

There will also be a Wire Frame group, this has a few layers in it that just provide an outline of where each of the traits layers in the layer composition exist. The Body Layer is a basic rectangle at the bottom center of the image, however staying in the bounds is not required, many body variations have wings or feet built into the Body Layer.
Same with the Head layer, staying within the bounds is not required, many of the craw designs on the head go outside the bounds, and a few variations explore Pooly with a turned head where much of the beak and craw are outside the bounds.

The other points are the connect points for the traits, so if wings or something else is to be added to either side of the body, they should overlap with the slim rectangles on either side of the body.
If something is designed to come our of the mouth of Pooly the single pixel point in the head is where the current traits come out of.
It's not required to use this location, but this location will be the location that will always work for all designs.
If eyewear is design the eye locations are also provided.
For hat wear the top rectangle is provided where a hat currently overlaps with the head.
Most hats also extend past the head by one or two pixels on either side to help cover the craw but this is not required.

It's also not necessary that all traits are composed at once, use some of the examples as a base and build the one or two traits desired.
For instance if a designer just want to build a hat, just build the hat in the corresponding location, delete all the example groups and wire frame when completed, save the SVG as a new hat with a clever name and submit a pull request.

#### What's Next
Build your Pooly!
In time an SVG with all traits will be compiled so an artist will be able to bring their custome trait into the SVG and see how their trait interacts with the other traits.
🪶🛡️

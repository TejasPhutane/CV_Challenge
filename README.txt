This is a coding challenge for computer vision.

In this challenge, we are matching the street view imagery to satellite imagery. The goal of this challenge is to find computer vision features that are common between the street view images and the aerial images from a folder.

The notation of the feature should have a unique identifier that is consistent across all the images.

e.g.

[{
    feature_id : "[id]",
    street_img : {
        path : "set 1/1607080640.0_51.45696126666542_-0.3218871507160777.jpg",
        x: [position in x from top left],
        y: [position in y from top left]
    },
    ref_imgs : [{
        path : "set 1/Screen Shot 2021-04-28 at 9.26.20 AM.png",
        x: [position in x from top left],
        y: [position in y from top left],
    },{
        path : "set 1/Screen Shot 2021-04-28 at 9.26.45 AM.png"   
        x: [position in x from top left],
        y: [position in y from top left],
    },{
        path : "set 1/Screen Shot 2021-04-28 at 9.26.58 AM.png"   
        x: [position in x from top left],
        y: [position in y from top left],
    }]

},
{...},
{...}]


At the minimum the feature must match atleast one of the reference satellite images in order to be considered. Features that have no matches must be thrown out.

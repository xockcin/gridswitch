A pretty, minimalist Bejeweled clone, made with Bootstrap and JQuery.

## Step One: Make the Grid

Make a grid of 12 columns and eight rows, populated with randomly colored buttons.

## Step Two: Enable Switching

Make it so that, when you click on two adjacent buttons, they switch colors.

## Step Three: Find Groups of Three

Just find them - don't do anything with them yet.

Note: It now records groups of three, but records groups of four as two groups of three. I will need to fix that.

## Step Four: Find Groups of Any Size

So it's like this: You're sitting at a conveyor belt that is delivering you a random sequence of different-colored beads. You have a big envelope and a bunch of small envelopes. You put the first bead in an empty small envelope and write "CURRENT" on the front of it with a Sharpie. Then you move onto the next bead. If this bead is the same color as the previous bead, put it in CURRENT. If this bead is not the same color as the previous bead, seal CURRENT, deposit it into the large envelope, grab a new small envelope, write CURRENT on it, and put this bead into CURRENT. Then, once all the beads are in the envelope, sort out and throw away all the small envelopes that contain fewer than three beads. Boom!

NOTE TO SELF: This app is written such that the data is stored in the DOM. That seems like bad design and a rookie mistake. It's like the skin is inside the bones. Eventually I will refactor this program so that the logic is first. Actually, I'll probably just use React. But for now I will persist in my folly.

## Step Five: Make The Sets Disappear

When the grid appears, wait two seconds, and then make all the sets of three or more disappear. For now, only the horizontal sets - I can deal with the vertical ones later. And for now, just make them disappear - don't worry yet about the buttons above moving down to take their place.

NOTE TO SELF: At the time of this writing, it removes SOME of the sets but not all of them. I don't know what's going on!
Addendum: Ok, I know what the problem is: it's not counting the sets that are all the way to the right. Somehow those aren't getting added to the big envelope. I knew this was going to be a problem, and now I have to figure it out.

## Step Six: Make The Sets Wait A Second Before They Disappear

NOTE TO SELF: I opted to use JQuery effects, which forced me to find a newer CDN link. Interesting.

## Step Seven: Make The Buttons Above The Empty Squares Move Down To Fill The Space

This will be tricky.
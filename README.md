# aliss
Automatic Length Inference Scoring System

Developed for Drone-Assisted Seated Chair Bocce, the world's hottest new sport.
Take an aerial picture of each round of the game, upload them to ALISS, and sit
back as she locates the balls, calculates their distances from the jack, and
tallies the final score.

NOTE: ALISS is great for long-term tracking of scores and statistics, but the
"Inference" bit of her name means she is no susbstitute for a good Senior Head
Chief Regional Supervising Referee. Final rulings are up to the SHCRSR.

TECHNICAL STUFF AND HOW TO USE:

Written in Python 3.8

For greatest reliability, replace the template images ("jack.jpg," "green.jpg,"
and "red.jpg") with respective templates created with your own balls using the
code in "image_avg" on this same  GitHub profile (diego-80). Note that you'll
have to adjust the px_to_in() funtion to match the particular physical and
digital dimensions of your setup.

"aliss.py," and the template images (either yours or the provided ones) should
all be in the same directory. Also in this directory should be a subdirectory
containing input images. Specify the input directory from the command line,
hard-code it in main(), or simply name it "input" and ALISS's defaults will
kick in. You can also optionally specify an output directory (either an existing
one or one for ALISS to create) in the same ways. If you specify an input but
not an output from the command line, ALISS will automatically create a
subdirectory with the name of the input and "\_output" appended. If giving both
input and output from the command line, do so in that order.

The final score based on one image per round will be printed to the console.
A long-term tracking system which will cooperate with ALISS to aggregate scores
and statistics over time is currently in development.

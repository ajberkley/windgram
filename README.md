# windgram
Common lisp code to process a set of geo-referenced data into a windgram, like those seen at: http://canadarasp.com/windgrams

The current canadarasp.com code uses an ancient set of NCL scripts to do this, but it's slow and tied tightly to the data.  This is an attempt to rewrite the generation in the language the rest of the back end is written in, Common Lisp.  I'll be using CL-GDAL and probably GNUPLOT, or else CL-GDAL, CL-GD, and CL-PNG (the trifecta used to generate the map overlay plots at: http://canadarasp.com/).  This is actually just step one of then moving the backend to serving the raw windgram data and generating the windgrams in the browser (currently the back end data is stored too coarsely for this, so all the processing is server side).

Anyway, I'll see where we are after a couple dozen hours and either skip this step and go straight to javascript (booo, no fun!)

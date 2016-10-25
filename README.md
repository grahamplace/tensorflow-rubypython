# tensorflow-rubypython
A an example of using RubyPython to access TensorFLow

I built this because the recommended installation method for
https://github.com/somaticio/tensorflow.rb
is "use Docker", which is generally shorthand for "we don't know how to
construct software correctly". The "build from source" instructions
required SWIG and some Google serialization libraries and ...
wait, isn't TensorFlow a Python module?

Yes, it is, and RubyPython (gem install rubypython) has allowed Ruby to 
run Python code for years now. OK, to be fair, RubyPython stopped working
awhile back, but it's easy enough to fix.

The tensorflow.rubypython.rb includes the general RubyPython fixes, as well
as an implementation of the code from the TensorFlow introduction at
  https://www.tensorflow.org/versions/r0.11/get_started/index.html
as a proof-of-concept.

This might grow into an actual TensorFlow wrapper if there proves to be a
need, but really, it looks like a simple RubyPython initialization is al
that's required.


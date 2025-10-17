# Vocal Time-Stretcher

A short experiment into time-domain audio stretching (and compression) using the overlap-add algorithm (see the `DropStretcher` class in the [notebook](./vocal_resampler.ipynb)). It turns out that time-domain algorithms handle speech much better than frequency-domain methods, since those struggle with long pitch periods from deep voices. If you actually want something robust, then you should probably use the TD-PSOLA algorithm, which builds on the ideas explored here, or check out a library like [sonic](https://github.com/waywardgeek/sonic).

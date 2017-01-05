# Real

This package exports a single type, `Real`, that can be defined at compile time to alias either `Float` or `Double`.

## Usage

The default is behaviour is to use `Float`. If you need double precision, set `swiftc` compiler flag `REAL_DOUBLE` e.g.:

	swift build -Xswiftc -DREAL_DOUBLE
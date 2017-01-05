# Real

This package exports a single type, `Real`, that can be defined at compile time to alias either `Float` or `Double`.

## Why not use generics?

Because Swift generics have no concept of a type's default value. This means it's impossible (as far as I can tell) to have generic parameters default to zero. Instead, all default values must be provided explicitly.

## Usage

The default is behaviour is to use `Float`. If you need double precision, set `swiftc` compiler flag `REAL_DOUBLE` e.g.:

	swift build -Xswiftc -DREAL_DOUBLE


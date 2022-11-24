# Forro

This is a sample verifier built on top of Boogie.

Forro gives a translation from a toy language, called Forro after the Brazilian
folk dance, into Boogie. The language only has integers, but it supports memory
allocation and heap dereferencing. Memory allocation returns an integer, but
you're told it's an integer that is "valid as a pointer". Heap dereferencing
takes an integer, but requires that the integer is valid as a pointer.

Build using .NET 6.0:

```
dotnet build src/Forro.sln
```

Run on an example program:

```
dotnet run --project src/Forro/Forro.fsproj test/prog0.forro
```

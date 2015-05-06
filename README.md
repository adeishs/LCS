# NAME

LCS - Longest Common Subsequence

# SYNOPSIS

    use LCS;

# DESCRIPTION

LCS is an implementation based on a LCS algorithm.

## CONSTRUCTOR

- new()

    Creates a new object which maintains internal storage areas
    for the LCS computation.  Use one of these per concurrent
    LCS() call.

## METHODS

- LCS(\\@a,\\@b)

    Finds a Longest Common Subsequence, taking two arrayrefs as method
    arguments. It returns an array reference of corresponding
    indices, which are represented by 2-element array refs.

- LLCS(\\@a,\\@b)

    Calculates the length of the Longest Common Subsequence.

- allLCS(\\@a,\\@b)

    Finds all Longest Common Subsequences. It returns an array reference of all
    LCS.

- lcs2align(\\@a,\\@b,$LCS)

    Returns the two sequences aligned, missing positions are represented as empty strings.

- sequences2hunks($a, $b)

    Transforms two array references of scalars to an array of hunks (two element arrays).

- hunks2sequences($hunks)

    Transforms an array of hunks to two arrays of scalars.

- align2strings($hunks, $gap\_character)

    Returns two strings aligned with gap characters.

- fill\_strings($string1, $string2, $fill\_character)

    If one of the two strings is shorter, fills it up to the same length.

- max($i, $j)

    Returns the maximum of two numbers.

## EXPORT

None by design.

# AUTHOR

Helmut Wollmersdorfer <helmut.wollmersdorfer@gmail.com>

# COPYRIGHT

Copyright 2014- Helmut Wollmersdorfer

# LICENSE

This library is free software; you can redistribute it and/or modify
it under the same terms as Perl itself.

# SEE ALSO

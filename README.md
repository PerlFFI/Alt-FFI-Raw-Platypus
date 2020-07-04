# Alt::FFI::Raw::Platypus [![Build Status](https://travis-ci.org/PerlFFI/Alt-FFI-Raw-Platypus.svg)](http://travis-ci.org/PerlFFI/Alt-FFI-Raw-Platypus)

Alternate FFI::Raw implementation powered by FFI::Platypus

# SYNOPSIS

```
env PERL_ALT_INSTALL=OVERWRITE cpanm Alt::FFI::Raw::Platypus
```

# DESCRIPTION

This distribution provides an alternative implementation of [FFI::Raw](https://metacpan.org/pod/FFI::Raw) that uses
[FFI::Platypus](https://metacpan.org/pod/FFI::Platypus) instead of its own XS code.  This may be useful in situations
that you want to use modules that rely on [FFI::Raw](https://metacpan.org/pod/FFI::Raw) on platforms that are not
supported by the original implementation.  This approach should allow you to use
[FFI::Raw](https://metacpan.org/pod/FFI::Raw) code without changing any code!

This implementation uses [FFI::Platypus::Legacy::Raw](https://metacpan.org/pod/FFI::Platypus::Legacy::Raw) which is a fork of the
original [FFI::Raw](https://metacpan.org/pod/FFI::Raw) that lives in its own namespace.  The former is useful when
you want to migrate to Platypus from Raw to take advantage of its type system
and ability to attach xsubs, but do not want to change all of your code all at
once.

# SEE ALSO

- [Alt](https://metacpan.org/pod/Alt)
- [FFI::Platypus](https://metacpan.org/pod/FFI::Platypus)
- [FFI::Platypus::Legacy::Raw](https://metacpan.org/pod/FFI::Platypus::Legacy::Raw)

# AUTHOR

Graham Ollis <plicease@cpan.org>

# COPYRIGHT AND LICENSE

This software is copyright (c) 2019 by Graham Ollis.

This is free software; you can redistribute it and/or modify it under
the same terms as the Perl 5 programming language system itself.

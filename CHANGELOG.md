1.2.1
-----

- Enable frozen_string_literal and do a bit of code cleanup

1.2.0
-----

- Add `IPAddr#link_local?` [Feature #10912](https://bugs.ruby-lang.org/issues/10912)
- Add `IPAddr#private?` [Feature #11666](https://bugs.ruby-lang.org/issues/11666)
- Add `IPAddr#loopback?`
- IPAddr.new now rejects invalid address mask. [Bug #13399]
- Warn that `IPAddr#ipv4_compat` and `#ipv4_compat?` are deprecated [Bug #13769]

1.1.0
-----

- Add IPAddr#prefix

1.0.0
-----

- Initial release as gem extracted from ruby 2.4.1.

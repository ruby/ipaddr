1.2.3
-----

- Ruby 2.3 is the minimum supported version
- Follow the license change in Ruby and add BSD-2-Clause
- Make the parser a bit stricter [Bug #15832](https://bugs.ruby-lang.org/issues/15832)
  - Disallow leading zeros and extra slashes in mask
- Make IPAddr#include? consider range of argument [Bug #14119](https://bugs.ruby-lang.org/issues/14119)
- Support zone identifiers in IPv6 addresses [Feature #10911](https://bugs.ruby-lang.org/issues/10911)
- Fix include? and ipv4_mapped (https://github.com/ruby/ipaddr/pull/31)

1.2.2
-----

- Include the input in the message when raising InvalidAddressError [Feature #5987] (https://bugs.ruby-lang.org/issues/5987)

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

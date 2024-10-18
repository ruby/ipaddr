Unreleased
----------

- Add `IPAddr#to_json/as_json` [\#77](https://github.com/ruby/ipaddr/pull/77) ([taketo1113](https://github.com/taketo1113))
- Consider IPv4-mapped IPv6 addresses link local/loopback if IPV4 address is private [\#65](https://github.com/ruby/ipaddr/pull/65) ([Earlopain](https://github.com/Earlopain))
- Fix broken exception messages [\#64](https://github.com/ruby/ipaddr/pull/64) ([lrandall-godaddy](https://github.com/lrandall-godaddy))
- ntop: Measure address size in bytes [\#61](https://github.com/ruby/ipaddr/pull/61) ([hanazuki](https://github.com/hanazuki))
- String\#split seems to be faster than capturing digits with Regexp [\#50](https://github.com/ruby/ipaddr/pull/50) ([amatsuda](https://github.com/amatsuda))
- Prefer String\#start\_with? over Regexp.match [\#49](https://github.com/ruby/ipaddr/pull/49) ([amatsuda](https://github.com/amatsuda))
- Add IPAddr\#wildcard\_mask [\#44](https://github.com/ruby/ipaddr/pull/44) ([taketo1113](https://github.com/taketo1113))
- Add IPAddr.cidr to return ip address in cidr notation [\#23](https://github.com/ruby/ipaddr/pull/23) ([beanieboi](https://github.com/beanieboi))

1.2.6
-----

- Consider IPv4-mapped IPv6 addresses private if IPv4 address is private [\#57](https://github.com/ruby/ipaddr/pull/57) ([jeremyevans](https://github.com/jeremyevans))
- Improve performance of include? by 5-10x [\#47](https://github.com/ruby/ipaddr/pull/47) ([skipkayhil](https://github.com/skipkayhil))

1.2.5
-----

- No user-visible changes for gem users

1.2.4
-----

- Fix exception calling `to_range' after `freeze' - fix \#35 [\#36](https://github.com/ruby/ipaddr/pull/36) ([esparta](https://github.com/esparta))
- IPAddr\#native must also coerce `@mask_addr` [\#34](https://github.com/ruby/ipaddr/pull/34) ([casperisfine](https://github.com/casperisfine))
- Expose IPAddr::VERSION [\#33](https://github.com/ruby/ipaddr/pull/33) ([casperisfine](https://github.com/casperisfine))

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

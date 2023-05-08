# README

*MIME::Mini* - Minimal code to parse/create mbox files and mail messages

# Description

*MIME::Mini* is a small *perl* module containing a collection of functions
that parse and/or create mailbox (mbox) files and individual mail messages.

It is an alternative to *MIME-tools*. *MIME-tools* does things that this
module doesn't (such as uuencode and binhex decoding). And this module does
things that *MIME-tools* doesn't do, such as reading and writing mbox files
(repairing incorrectly formatted ones along the way), and transparently
unravelling `winmail.dat` attachments (aka *MS-TNEF*).

It is very small (about 3% of the size of *MIME-tools* and the other modules
that it requires, and about 20% of the size of I<MIME-Lite> (which doesn't
parse)), so it takes much less time during program start up. This makes it
more suitable for uses that require a separate process for each mail
message, such as in *procmail* recipes.

The following RFCs are relevant:

- RFC2822 - Internet Message Format
- RFC2045 - (MIME) Part One: Format of Internet Message Bodies
- RFC2046 - (MIME) Part Two: Media Types
- RFC2047 - (MIME) Part Three: Message Header Extensions for Non-ASCII Text
- RFC2231 - MIME Parameter Value and Encoded Word Extensions: Character Sets, Languages, and Continuations
- RFC2183 - Communicating Presentation Information in Internet Messages: The Content-Disposition Header Field
- RFC3282 - Content Language Headers
- RFC3066 - Tags for the Identification of Languages
- RFC2424 - Content Duration MIME Header Definition
- RFC2557 - MIME Encapsulation of Aggregate Documents, such as HTML (MHTML)
- RFC3297 - Content Negotiation for Messaging Services based on Email
- RFC2912 - Indicating Media Features for MIME Content
- RFC2533 - A Syntax for Describing Media Feature Sets
- RFC1864 - The Content-MD5 Header Field
- RFC2387 - The MIME Multipart/Related Content-type
- RFC2912 - Indicating Media Features for MIME Content
- RFC2533 - A Syntax for Describing Media Feature Sets
- RFC2076 - Common Internet Message Headers

This is free software; you can redistribute it and/or modify it under the
same terms as the Perl 5 programming language system itself.

# Documentation

There is a manual entry:

- <https://metacpan.org/pod/MIME::Mini>

# Download

*MIME::Mini* is on CPAN:

- <https://metacpan.org/dist/MIME-Mini>

And can be installed using any CPAN client:

        cpanm MIME::Mini

# Requirements

*MIME::Mini* is a perl module and requires no non-standard modules.
It should work on any system with any version of *perl* since v5.14.

--------------------------------------------------------------------------------

    URL: https://metacpan.org/dist/MIME-Mini
    GIT: https://github.com/rafmod/MIME-Mini
    GIT: https://codeberg.org/rafmod/MIME-Mini
    Date: 20230508
    Author: raf <raf@raf.org>


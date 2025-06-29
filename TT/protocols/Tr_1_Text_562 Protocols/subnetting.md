
I have a system. Really. It takes 15 minutes and a whiteboard. "Double and half"

I have non-networking people subnetting in their head. I taught a few security people to do it and had them show it off to unwitting network engineers. Works on IPv6 too.

I have taught experienced network engineers and they were annoyed that they have been doing it inefficiently for years. I should YouTube it.

Edit. /23 is one bit away from /24. /24 is a block of 256. Double and half. Forget the unusable first/last address.

Double. /23 is a block of 512. Now figure out the ranges.

Half. You need two /24 to make a /23. You have to gather them in two, and you must choose a boundary. 0 2 4 6

Range. Think of the dotted decimal like a car odometer. 192.168.(factor of two). 192.168.0.0/23 is 192.168.0.0 through 192.168.0.255 AND 192.168.1.0 on through to 192.168.1.255

/22 is four /24. Count by fours 192.168.0.0 through 192.168.3.255.

/21 is eights. 8,16,24,32,40,48,56,64. 192.168.32.0 to 192.168.39.255 - that last address is easy to find because it is one less than the start of the next range at 192.168.40.0.

/25 is half. /24 is 256. /25 is 128. Count by 128. 192.168.0.0 to 192.168.0.127 is the first block. The other is 192.168.0.128 to 192.168.0.255

Take that and apply it to any 8 bit range in the mask.

10.0.0.0/7 is double 10/8. You're combining 10/8 and the next block up, which is 11.0.0.0/8. Count by twos. Range is 10.0.0.0 to 11.255.255.255.

10.0.0.0/9 is half of 10/8. 10/8 is 10.0.0.0 to 10.255.255.255. Half? Second octet is 256 so half is 128. Two ranges. 10.0.0.0 to 10.127.255.255 and 10.128.0.0 to 10.255.255.255.

That works when you start at mask values 0 8 16 24 and 32. /32 is a host route. /31 is two up addresses. /30 is four.

0/0 is all addresses. First octet is all 256 values. 0/1 is class A. Half of all ipv4. Half of 256 is 128. 0.0.0.0 through 127.255.255.255.

Now figure out the range for CGN 100.64/10 - 100.64.0.0 through 100.127.255.255. Start at /8 or /16. It works either way. 16 is easier but involves more counting on fingers. What is 100.64/15? /14? Keep going.

#Adding geoip to wireshark / tshark parsing:

Match Packets with a Destination IP address in the United Starts:

ip.geoip.dst_country == "United States"

Match Packets to or from an IP address North of the Arctic Circle:

ip.geoip.lat > "66.5"

Match packets to or from an IP address in California:

ip.geoip.city contains "CA"

The display filter syntax has actually been expanded to include the following:
 
ip.geoip.asnum

ip.geoip.city

ip.geoip.country

ip.geoip.dst_asnum

ip.geoip.dst_city

ip.geoip.dst_country

ip.geoip.dst_lat

ip.geoip.dst_lon

ip.geoip.lat

ip.geoip.lon

ip.geoip.src_asnum

ip.geoip.src_city

ip.geoip.src_country

ip.geoip.src_lat

ip.geoip.src_lon

I have not seen the following work, but they are also included in the documentation.  Maybe they are "coming soon", or possibly they require another database:
 
ip.geoip.dst_isp

ip.geoip.isp

ip.geoip.org

ip.geoip.dst_org

ip.geoip.src_isp

ip.geoip.src_org

#Manuals:

https://learningnetwork.cisco.com/blogs/vip-perspectives/2010/12/11/geolocation-in-wireshark

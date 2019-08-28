# dns_resolver
DNS resolver from CSE 310 (Computer Networks)

How to run:
My program is ran through the command line. All my tests were done from the console
inside my IDE, Pycharm. You must have DNSPython installed, as this is the library I used to
query the DNS servers. Running the python script takes one argument, the website to query,
and outputs a mydig_output.txt to the same folder as mydig.py. Here is an example command
line command:
C:\...\(Path to mydig.py)> python mydig.py www.cs.stonybrook.edu
Explanation of data:
The data I collected is on the second page of this pdf. My results are significantly worse
than the other two DNS resolvers, but this was expected as this was my first time ever
implementing something like this, as well as my first time developing in python.
Google’s DNS resolver Proved to have better average times than my local DNS resolver
while experiencing higher times in most of the same websites (5, 8, 9, 12, 13, 18, 19, 21, and
22). One important extrapolation from the graph is where the average is greater than the 75th
percentile. This is an indication of having a fairly large outlier which is usually because of a
timeout. Google’s DNS resolver, for whatever reason, had much less timeouts than the local
resolver. This can be seen when comparing websites (5, 6, 7, 8, 10, 12, 13, 16, 19, 22, 24, and
25).
The conclusion I can draw from this data is that Google’s DNS resolver is better at
getting the IP addresses of popular websites, but additional tests would need to be down to find
if it is better in most cases. On top of this I can also conclude that you should not rely on using a
DNS resolver made by a sophomore college student.
If you wish to look at the exact data I obtained, here is a link to my data on a google
spreadsheet.

# latlong_to_UTM

If you work with large scale data from different parts of the world, you might very well be working with data projected using the UTM (Universal Transverse Mercator) map projection. As you may remember from working with data projected in UTM, there are 60 different UTM zones, each centred on different lines of longitude. If you need to define your projection, or reproject your data into UTM, you therefore need to know the zone number.

This program will automate which zone a particular x,y coordinate pair falls within. This is useful to convert large lat/long data to UTM in cases where software can give issues as this code will handle different types of errors usually found in CSV files.

Method1:

The easiest and convenient method of the three was using the equation. However, it was impossible
to convert latitudes to UTM bands as they were irregular in widths.] For method 1, the equation was
used for converting longitudes and a series of if-else statements for latitudes.
As I had an elementary practice with Java, the basics I had immensely helped me form ideas for the
code. The first step towards approaching the code was understanding the working of a basic
function(def) and an argument function. The next was correctly understanding the latitude bands,
UTM zone numbers, and their respective value ranges. I was aware of how to assign values to variables
and write if-else statements with my previous experience with Java and the notes given in the selflearning materials. The difference was only with the syntax.


Method2:

This method was challenging. I used dictionaries to look up values. Initially, I created sets of latitude
and longitude values but did not understand how to look up and generate their zone numbers or
bands. Then, the idea of dictionaries came up when I was researching hash tables as the most used
method to perform lookups. This article helped me form an idea of how to search and return the keys
if the dictionary contained multiple values for a single key. The input latitude/longitude values were
rounded off, and the dictionary only had whole number integers to make it easier to store multiple
values and taking up more space. I experimented with the NumPy.arange function to return various
values within the dictionary through a for-loop. This function can take the start, stop, and
difference(step) variables, effortlessly printing hundreds of numbers using a loop

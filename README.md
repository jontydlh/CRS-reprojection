# CRS-reprojection
A tool for batch-converting a series of coordinates from one Coordinate Reference System to another (e.g. latitude &amp; longitude to metres East and metres North) 

* This .ipynb script reads a specified CSV file, containing coordinate data with headers.

* The user must enter their desired input and output CRS according to its EPSG code (refer to https://epsg.io/).
  _For example, the latitude and longitude CRS used by GPS is EPSG:4326. (WGS84 - World Geodetic System 1984)._
  _A commonly used CRS for mE and mN covering the UK is EPSG:32629 (WGS 84 / UTM zone 29N)._

* The user must then enter the names of the headers under which the x and y coordinates are saved.

* The tool creates a new CSV file in the same directory as itself, called "reprojected.csv".
  _This is a copy of the original csv, with the reprojected coordinates appended._

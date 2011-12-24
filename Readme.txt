metadataRetriever - get the ID3 data of any unencrypted mp3 file.
Setup: 
1. Link against the AudioToolbox framework 
2. Add #import metadataRetriever.h  

Usage: NSArray *metadataArray = [metadataRetriever getMetadataForFile:@/path/to/file/];

this returns an array with the artist, song, and album info (in that order)  

to get the actual data, you must do the code below: 

NSString *artist = [metadataArray artistForMetadataArray:array]; 
NSString *song = [metadataArray songForMetadataArray:array]; 
NSString *album = [metadataArray albumForMetadataArray:array]; 

metadataRetriever Supports both iOS and MacOSX
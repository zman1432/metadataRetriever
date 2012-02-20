metadataRetriever - get the ID3 data of any unencrypted mp3 file.
Supports both iOS and MacOSX

Setup: 
1. Link against the AudioToolbox framework 
2. #import metadataRetriever.h  

Usage: NSArray *metadataArray = [metadataRetriever getMetadataForFile:@"/path/to/file.mp3"];

NSString *artist = [metadataArray objectAtIndex:0]; 
NSString *song = [metadataArray objectAtIndex:1]; 
NSString *album = [metadataArray objectAtIndex:2]; 

# url-shortener
This C++ URL shortener class generates shortened URLs using random alphanumeric codes. It maps long URLs to shorter, custom ones with a specified base URL. The class stores links in an unordered map and includes functions to shorten a link and retrieve the original link. It uses a random code generator to ensure unique codes.
This C++ URL Shortener program provides an efficient way to generate short URLs from longer ones. Designed as a `LinkShortener` class, it uses an unordered map to store shortened links, with each short link mapped to its corresponding original URL. 

The program includes a base URL (in this case, `"https://www.linkedin.com/in/"`), which serves as the prefix for each shortened link. The `shortenLink` function generates a unique, six-character code using alphanumeric characters. It checks for duplicates in the map to ensure each code is unique before mapping it to the original link. Once created, the shortened URL is saved in the map for easy retrieval. 

The `getOriginalLink` function allows users to look up the original URL from a given shortened link. If the link exists in the map, the function returns the original URL; otherwise, it returns an empty string to indicate that the link is invalid or not found.

The main function demonstrates the program’s functionality by creating a shortened URL and retrieving it to display both the original and shortened links. This URL shortener is efficient, with O(1) average time complexity for both insertion and retrieval due to the unordered map, and it's versatile enough to handle various URL shortening needs.

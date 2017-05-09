# C++ Utility Classes

Utility classes for C++. Updated as needed.

## String Utilities
#### `std::vector<std::string> SplitString(const std::string &input, const std::string &delimiter) noexcept`
##### Description: Splits a string based on tokens

<br>

#### `void TrimInPlace(std::string& input) noexcept`
##### Removes whitespace from the beginning and end of a string. Mutates the input string

<br>

#### `std::string Trim(const std::string& input) noexcept`
##### Removes whitespace from the beginning and end of a string. Returns the trimmed string

<br>

#### `std::string TrimFront(const std::string& input) noexcept`
##### Removes whitespace from the beginning. Returns the trimmed string

<br>

#### `std::string TrimBack(const std::string& input) noexcept`
##### Removes whitespace from the end of a string. Returns the trimmed string

<br>

#### `bool IsNumber(const std::string& input) noexcept`
##### Returns true if the input string is an integer number, false otherwise

<br>

#### `std::string ToStringWithPrecision(const T& number, const int decimalPlaces) noexcept`
##### Returns a string of the passed in number formated with decimal spaces

<br>

#### `bool Contains(std::string input, std::string substring) noexcept`
##### Retruns true if the substring is contained in the input strung, false otherwise

<br>

#### `bool StartsWith(std::string input, std::string substring) noexcept`
##### Returns true if the input string starts with the substring, false otherwise

<br>

#### `bool EndsWith(std::string input, std::string substring) noexcept`
##### Returns true if the input string ends with the substring, false otherwise

<br>

#### `bool IsLower(char c) noexcept`
##### Returns true if the character is lowercase, false otherwise

<br>

#### `bool IsUpper(char c) noexcept`
##### Returns true if the character is uppercase, false otherwise

<br>

#### `bool IsChar(char c) noexcept`
##### Returns true if the character is an ASCII character, false otherwise

<br>

#### `std::string ToUpper(const std::string &toConvert) noexcept`
##### Returns a new string with the input string converted to uppercase

<br>

#### `std::string ToLower(const std::string &toConvert) noexcept`
##### Returns a new string with the input string converted to lowercase

<br>

### To use
* Include in `#include "StringUtils.h"` in the source file you would like to use.

### Example: 2 options
1. You can prepend `StringUtils::` to any function calls such as `StringUtils::IsLower('a');`
2. Include the namespace by `using namespace StringUtils` and call the functions directly `IsLower('a');`
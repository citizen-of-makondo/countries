[![](https://jitpack.io/v/citizen-of-makondo/countries.svg)](https://jitpack.io/#citizen-of-makondo/countries)

# Countries Library

Simple Kotlin library for working with country codes, names and flags.

## Installation

Add the JitPack repository to your build file. Add it in your root build.gradle at the end of repositories:

```gradle
allprojects {
    repositories {
        ...
        maven { url 'https://jitpack.io' }
    }
}
```

Add the dependency:

```gradle
dependencies {
    implementation 'com.github.citizen-of-makondo:countries:1.0.0'
}
```

## Usage

```kotlin
// Get all countries
val countries = CountryUtils.getAllCountries()

// Find country by code
val russia = CountryUtils.findByCode("RU")
println("${russia?.name} ${russia?.flag}")

// Find countries by name
val islandCountries = CountryUtils.findByName("island")
islandCountries.forEach { 
    println("${it.name} ${it.flag}")
}
```

## License

```
MIT License

Copyright (c) 2025 citizen-of-makondo

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

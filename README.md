# Mapeo Presets Builder

`mapeo-presets-builder` exists for the sole function of building packages of presets for the Mapeo Desktop application. 


## Table of Contents

- [Installation](#installation)
- [Usage](#usage)

## Install

```
npm install mapeo-presets-builder
```

## Usage

Mapeo Presets Builder expects to be run from within a very specific file structure, which is as follows:

* categories
  * JSON category files
* fields
  * JSON field files
* presets
  * preset category folders
     * JSON preset files
  * uncategorized JSON preset files
* schema
  * JSON schema files
* sprites
  * 24-px and 100-px SVG format sprite images
* defaults.json
* imagery.json
* region.css (used to be wao.css)

Run with the command `mapeo-presets-builder` (or `./node_modules/.bin/mapeo-presets-builder` if it is not correctly exported into your path) to create a `presets.mapeopresets` file within the build folder. `presets.mapeopresets` is a tarball that can be unzipped or opened with Mapeo Desktop.


## Development Status

Not stable--needs better error-handling and testing. Mapeo Desktop also still needs to be given the capacity to open .mapeopresets files.
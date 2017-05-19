# MP3LibraryClean
I needed something to keep my library together ;)

## Purpose
Easy to program modular application to iterate across MP3 files and perform actions

## Main Application
The main application actually has no abiliy to do anything other than scan for files.
It's purpose is to interpret configuration directives, Providing a sane view of all configuration for each module.

## Modules
### Structure 
This module performs library Structuring based on supplied configuration.
### Rename
Renames files based on supplied configuration.
### TagCleanup
This module applies basic features such as character limits ( Example: Removing all non-ascii characters ) and performs specific cleanups such as whitespace trimming.

## Configuration File
### Configuration Layout
* Global
** Global Configuration is applied to the main application and all sub-modules, it provides the basic required configuration as well as holds global shared module settings.
* Module
** Module Configuration supplies the configuration for a Module and will override any Global Configuration for that module only.
* Path
** Path Configuration is a regex based section which supplies configuration overrides for a specific path match.


# Inconsistent Expo CLI Native Module Linking Errors in CI/CD

This repository demonstrates a problem encountered during the build process of an Expo application using native modules.  The issue is an inconsistent failure in the native module linking stage, occurring specifically within a CI/CD pipeline environment. The error is not consistently reproducible and often builds successfully locally.

## Steps to Reproduce

1. Clone this repository.
2. Run `npm install`.
3. Try running `expo build:ios` and/or `expo build:android` locally. Observe if the build is successful. 
4. Attempt to build via your CI/CD pipeline (refer to the CI/CD configuration file in the repo). Observe the inconsistency in build success. 

## Potential Causes

* Issues with the node version. 
* Problems with the expo CLI installation process. 
* Differences in environment variables or system configurations between local and CI/CD environments. 
* Potential caching or temporary file issues. 

## Solution

Refer to expoBugSolution.js for a potential solution or set of approaches that helped resolve this issue.

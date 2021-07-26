# MalDocA - Malicious Document Analyzer

MalDocA is a library to parse and extract features from Microsoft Office documents. It supports both OLE and OOXML documents.

The project's goal is to analyze potentially malicious documents to improve user safety and security.

## REQUIREMENTS
- [Bazel](https://bazel.build) (recommended version: 4.1.0)
- [Clang](https://clang.llvm.org) (recommended version: 11 or 12)
- Windows: enable symlink support ([how-to](https://docs.bazel.build/versions/main/windows.html#enable-symlink-support))

## CHECKOUT
git clone --recurse-submodules https://github.com/google/maldoca.git

cd maldoca

## DOCKER
We proivde a docker file in "docker/Dockerfile". This is the reference
platform we use for continous integration and optionally (arguably recommended)
for development as well. Please check the documentation in "docker/Dockerfile" on how to
build and use for development.

## BUILD
Linux: bazel build --config=linux //maldoca/...

Windows: bazel build --config=windows //maldoca/...

## TEST
Linux: bazel test --config=linux //maldoca/...

Windows: bazel test --config=windows //maldoca/...

## CONTACT
maldoca-community@google.com

## DISCLAIMER
This is not an official Google product.

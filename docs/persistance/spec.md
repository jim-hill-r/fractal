# Files
- Files must be self describing. We have used extensions and mimeTypes as a crutch for too long. Any process should be able to take in a file, read that file, decode that file, and parse that file without any external metadata.
  - Why?
  - A self-describing file cannot be spoofed.
  - A file that is supposed to be data cannot instead be executed. 
  - The entirety of it's existence can be encrypted at rest and in transit making it much harder to know what it is or how to hack it.

# Memory
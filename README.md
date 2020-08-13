# NGL Viewer Test - Team IISER Pune India - iGEM 2020

A simple site setup to test [NGL](https://github.com/nglviewer/ngl), for later embedding in the iGEM Wiki.

iGEM requires all files to be locally served, and has restrictions on what kinds of files can be uploaded to the server. The allowed formats do not include `.pdb` files, so we use a simple workaround:

- Rename the `.pdb` file to `.txt` file
- Pass the `ext: 'pdb` parameter into the `stage.loadFile` function, as in:

```js
stage.loadFile('5mza.txt', {ext: 'pdb'})
```


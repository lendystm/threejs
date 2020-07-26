# Herosaver

Methodology to Save Configuration and STLs from websites using the THREE.JS framework for academic and educational purposes.

Please **Always** think about the **developers** of such websites and try to **support them whenever possible**, as without them, there would be no such tools.

## Usage
### Browser Console
  1. Go to the intended website
  2. Open the Javascript Console [F12], then click on Console
  3. Paste the following

```
var xhr=new XMLHttpRequest;xhr.open("get","https://raw.githubusercontent.com/lendystm/threejs/master/dist/saver.min.js",true);xhr.onreadystatechange=function(){if(xhr.readyState==4){var script=document.createElement("script");script.type="text/javascript";script.text=xhr.responseText;document.body.appendChild(script)}};xhr.send(null);
```

## Limitations

* This is a collaborative effort by people of the community, so the output is not perfect. 
* If you want higher quality exports, consider purchasing the stl files or help work on the code :)
* The outputted file is not a solid object, but a set of objects which is fine for some uses, but can be problimatic if you want to print the 3D object. You will probabily need to combine these into a solid ojbect, Consider using [Meshmixer](http://www.meshmixer.com/download.html "Meshmixer Download Link") (or equvilient) to produce a printable output, some guides below.

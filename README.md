# SVG to Javascript object

## What is it

**svg-to-json** is a library which can transform a SVG into a javascript objects(JSON) and viceversa, written in JavaScript. It's
based on the original version is XML.ObjTree developed by [Yusuke Kawasaki](https://github.com/kawanet) a parser/generater for XML source code and JavaScript objects.


## Installation

Include either `svg-to-json.js` or `svg-to-json.min.js` in your page
and it will make the `XML.ObjTree` variable available in the global scope.

## Usage

```html
<script src="path/to/svg-to-json.min.js" />
<script>
    //convert svg to json 
    var xotree = new XML.ObjTree();
    var dumper = new JKL.Dumper(); 
    var json = xotree.parseXML('raw-svg-data');

    //convert json to svg
    var xotree = new XML.ObjTree();
    var json = eval("(" + json-value + ")");
    var svg = formatXml(xotree.writeXML(json)); 
</script>
```

## Authors

Karthick Kumar, Yusuke Kawasaki (original idea)

## License

MIT

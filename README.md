![logo](public/logo.jpg)
# jaspit
Simple report rendering library based on Jasper Report

# Usage
```
<div id="report"></div>

<script type="text/javascript" src="jaspit.bundle.min.js"></script>
<script>
Jaspit.render({
	dom_id:"report",
	fetch:true,//if true, the following two parameters will be taken as URL
	design:"/invoice.jrxml",
	data:"/invoice.json",
	param:{logo1:'/logo.jpg'},
	done:function(){//will be called when render is complete
		//uncomment to print from browser
		//print();
	}
});
</script>
```

# Development
Clone this repo, then `npm install`
- Run `npm run dev`
- Then visit [http://localhost:9000](http://localhost:9000/)

## Future plan

- Editor
- Support for most components
- CLI

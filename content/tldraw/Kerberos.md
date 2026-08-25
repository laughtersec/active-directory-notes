---
tldraw-file: true
tags: []
---

````json !!!_START_OF_TLDRAW_DATA__DO_NOT_CHANGE_THIS_PHRASE_!!!
{
	"meta": {
		"plugin-version": "1.0.6",
		"tldraw-version": "2.1.4"
	},
	"raw": {
		"document:document": {
			"gridSize": 10,
			"name": "",
			"meta": {},
			"id": "document:document",
			"typeName": "document"
		},
		"page:page": {
			"meta": {},
			"id": "page:page",
			"name": "Page 1",
			"index": "a1",
			"typeName": "page"
		},
		"shape:f4yomPZLjlKxrI3ECEZh1": {
			"x": 787,
			"y": 133.5625,
			"rotation": 0,
			"isLocked": false,
			"opacity": 1,
			"meta": {},
			"id": "shape:f4yomPZLjlKxrI3ECEZh1",
			"type": "geo",
			"props": {
				"w": 206,
				"h": 118,
				"geo": "rectangle",
				"color": "light-blue",
				"labelColor": "black",
				"fill": "none",
				"dash": "draw",
				"size": "m",
				"font": "mono",
				"text": "Domain Controller",
				"align": "middle",
				"verticalAlign": "middle",
				"growY": 0,
				"url": ""
			},
			"parentId": "page:page",
			"index": "a1",
			"typeName": "shape"
		},
		"shape:QrVCNkCiIeumNgJTIT4im": {
			"x": 407,
			"y": 438.5625,
			"rotation": 0,
			"isLocked": false,
			"opacity": 1,
			"meta": {},
			"id": "shape:QrVCNkCiIeumNgJTIT4im",
			"type": "geo",
			"props": {
				"w": 214,
				"h": 127,
				"geo": "rectangle",
				"color": "yellow",
				"labelColor": "black",
				"fill": "none",
				"dash": "draw",
				"size": "m",
				"font": "mono",
				"text": "Client",
				"align": "middle",
				"verticalAlign": "middle",
				"growY": 0,
				"url": ""
			},
			"parentId": "page:page",
			"index": "a2",
			"typeName": "shape"
		},
		"shape:pzEQwag9rKuY3BJDMyQAA": {
			"x": 1072,
			"y": 506.5625,
			"rotation": 0,
			"isLocked": false,
			"opacity": 1,
			"meta": {},
			"id": "shape:pzEQwag9rKuY3BJDMyQAA",
			"type": "geo",
			"props": {
				"w": 213,
				"h": 124,
				"geo": "rectangle",
				"color": "orange",
				"labelColor": "black",
				"fill": "none",
				"dash": "draw",
				"size": "m",
				"font": "mono",
				"text": "Application Server",
				"align": "middle",
				"verticalAlign": "middle",
				"growY": 0,
				"url": ""
			},
			"parentId": "page:page",
			"index": "a3",
			"typeName": "shape"
		},
		"shape:BYyOHkQVU91QeiQ5RTjGt": {
			"x": 492,
			"y": 375.5625,
			"rotation": 0,
			"isLocked": false,
			"opacity": 1,
			"meta": {},
			"id": "shape:BYyOHkQVU91QeiQ5RTjGt",
			"type": "arrow",
			"parentId": "page:page",
			"index": "a4",
			"props": {
				"dash": "draw",
				"size": "s",
				"fill": "none",
				"color": "yellow",
				"labelColor": "black",
				"bend": 0,
				"start": {
					"type": "point",
					"x": -69,
					"y": 57
				},
				"end": {
					"type": "point",
					"x": 295,
					"y": -219
				},
				"arrowheadStart": "none",
				"arrowheadEnd": "arrow",
				"text": "1. AS-REQ",
				"labelPosition": 0.5,
				"font": "mono"
			},
			"typeName": "shape"
		},
		"shape:wHL2bC_W7faAN8xbDpint": {
			"x": 787,
			"y": 249.5625,
			"rotation": 0,
			"isLocked": false,
			"opacity": 1,
			"meta": {},
			"id": "shape:wHL2bC_W7faAN8xbDpint",
			"type": "arrow",
			"parentId": "page:page",
			"index": "a1V",
			"props": {
				"dash": "draw",
				"size": "s",
				"fill": "none",
				"color": "light-blue",
				"labelColor": "black",
				"bend": 0,
				"start": {
					"type": "binding",
					"boundShapeId": "shape:f4yomPZLjlKxrI3ECEZh1",
					"normalizedAnchor": {
						"x": 0,
						"y": 0.9830508474576272
					},
					"isPrecise": false,
					"isExact": false
				},
				"end": {
					"type": "point",
					"x": -209,
					"y": 186
				},
				"arrowheadStart": "none",
				"arrowheadEnd": "arrow",
				"text": "2. AS-REP",
				"labelPosition": 0.5,
				"font": "mono"
			},
			"typeName": "shape"
		},
		"shape:lGFHv7W3THa2xU4Q3rx5U": {
			"x": 624,
			"y": 463.5625,
			"rotation": 0,
			"isLocked": false,
			"opacity": 1,
			"meta": {},
			"id": "shape:lGFHv7W3THa2xU4Q3rx5U",
			"type": "arrow",
			"parentId": "page:page",
			"index": "a1G",
			"props": {
				"dash": "draw",
				"size": "s",
				"fill": "none",
				"color": "light-green",
				"labelColor": "black",
				"bend": 94.79659820820115,
				"start": {
					"type": "point",
					"x": 0,
					"y": 0
				},
				"end": {
					"type": "point",
					"x": 283,
					"y": -205
				},
				"arrowheadStart": "none",
				"arrowheadEnd": "arrow",
				"text": "3. TGS-REQ",
				"labelPosition": 0.5,
				"font": "mono"
			},
			"typeName": "shape"
		},
		"shape:2p7cIPMM10CBpAWVx8ay7": {
			"x": 957,
			"y": 255.5625,
			"rotation": 0,
			"isLocked": false,
			"opacity": 1,
			"meta": {},
			"id": "shape:2p7cIPMM10CBpAWVx8ay7",
			"type": "arrow",
			"parentId": "page:page",
			"index": "a2V",
			"props": {
				"dash": "draw",
				"size": "s",
				"fill": "none",
				"color": "light-green",
				"labelColor": "black",
				"bend": -134.71684711476087,
				"start": {
					"type": "point",
					"x": 24,
					"y": 0
				},
				"end": {
					"type": "point",
					"x": -333,
					"y": 301
				},
				"arrowheadStart": "none",
				"arrowheadEnd": "arrow",
				"text": "4. TGS-REP",
				"labelPosition": 0.5,
				"font": "mono"
			},
			"typeName": "shape"
		},
		"shape:8zQTz5skEYI3PWeRck4FB": {
			"x": 568,
			"y": 566.5625,
			"rotation": 0,
			"isLocked": false,
			"opacity": 1,
			"meta": {},
			"id": "shape:8zQTz5skEYI3PWeRck4FB",
			"type": "arrow",
			"parentId": "page:page",
			"index": "a5",
			"props": {
				"dash": "draw",
				"size": "s",
				"fill": "none",
				"color": "yellow",
				"labelColor": "black",
				"bend": 73.04135221305927,
				"start": {
					"type": "point",
					"x": 0,
					"y": 0
				},
				"end": {
					"type": "point",
					"x": 498,
					"y": 23
				},
				"arrowheadStart": "none",
				"arrowheadEnd": "arrow",
				"text": "5. AP-REQ",
				"labelPosition": 0.5,
				"font": "mono"
			},
			"typeName": "shape"
		},
		"shape:CXHVauSVKCzdlPBPmf23K": {
			"x": 1097,
			"y": 633.5625,
			"rotation": 0,
			"isLocked": false,
			"opacity": 1,
			"meta": {},
			"id": "shape:CXHVauSVKCzdlPBPmf23K",
			"type": "arrow",
			"parentId": "page:page",
			"index": "a2G",
			"props": {
				"dash": "draw",
				"size": "s",
				"fill": "none",
				"color": "red",
				"labelColor": "black",
				"bend": -127.34116090692766,
				"start": {
					"type": "point",
					"x": 0,
					"y": 0
				},
				"end": {
					"type": "point",
					"x": -623,
					"y": -67
				},
				"arrowheadStart": "none",
				"arrowheadEnd": "arrow",
				"text": "Optional Mutual Authentication",
				"labelPosition": 0.5,
				"font": "mono"
			},
			"typeName": "shape"
		},
		"shape:Azw9V_MlIvw4YRyR6WxMc": {
			"x": 1129,
			"y": 501.5625,
			"rotation": 0,
			"isLocked": false,
			"opacity": 1,
			"meta": {},
			"id": "shape:Azw9V_MlIvw4YRyR6WxMc",
			"type": "arrow",
			"parentId": "page:page",
			"index": "a6",
			"props": {
				"dash": "draw",
				"size": "s",
				"fill": "none",
				"color": "orange",
				"labelColor": "black",
				"bend": 4.6497232103929536,
				"start": {
					"type": "point",
					"x": 0,
					"y": 0
				},
				"end": {
					"type": "point",
					"x": -134,
					"y": -305
				},
				"arrowheadStart": "none",
				"arrowheadEnd": "arrow",
				"text": "Optional PAC\nValid Request",
				"labelPosition": 0.5,
				"font": "mono"
			},
			"typeName": "shape"
		},
		"shape:5jX3TmFG5jjpNMXQiRfpP": {
			"x": 997,
			"y": 153.5625,
			"rotation": 0,
			"isLocked": false,
			"opacity": 1,
			"meta": {},
			"id": "shape:5jX3TmFG5jjpNMXQiRfpP",
			"type": "arrow",
			"parentId": "page:page",
			"index": "a7",
			"props": {
				"dash": "draw",
				"size": "s",
				"fill": "none",
				"color": "violet",
				"labelColor": "black",
				"bend": -81.30382375776871,
				"start": {
					"type": "point",
					"x": 0,
					"y": 0
				},
				"end": {
					"type": "point",
					"x": 256,
					"y": 352
				},
				"arrowheadStart": "none",
				"arrowheadEnd": "arrow",
				"text": "Optional PAC validation response",
				"labelPosition": 0.5,
				"font": "mono"
			},
			"typeName": "shape"
		}
	}
}
!!!_END_OF_TLDRAW_DATA__DO_NOT_CHANGE_THIS_PHRASE_!!! ```
````

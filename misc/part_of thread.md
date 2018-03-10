Granted that the RDF interpretation of this may not be as intended, the scenario you describe would look like this in the draft format (length of timespans array should be 5 to allow for earliest/latest start, earliest/latest end, label). To me, the subjects of the 'when' for all are their respective 'part_of' elements. At least, it's easy for me to imagine code to make that interpretation. When I [view this bit in JSON-LD Playground N-Quads](http://tinyurl.com/ybjg59ed) it seems to indicate correct s-p-o relations. I will flag this thread in twitter (@kgeographer) and ask for further input.

	{ "type": "FeatureCollection",
	  "@context": "http://linkedpasts.org/assets/place-v3-context.jsonld",
	  "features": [
	    { "@id": "myplace:Abingdon",
	       "part_of": [
		        { "id": "myplace:Berkshire",
		          "when": {"timespans": [["1600","1700","","1974",""]]}
		        },
		        { "id": "myplace:Oxfordshire",
		          "when": {"timespans": [["1974","","","2018",""]]}
		        }
	      	]
	     },
	     { "@id": "myplace:Oxford",
	       "part_of": [
		        { "id": "myplace:Oxfordshire",
		          "when": {"timespans": [["1000","","","2018",""]]}
		        }
	      	]
	    }
	  ]
	}


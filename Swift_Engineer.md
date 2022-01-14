You are writing a Swift app which needs to construct a model object using JSON data retrieved from a REST API. The model structure contains at least one integer value representing a counter. The REST API may represent this counter as a string or an integer in JSON. The response may also contain additional keys which need to be ignored, or no counter key at all, in which case it should be initialized to zero.

Examples of potential responses for the request GET /api/counts:

{ “counter”: 123 }
{ “color”: “red”, “counter”: “123” }
{ “counter”: “123”, foods:[“pizza”, “carrots”, { “cupcakes?”: “yes please” }] }
{ “counter”: 123, “false?”: true }
{ “oh no the counter is missing”: true }

How would you construct a robust Swift model such that counter is properly initialized in all of the above cases?

Please send us a zipped file of your files for this exercise. Do not submit a pull request.

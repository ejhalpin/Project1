# Project1

Requirements:
-Must uses at least two APIs
-Must use AJAX to pull data
-Must utilize at least one new library or technology that we haven't discussed
-Must have a polished frontend / UI
-Must meet good quality coding standards (indentation, scoping, naming)
-Must NOT use alerts, confirms, or prompts (look into modals!)
-Must have some sort of repeating element (table, columns, etc)
-Must use Bootstrap or Alternative CSS Framework
-Must be Deployed (GitHub Pages or Firebase)
-Must have User Input Validation

####Edamam.com Recipe API info

## example query string

- https://api.edamam.com/search?q=chicken&app_id=${YOUR_APP_ID}&app_key=${YOUR_APP_KEY}&from=0&to=3&calories=591-722&health=alcohol-free

## DEMO Query

- https://api.edamam.com/search?q=chicken&app_id=3f5ead16&app_key=c225ae2c7c6a61ce84c5a6514777dbd2&from=0&to=3&calories=591-722&health=alcohol-free

##Quesry deconstruction

- path: https://api.edamam.com/search?
- query string: q=chicken
- app id and key: &app_id=3f5ead16&app_key=c225ae2c7c6a61ce84c5a6514777dbd2
- limit the number of responses: &from=0&to=3
- extra search critera: &calories=591-722&health=alcohol-free : which returns recipes that have calories listed within the range given and have the tag "alcohol-free"

## Sample Result - format: JSON

{
"q": "chicken",
"from": 0,
"to": 3,
"params": {
"sane": [],
"q": [
"chicken"
],
"app_key": [
"c225ae2c7c6a61ce84c5a6514777dbd2"
],
"health": [
"alcohol-free"
],
"from": [
"0"
],
"to": [
"3"
],
"calories": [
"591-722"
],
"app_id": [
"3f5ead16"
]
},
"more": true,
"count": 11882,
"hits": [
{
"recipe": {
"uri": "http://www.edamam.com/ontologies/edamam.owl#recipe_d81795fb677ba4f12ab1a104e10aac98",
"label": "Citrus Roasted Chicken",
"image": "https://www.edamam.com/web-img/d4b/d4bb1e6c7a6c3738d8e01707eb0ad83d.jpg",
"source": "Food52",
"url": "https://food52.com/recipes/3403-citrus-roasted-chicken",
"shareAs": "http://www.edamam.com/recipe/citrus-roasted-chicken-d81795fb677ba4f12ab1a104e10aac98/chicken/alcohol-free/591-722-cal",
"yield": 4,
"dietLabels": [
"Low-Carb"
],
"healthLabels": [
"Peanut-Free",
"Tree-Nut-Free",
"Alcohol-Free"
],
"cautions": [
"Sulfites",
"FODMAP"
],
"ingredientLines": [
"1 chicken, about 3.5 to 4 pounds",
"1 lemon",
"1 blood orange",
"1 tangerine or clementine",
"Kosher salt",
"1/2 cup chicken broth"
],
"ingredients": [
{
"text": "1 chicken, about 3.5 to 4 pounds",
"weight": 1700.9713875
},
{
"text": "1 lemon",
"weight": 58
},
{
"text": "1 blood orange",
"weight": 131
},
{
"text": "1 tangerine or clementine",
"weight": 74
},
{
"text": "Kosher salt",
"weight": 12.503828324999999
},
{
"text": "1/2 cup chicken broth",
"weight": 120
}
],
"calories": 2643.1901685250004,
"totalWeight": 2093.938546284647,
"totalTime": 424,
"totalNutrients": {
"ENERC_KCAL": {
"label": "Energy",
"quantity": 2643.1901685250004,
"unit": "kcal"
},
"FAT": {
"label": "Fat",
"quantity": 176.07527785109997,
"unit": "g"
},
"FASAT": {
"label": "Saturated",
"quantity": 50.27953942484999,
"unit": "g"
},
"FATRN": {
"label": "Trans",
"quantity": 1.121960727195,
"unit": "g"
},
"FAMS": {
"label": "Monounsaturated",
"quantity": 72.91052791439999,
"unit": "g"
},
"FAPU": {
"label": "Polyunsaturated",
"quantity": 37.70010555505,
"unit": "g"
},
"CHOCDF": {
"label": "Carbs",
"quantity": 33.9289,
"unit": "g"
},
"FIBTG": {
"label": "Fiber",
"quantity": 6.026,
"unit": "g"
},
"SUGAR": {
"label": "Sugars",
"quantity": 22.3877,
"unit": "g"
},
"PROCNT": {
"label": "Protein",
"quantity": 220.661261091,
"unit": "g"
},
"CHOLE": {
"label": "Cholesterol",
"quantity": 871.095407625,
"unit": "mg"
},
"NA": {
"label": "Sodium",
"quantity": 4846.2337822035,
"unit": "mg"
},
"CA": {
"label": "Calcium",
"quantity": 222.90477789331527,
"unit": "mg"
},
"MG": {
"label": "Magnesium",
"quantity": 261.37178028784643,
"unit": "mg"
},
"K": {
"label": "Potassium",
"quantity": 2761.015799917772,
"unit": "mg"
},
"FE": {
"label": "Iron",
"quantity": 11.277436515489338,
"unit": "mg"
},
"ZN": {
"label": "Zinc",
"quantity": 15.501120278634646,
"unit": "mg"
},
"P": {
"label": "Phosphorus",
"quantity": 1775.850998945,
"unit": "mg"
},
"VITA_RAE": {
"label": "Vitamin A",
"quantity": 490.42082283499997,
"unit": "µg"
},
"VITC": {
"label": "Vitamin C",
"quantity": 155.290568696,
"unit": "mg"
},
"THIA": {
"label": "Thiamin (B1)",
"quantity": 0.9368063261,
"unit": "mg"
},
"RIBF": {
"label": "Riboflavin (B2)",
"quantity": 1.5761926522,
"unit": "mg"
},
"NIA": {
"label": "Niacin (B3)",
"quantity": 81.46334356343502,
"unit": "mg"
},
"VITB6A": {
"label": "Vitamin B6",
"quantity": 4.30201190225,
"unit": "mg"
},
"FOLDFE": {
"label": "Folate equivalent (total)",
"quantity": 138.83963261,
"unit": "µg"
},
"FOLFD": {
"label": "Folate (food)",
"quantity": 138.83963261,
"unit": "µg"
},
"VITB12": {
"label": "Vitamin B12",
"quantity": 3.58564768485,
"unit": "µg"
},
"VITD": {
"label": "Vitamin D",
"quantity": 2.313321087,
"unit": "µg"
},
"TOCPHA": {
"label": "Vitamin E",
"quantity": 3.9767816305000006,
"unit": "mg"
},
"VITK1": {
"label": "Vitamin K",
"quantity": 17.589908152499998,
"unit": "µg"
}
},
"totalDaily": {
"ENERC_KCAL": {
"label": "Energy",
"quantity": 132.15950842625003,
"unit": "%"
},
"FAT": {
"label": "Fat",
"quantity": 270.8850428478461,
"unit": "%"
},
"FASAT": {
"label": "Saturated",
"quantity": 251.39769712424996,
"unit": "%"
},
"CHOCDF": {
"label": "Carbs",
"quantity": 11.309633333333332,
"unit": "%"
},
"FIBTG": {
"label": "Fiber",
"quantity": 24.104,
"unit": "%"
},
"PROCNT": {
"label": "Protein",
"quantity": 441.32252218200006,
"unit": "%"
},
"CHOLE": {
"label": "Cholesterol",
"quantity": 290.36513587499996,
"unit": "%"
},
"NA": {
"label": "Sodium",
"quantity": 201.92640759181248,
"unit": "%"
},
"CA": {
"label": "Calcium",
"quantity": 22.290477789331526,
"unit": "%"
},
"MG": {
"label": "Magnesium",
"quantity": 62.23137625901106,
"unit": "%"
},
"K": {
"label": "Potassium",
"quantity": 58.74501701952706,
"unit": "%"
},
"FE": {
"label": "Iron",
"quantity": 62.65242508605187,
"unit": "%"
},
"ZN": {
"label": "Zinc",
"quantity": 140.91927526031498,
"unit": "%"
},
"P": {
"label": "Phosphorus",
"quantity": 253.69299984928568,
"unit": "%"
},
"VITA_RAE": {
"label": "Vitamin A",
"quantity": 54.49120253722222,
"unit": "%"
},
"VITC": {
"label": "Vitamin C",
"quantity": 172.5450763288889,
"unit": "%"
},
"THIA": {
"label": "Thiamin (B1)",
"quantity": 78.06719384166668,
"unit": "%"
},
"RIBF": {
"label": "Riboflavin (B2)",
"quantity": 121.24558863076923,
"unit": "%"
},
"NIA": {
"label": "Niacin (B3)",
"quantity": 509.14589727146887,
"unit": "%"
},
"VITB6A": {
"label": "Vitamin B6",
"quantity": 330.92399248076924,
"unit": "%"
},
"FOLDFE": {
"label": "Folate equivalent (total)",
"quantity": 34.7099081525,
"unit": "%"
},
"VITB12": {
"label": "Vitamin B12",
"quantity": 149.40198686875001,
"unit": "%"
},
"VITD": {
"label": "Vitamin D",
"quantity": 15.422140579999999,
"unit": "%"
},
"TOCPHA": {
"label": "Vitamin E",
"quantity": 26.51187753666667,
"unit": "%"
},
"VITK1": {
"label": "Vitamin K",
"quantity": 14.658256793749997,
"unit": "%"
}
},
"digest": [
{
"label": "Fat",
"tag": "FAT",
"schemaOrgTag": "fatContent",
"total": 176.07527785109997,
"hasRDI": true,
"daily": 270.8850428478461,
"unit": "g",
"sub": [
{
"label": "Saturated",
"tag": "FASAT",
"schemaOrgTag": "saturatedFatContent",
"total": 50.27953942484999,
"hasRDI": true,
"daily": 251.39769712424996,
"unit": "g"
},
{
"label": "Trans",
"tag": "FATRN",
"schemaOrgTag": "transFatContent",
"total": 1.121960727195,
"hasRDI": false,
"daily": 0,
"unit": "g"
},
{
"label": "Monounsaturated",
"tag": "FAMS",
"schemaOrgTag": null,
"total": 72.91052791439999,
"hasRDI": false,
"daily": 0,
"unit": "g"
},
{
"label": "Polyunsaturated",
"tag": "FAPU",
"schemaOrgTag": null,
"total": 37.70010555505,
"hasRDI": false,
"daily": 0,
"unit": "g"
}
]
},
{
"label": "Carbs",
"tag": "CHOCDF",
"schemaOrgTag": "carbohydrateContent",
"total": 33.9289,
"hasRDI": true,
"daily": 11.309633333333332,
"unit": "g",
"sub": [
{
"label": "Carbs (net)",
"tag": "CHOCDF.net",
"schemaOrgTag": null,
"total": 27.9029,
"hasRDI": false,
"daily": 0,
"unit": "g"
},
{
"label": "Fiber",
"tag": "FIBTG",
"schemaOrgTag": "fiberContent",
"total": 6.026,
"hasRDI": true,
"daily": 24.104,
"unit": "g"
},
{
"label": "Sugars",
"tag": "SUGAR",
"schemaOrgTag": "sugarContent",
"total": 22.3877,
"hasRDI": false,
"daily": 0,
"unit": "g"
},
{
"label": "Sugars, added",
"tag": "SUGAR.added",
"schemaOrgTag": null,
"total": 0,
"hasRDI": false,
"daily": 0,
"unit": "g"
}
]
},
{
"label": "Protein",
"tag": "PROCNT",
"schemaOrgTag": "proteinContent",
"total": 220.661261091,
"hasRDI": true,
"daily": 441.32252218200006,
"unit": "g"
},
{
"label": "Cholesterol",
"tag": "CHOLE",
"schemaOrgTag": "cholesterolContent",
"total": 871.095407625,
"hasRDI": true,
"daily": 290.36513587499996,
"unit": "mg"
},
{
"label": "Sodium",
"tag": "NA",
"schemaOrgTag": "sodiumContent",
"total": 4846.2337822035,
"hasRDI": true,
"daily": 201.92640759181248,
"unit": "mg"
},
{
"label": "Calcium",
"tag": "CA",
"schemaOrgTag": null,
"total": 222.90477789331527,
"hasRDI": true,
"daily": 22.290477789331526,
"unit": "mg"
},
{
"label": "Magnesium",
"tag": "MG",
"schemaOrgTag": null,
"total": 261.37178028784643,
"hasRDI": true,
"daily": 62.23137625901106,
"unit": "mg"
},
{
"label": "Potassium",
"tag": "K",
"schemaOrgTag": null,
"total": 2761.015799917772,
"hasRDI": true,
"daily": 58.74501701952706,
"unit": "mg"
},
{
"label": "Iron",
"tag": "FE",
"schemaOrgTag": null,
"total": 11.277436515489338,
"hasRDI": true,
"daily": 62.65242508605187,
"unit": "mg"
},
{
"label": "Zinc",
"tag": "ZN",
"schemaOrgTag": null,
"total": 15.501120278634646,
"hasRDI": true,
"daily": 140.91927526031498,
"unit": "mg"
},
{
"label": "Phosphorus",
"tag": "P",
"schemaOrgTag": null,
"total": 1775.850998945,
"hasRDI": true,
"daily": 253.69299984928568,
"unit": "mg"
},
{
"label": "Vitamin A",
"tag": "VITA_RAE",
"schemaOrgTag": null,
"total": 490.42082283499997,
"hasRDI": true,
"daily": 54.49120253722222,
"unit": "µg"
},
{
"label": "Vitamin C",
"tag": "VITC",
"schemaOrgTag": null,
"total": 155.290568696,
"hasRDI": true,
"daily": 172.5450763288889,
"unit": "mg"
},
{
"label": "Thiamin (B1)",
"tag": "THIA",
"schemaOrgTag": null,
"total": 0.9368063261,
"hasRDI": true,
"daily": 78.06719384166668,
"unit": "mg"
},
{
"label": "Riboflavin (B2)",
"tag": "RIBF",
"schemaOrgTag": null,
"total": 1.5761926522,
"hasRDI": true,
"daily": 121.24558863076923,
"unit": "mg"
},
{
"label": "Niacin (B3)",
"tag": "NIA",
"schemaOrgTag": null,
"total": 81.46334356343502,
"hasRDI": true,
"daily": 509.14589727146887,
"unit": "mg"
},
{
"label": "Vitamin B6",
"tag": "VITB6A",
"schemaOrgTag": null,
"total": 4.30201190225,
"hasRDI": true,
"daily": 330.92399248076924,
"unit": "mg"
},
{
"label": "Folate equivalent (total)",
"tag": "FOLDFE",
"schemaOrgTag": null,
"total": 138.83963261,
"hasRDI": true,
"daily": 34.7099081525,
"unit": "µg"
},
{
"label": "Folate (food)",
"tag": "FOLFD",
"schemaOrgTag": null,
"total": 138.83963261,
"hasRDI": false,
"daily": 0,
"unit": "µg"
},
{
"label": "Folic acid",
"tag": "FOLAC",
"schemaOrgTag": null,
"total": 0,
"hasRDI": false,
"daily": 0,
"unit": "µg"
},
{
"label": "Vitamin B12",
"tag": "VITB12",
"schemaOrgTag": null,
"total": 3.58564768485,
"hasRDI": true,
"daily": 149.40198686875001,
"unit": "µg"
},
{
"label": "Vitamin D",
"tag": "VITD",
"schemaOrgTag": null,
"total": 2.313321087,
"hasRDI": true,
"daily": 15.422140579999999,
"unit": "µg"
},
{
"label": "Vitamin E",
"tag": "TOCPHA",
"schemaOrgTag": null,
"total": 3.9767816305000006,
"hasRDI": true,
"daily": 26.51187753666667,
"unit": "mg"
},
{
"label": "Vitamin K",
"tag": "VITK1",
"schemaOrgTag": null,
"total": 17.589908152499998,
"hasRDI": true,
"daily": 14.658256793749997,
"unit": "µg"
}
]
},
"bookmarked": false,
"bought": false
},
{
"recipe": {
"uri": "http://www.edamam.com/ontologies/edamam.owl#recipe_56008870a1e326be7851141fc49bd53e",
"label": "Roast Chicken",
"image": "https://www.edamam.com/web-img/c24/c24a86f98a8cc1f13f795bdba2dae614.jpg",
"source": "Epicurious",
"url": "http://www.epicurious.com/recipes/food/views/Roast-Chicken-394676",
"shareAs": "http://www.edamam.com/recipe/roast-chicken-56008870a1e326be7851141fc49bd53e/chicken/alcohol-free/591-722-cal",
"yield": 4,
"dietLabels": [
"Low-Carb"
],
"healthLabels": [
"Sugar-Conscious",
"Peanut-Free",
"Tree-Nut-Free",
"Alcohol-Free"
],
"cautions": [],
"ingredientLines": [
"1 tablespoon kosher salt",
"1 whole 4-pound chicken, giblets reserved for another use",
"1/4 cup (1/2 stick) unsalted butter, melted"
],
"ingredients": [
{
"text": "1 tablespoon kosher salt",
"weight": 14.562499999753793
},
{
"text": "1 whole 4-pound chicken, giblets reserved for another use",
"weight": 920
},
{
"text": "1/4 cup (1/2 stick) unsalted butter, melted",
"weight": 56.75
}
],
"calories": 2384.8975,
"totalWeight": 980.9328012023324,
"totalTime": 320,
"totalNutrients": {
"ENERC_KCAL": {
"label": "Energy",
"quantity": 2384.8975,
"unit": "kcal"
},
"FAT": {
"label": "Fat",
"quantity": 184.581925,
"unit": "g"
},
"FASAT": {
"label": "Saturated",
"quantity": 68.80334,
"unit": "g"
},
"FATRN": {
"label": "Trans",
"quantity": 2.7526650000000004,
"unit": "g"
},
"FAMS": {
"label": "Monounsaturated",
"quantity": 69.33741750000002,
"unit": "g"
},
"FAPU": {
"label": "Polyunsaturated",
"quantity": 31.442902500000006,
"unit": "g"
},
"CHOCDF": {
"label": "Carbs",
"quantity": 0.03405,
"unit": "g"
},
"SUGAR": {
"label": "Sugars",
"quantity": 0.03405,
"unit": "g"
},
"PROCNT": {
"label": "Protein",
"quantity": 171.60237500000002,
"unit": "g"
},
"CHOLE": {
"label": "Cholesterol",
"quantity": 812.0125000000002,
"unit": "mg"
},
"NA": {
"label": "Sodium",
"quantity": 2271.4125900000004,
"unit": "mg"
},
"CA": {
"label": "Calcium",
"quantity": 115.8238722885598,
"unit": "mg"
},
"MG": {
"label": "Magnesium",
"quantity": 185.17682801202335,
"unit": "mg"
},
"K": {
"label": "Potassium",
"quantity": 1752.7546240961867,
"unit": "mg"
},
"FE": {
"label": "Iron",
"quantity": 8.305153243967698,
"unit": "mg"
},
"ZN": {
"label": "Zinc",
"quantity": 12.107257801202335,
"unit": "mg"
},
"P": {
"label": "Phosphorus",
"quantity": 1366.02,
"unit": "mg"
},
"VITA_RAE": {
"label": "Vitamin A",
"quantity": 765.3700000000001,
"unit": "µg"
},
"VITC": {
"label": "Vitamin C",
"quantity": 14.720000000000002,
"unit": "mg"
},
"THIA": {
"label": "Thiamin (B1)",
"quantity": 0.5548375000000001,
"unit": "mg"
},
"RIBF": {
"label": "Riboflavin (B2)",
"quantity": 1.1232950000000002,
"unit": "mg"
},
"NIA": {
"label": "Niacin (B3)",
"quantity": 62.59303500000001,
"unit": "mg"
},
"VITB6A": {
"label": "Vitamin B6",
"quantity": 3.2217025,
"unit": "mg"
},
"FOLDFE": {
"label": "Folate equivalent (total)",
"quantity": 56.9025,
"unit": "µg"
},
"FOLFD": {
"label": "Folate (food)",
"quantity": 56.9025,
"unit": "µg"
},
"VITB12": {
"label": "Vitamin B12",
"quantity": 2.948475,
"unit": "µg"
},
"VITD": {
"label": "Vitamin D",
"quantity": 2.69125,
"unit": "µg"
},
"TOCPHA": {
"label": "Vitamin E",
"quantity": 4.0766,
"unit": "mg"
},
"VITK1": {
"label": "Vitamin K",
"quantity": 17.7725,
"unit": "µg"
}
},
"totalDaily": {
"ENERC_KCAL": {
"label": "Energy",
"quantity": 119.244875,
"unit": "%"
},
"FAT": {
"label": "Fat",
"quantity": 283.9721923076923,
"unit": "%"
},
"FASAT": {
"label": "Saturated",
"quantity": 344.0167,
"unit": "%"
},
"CHOCDF": {
"label": "Carbs",
"quantity": 0.011349999999999999,
"unit": "%"
},
"PROCNT": {
"label": "Protein",
"quantity": 343.20475000000005,
"unit": "%"
},
"CHOLE": {
"label": "Cholesterol",
"quantity": 270.6708333333334,
"unit": "%"
},
"NA": {
"label": "Sodium",
"quantity": 94.64219125000002,
"unit": "%"
},
"CA": {
"label": "Calcium",
"quantity": 11.58238722885598,
"unit": "%"
},
"MG": {
"label": "Magnesium",
"quantity": 44.089720955243656,
"unit": "%"
},
"K": {
"label": "Potassium",
"quantity": 37.29265157651461,
"unit": "%"
},
"FE": {
"label": "Iron",
"quantity": 46.13974024426499,
"unit": "%"
},
"ZN": {
"label": "Zinc",
"quantity": 110.06598001093033,
"unit": "%"
},
"P": {
"label": "Phosphorus",
"quantity": 195.1457142857143,
"unit": "%"
},
"VITA_RAE": {
"label": "Vitamin A",
"quantity": 85.04111111111112,
"unit": "%"
},
"VITC": {
"label": "Vitamin C",
"quantity": 16.355555555555558,
"unit": "%"
},
"THIA": {
"label": "Thiamin (B1)",
"quantity": 46.23645833333334,
"unit": "%"
},
"RIBF": {
"label": "Riboflavin (B2)",
"quantity": 86.4073076923077,
"unit": "%"
},
"NIA": {
"label": "Niacin (B3)",
"quantity": 391.20646875000006,
"unit": "%"
},
"VITB6A": {
"label": "Vitamin B6",
"quantity": 247.82326923076923,
"unit": "%"
},
"FOLDFE": {
"label": "Folate equivalent (total)",
"quantity": 14.225625,
"unit": "%"
},
"VITB12": {
"label": "Vitamin B12",
"quantity": 122.85312500000002,
"unit": "%"
},
"VITD": {
"label": "Vitamin D",
"quantity": 17.941666666666666,
"unit": "%"
},
"TOCPHA": {
"label": "Vitamin E",
"quantity": 27.177333333333333,
"unit": "%"
},
"VITK1": {
"label": "Vitamin K",
"quantity": 14.810416666666667,
"unit": "%"
}
},
"digest": [
{
"label": "Fat",
"tag": "FAT",
"schemaOrgTag": "fatContent",
"total": 184.581925,
"hasRDI": true,
"daily": 283.9721923076923,
"unit": "g",
"sub": [
{
"label": "Saturated",
"tag": "FASAT",
"schemaOrgTag": "saturatedFatContent",
"total": 68.80334,
"hasRDI": true,
"daily": 344.0167,
"unit": "g"
},
{
"label": "Trans",
"tag": "FATRN",
"schemaOrgTag": "transFatContent",
"total": 2.7526650000000004,
"hasRDI": false,
"daily": 0,
"unit": "g"
},
{
"label": "Monounsaturated",
"tag": "FAMS",
"schemaOrgTag": null,
"total": 69.33741750000002,
"hasRDI": false,
"daily": 0,
"unit": "g"
},
{
"label": "Polyunsaturated",
"tag": "FAPU",
"schemaOrgTag": null,
"total": 31.442902500000006,
"hasRDI": false,
"daily": 0,
"unit": "g"
}
]
},
{
"label": "Carbs",
"tag": "CHOCDF",
"schemaOrgTag": "carbohydrateContent",
"total": 0.03405,
"hasRDI": true,
"daily": 0.011349999999999999,
"unit": "g",
"sub": [
{
"label": "Carbs (net)",
"tag": "CHOCDF.net",
"schemaOrgTag": null,
"total": 0.03405,
"hasRDI": false,
"daily": 0,
"unit": "g"
},
{
"label": "Fiber",
"tag": "FIBTG",
"schemaOrgTag": "fiberContent",
"total": 0,
"hasRDI": false,
"daily": 0,
"unit": "g"
},
{
"label": "Sugars",
"tag": "SUGAR",
"schemaOrgTag": "sugarContent",
"total": 0.03405,
"hasRDI": false,
"daily": 0,
"unit": "g"
},
{
"label": "Sugars, added",
"tag": "SUGAR.added",
"schemaOrgTag": null,
"total": 0,
"hasRDI": false,
"daily": 0,
"unit": "g"
}
]
},
{
"label": "Protein",
"tag": "PROCNT",
"schemaOrgTag": "proteinContent",
"total": 171.60237500000002,
"hasRDI": true,
"daily": 343.20475000000005,
"unit": "g"
},
{
"label": "Cholesterol",
"tag": "CHOLE",
"schemaOrgTag": "cholesterolContent",
"total": 812.0125000000002,
"hasRDI": true,
"daily": 270.6708333333334,
"unit": "mg"
},
{
"label": "Sodium",
"tag": "NA",
"schemaOrgTag": "sodiumContent",
"total": 2271.4125900000004,
"hasRDI": true,
"daily": 94.64219125000002,
"unit": "mg"
},
{
"label": "Calcium",
"tag": "CA",
"schemaOrgTag": null,
"total": 115.8238722885598,
"hasRDI": true,
"daily": 11.58238722885598,
"unit": "mg"
},
{
"label": "Magnesium",
"tag": "MG",
"schemaOrgTag": null,
"total": 185.17682801202335,
"hasRDI": true,
"daily": 44.089720955243656,
"unit": "mg"
},
{
"label": "Potassium",
"tag": "K",
"schemaOrgTag": null,
"total": 1752.7546240961867,
"hasRDI": true,
"daily": 37.29265157651461,
"unit": "mg"
},
{
"label": "Iron",
"tag": "FE",
"schemaOrgTag": null,
"total": 8.305153243967698,
"hasRDI": true,
"daily": 46.13974024426499,
"unit": "mg"
},
{
"label": "Zinc",
"tag": "ZN",
"schemaOrgTag": null,
"total": 12.107257801202335,
"hasRDI": true,
"daily": 110.06598001093033,
"unit": "mg"
},
{
"label": "Phosphorus",
"tag": "P",
"schemaOrgTag": null,
"total": 1366.02,
"hasRDI": true,
"daily": 195.1457142857143,
"unit": "mg"
},
{
"label": "Vitamin A",
"tag": "VITA_RAE",
"schemaOrgTag": null,
"total": 765.3700000000001,
"hasRDI": true,
"daily": 85.04111111111112,
"unit": "µg"
},
{
"label": "Vitamin C",
"tag": "VITC",
"schemaOrgTag": null,
"total": 14.720000000000002,
"hasRDI": true,
"daily": 16.355555555555558,
"unit": "mg"
},
{
"label": "Thiamin (B1)",
"tag": "THIA",
"schemaOrgTag": null,
"total": 0.5548375000000001,
"hasRDI": true,
"daily": 46.23645833333334,
"unit": "mg"
},
{
"label": "Riboflavin (B2)",
"tag": "RIBF",
"schemaOrgTag": null,
"total": 1.1232950000000002,
"hasRDI": true,
"daily": 86.4073076923077,
"unit": "mg"
},
{
"label": "Niacin (B3)",
"tag": "NIA",
"schemaOrgTag": null,
"total": 62.59303500000001,
"hasRDI": true,
"daily": 391.20646875000006,
"unit": "mg"
},
{
"label": "Vitamin B6",
"tag": "VITB6A",
"schemaOrgTag": null,
"total": 3.2217025,
"hasRDI": true,
"daily": 247.82326923076923,
"unit": "mg"
},
{
"label": "Folate equivalent (total)",
"tag": "FOLDFE",
"schemaOrgTag": null,
"total": 56.9025,
"hasRDI": true,
"daily": 14.225625,
"unit": "µg"
},
{
"label": "Folate (food)",
"tag": "FOLFD",
"schemaOrgTag": null,
"total": 56.9025,
"hasRDI": false,
"daily": 0,
"unit": "µg"
},
{
"label": "Folic acid",
"tag": "FOLAC",
"schemaOrgTag": null,
"total": 0,
"hasRDI": false,
"daily": 0,
"unit": "µg"
},
{
"label": "Vitamin B12",
"tag": "VITB12",
"schemaOrgTag": null,
"total": 2.948475,
"hasRDI": true,
"daily": 122.85312500000002,
"unit": "µg"
},
{
"label": "Vitamin D",
"tag": "VITD",
"schemaOrgTag": null,
"total": 2.69125,
"hasRDI": true,
"daily": 17.941666666666666,
"unit": "µg"
},
{
"label": "Vitamin E",
"tag": "TOCPHA",
"schemaOrgTag": null,
"total": 4.0766,
"hasRDI": true,
"daily": 27.177333333333333,
"unit": "mg"
},
{
"label": "Vitamin K",
"tag": "VITK1",
"schemaOrgTag": null,
"total": 17.7725,
"hasRDI": true,
"daily": 14.810416666666667,
"unit": "µg"
}
]
},
"bookmarked": false,
"bought": false
},
{
"recipe": {
"uri": "http://www.edamam.com/ontologies/edamam.owl#recipe_95fa6f5689286a4ffab774da45192494",
"label": "Thomato Chicken",
"image": "https://www.edamam.com/web-img/561/56100df8491403ea215cea3c782faec9.jpg",
"source": "BBC Good Food",
"url": "http://www.bbcgoodfood.com/recipes/94602/thomato-chicken",
"shareAs": "http://www.edamam.com/recipe/thomato-chicken-95fa6f5689286a4ffab774da45192494/chicken/alcohol-free/591-722-cal",
"yield": 3,
"dietLabels": [
"Low-Carb"
],
"healthLabels": [
"Peanut-Free",
"Tree-Nut-Free",
"Alcohol-Free"
],
"cautions": [
"Sulfites"
],
"ingredientLines": [
"2 chicken breasts",
"2 tsp capers",
"1 large onion",
"6 cherry tomatoes",
"1.5 tsp oregano",
"3 tsps of tomato puree",
"1 red pepper",
"1 tin chopped tomatoes",
"5 sun-dried tomatoes",
"1 tsp basil",
"Salt and pepper to taste",
"Olive oil for frying chicken"
],
"ingredients": [
{
"text": "2 chicken breasts",
"weight": 348
},
{
"text": "2 tsp capers",
"weight": 4.733333333573413
},
{
"text": "1 large onion",
"weight": 150
},
{
"text": "6 cherry tomatoes",
"weight": 90
},
{
"text": "1.5 tsp oregano",
"weight": 1.5
},
{
"text": "3 tsps of tomato puree",
"weight": 15.125000000767159
},
{
"text": "1 red pepper",
"weight": 119
},
{
"text": "1 tin chopped tomatoes",
"weight": 190
},
{
"text": "5 sun-dried tomatoes",
"weight": 10
},
{
"text": "1 tsp basil",
"weight": 0.5000000000253606
},
{
"text": "Salt and pepper to taste",
"weight": 5.573150000006196
},
{
"text": "Salt and pepper to taste",
"weight": 2.786575000003098
},
{
"text": "Olive oil for frying chicken",
"weight": 12.632473333347377
}
],
"calories": 2027.6141152683626,
"totalWeight": 1077.0594163082444,
"totalTime": 0,
"totalNutrients": {
"ENERC_KCAL": {
"label": "Energy",
"quantity": 2027.6141152683626,
"unit": "kcal"
},
"FAT": {
"label": "Fat",
"quantity": 174.47300776182743,
"unit": "g"
},
"FASAT": {
"label": "Saturated",
"quantity": 28.975328214889167,
"unit": "g"
},
"FATRN": {
"label": "Trans",
"quantity": 0.3654,
"unit": "g"
},
"FAMS": {
"label": "Monounsaturated",
"quantity": 116.08107867045206,
"unit": "g"
},
"FAPU": {
"label": "Polyunsaturated",
"quantity": 22.182989043614004,
"unit": "g"
},
"CHOCDF": {
"label": "Carbs",
"quantity": 41.018837212570325,
"unit": "g"
},
"FIBTG": {
"label": "Fiber",
"quantity": 12.758345141690114,
"unit": "g"
},
"SUGAR": {
"label": "Sugars",
"quantity": 23.094590746701503,
"unit": "g"
},
"PROCNT": {
"label": "Protein",
"quantity": 79.89013180918606,
"unit": "g"
},
"CHOLE": {
"label": "Cholesterol",
"quantity": 222.72,
"unit": "mg"
},
"NA": {
"label": "Sodium",
"quantity": 2493.4438789777223,
"unit": "mg"
},
"CA": {
"label": "Calcium",
"quantity": 210.59581948494295,
"unit": "mg"
},
"MG": {
"label": "Magnesium",
"quantity": 178.35036124249137,
"unit": "mg"
},
"K": {
"label": "Potassium",
"quantity": 2260.0005361111926,
"unit": "mg"
},
"FE": {
"label": "Iron",
"quantity": 7.5542062056209005,
"unit": "mg"
},
"ZN": {
"label": "Zinc",
"quantity": 4.054876208393468,
"unit": "mg"
},
"P": {
"label": "Phosphorus",
"quantity": 781.676121833622,
"unit": "mg"
},
"VITA_RAE": {
"label": "Vitamin A",
"quantity": 355.89245858350233,
"unit": "µg"
},
"VITC": {
"label": "Vitamin C",
"quantity": 204.97253333341877,
"unit": "mg"
},
"THIA": {
"label": "Thiamin (B1)",
"quantity": 1.5491302510006304,
"unit": "mg"
},
"RIBF": {
"label": "Riboflavin (B2)",
"quantity": 0.6357101683340908,
"unit": "mg"
},
"NIA": {
"label": "Niacin (B3)",
"quantity": 38.93289938559454,
"unit": "mg"
},
"VITB6A": {
"label": "Vitamin B6",
"quantity": 2.7351100999179208,
"unit": "mg"
},
"FOLDFE": {
"label": "Folate equivalent (total)",
"quantity": 140.0836344168394,
"unit": "µg"
},
"FOLFD": {
"label": "Folate (food)",
"quantity": 140.0836344168394,
"unit": "µg"
},
"VITB12": {
"label": "Vitamin B12",
"quantity": 1.1832,
"unit": "µg"
},
"VITD": {
"label": "Vitamin D",
"quantity": 1.3920000000000001,
"unit": "µg"
},
"TOCPHA": {
"label": "Vitamin E",
"quantity": 25.169014918992694,
"unit": "mg"
},
"VITK1": {
"label": "Vitamin K",
"quantity": 125.33893894280406,
"unit": "µg"
}
},
"totalDaily": {
"ENERC_KCAL": {
"label": "Energy",
"quantity": 101.38070576341812,
"unit": "%"
},
"FAT": {
"label": "Fat",
"quantity": 268.42001194127295,
"unit": "%"
},
"FASAT": {
"label": "Saturated",
"quantity": 144.87664107444584,
"unit": "%"
},
"CHOCDF": {
"label": "Carbs",
"quantity": 13.672945737523442,
"unit": "%"
},
"FIBTG": {
"label": "Fiber",
"quantity": 51.033380566760464,
"unit": "%"
},
"PROCNT": {
"label": "Protein",
"quantity": 159.78026361837212,
"unit": "%"
},
"CHOLE": {
"label": "Cholesterol",
"quantity": 74.24,
"unit": "%"
},
"NA": {
"label": "Sodium",
"quantity": 103.8934949574051,
"unit": "%"
},
"CA": {
"label": "Calcium",
"quantity": 21.059581948494294,
"unit": "%"
},
"MG": {
"label": "Magnesium",
"quantity": 42.46437172440271,
"unit": "%"
},
"K": {
"label": "Potassium",
"quantity": 48.08511778959984,
"unit": "%"
},
"FE": {
"label": "Iron",
"quantity": 41.96781225344945,
"unit": "%"
},
"ZN": {
"label": "Zinc",
"quantity": 36.86251098539516,
"unit": "%"
},
"P": {
"label": "Phosphorus",
"quantity": 111.66801740480315,
"unit": "%"
},
"VITA_RAE": {
"label": "Vitamin A",
"quantity": 39.543606509278035,
"unit": "%"
},
"VITC": {
"label": "Vitamin C",
"quantity": 227.74725925935417,
"unit": "%"
},
"THIA": {
"label": "Thiamin (B1)",
"quantity": 129.09418758338586,
"unit": "%"
},
"RIBF": {
"label": "Riboflavin (B2)",
"quantity": 48.90078217954544,
"unit": "%"
},
"NIA": {
"label": "Niacin (B3)",
"quantity": 243.33062115996586,
"unit": "%"
},
"VITB6A": {
"label": "Vitamin B6",
"quantity": 210.39308460907083,
"unit": "%"
},
"FOLDFE": {
"label": "Folate equivalent (total)",
"quantity": 35.02090860420985,
"unit": "%"
},
"VITB12": {
"label": "Vitamin B12",
"quantity": 49.300000000000004,
"unit": "%"
},
"VITD": {
"label": "Vitamin D",
"quantity": 9.280000000000001,
"unit": "%"
},
"TOCPHA": {
"label": "Vitamin E",
"quantity": 167.7934327932846,
"unit": "%"
},
"VITK1": {
"label": "Vitamin K",
"quantity": 104.44911578567006,
"unit": "%"
}
},
"digest": [
{
"label": "Fat",
"tag": "FAT",
"schemaOrgTag": "fatContent",
"total": 174.47300776182743,
"hasRDI": true,
"daily": 268.42001194127295,
"unit": "g",
"sub": [
{
"label": "Saturated",
"tag": "FASAT",
"schemaOrgTag": "saturatedFatContent",
"total": 28.975328214889167,
"hasRDI": true,
"daily": 144.87664107444584,
"unit": "g"
},
{
"label": "Trans",
"tag": "FATRN",
"schemaOrgTag": "transFatContent",
"total": 0.3654,
"hasRDI": false,
"daily": 0,
"unit": "g"
},
{
"label": "Monounsaturated",
"tag": "FAMS",
"schemaOrgTag": null,
"total": 116.08107867045206,
"hasRDI": false,
"daily": 0,
"unit": "g"
},
{
"label": "Polyunsaturated",
"tag": "FAPU",
"schemaOrgTag": null,
"total": 22.182989043614004,
"hasRDI": false,
"daily": 0,
"unit": "g"
}
]
},
{
"label": "Carbs",
"tag": "CHOCDF",
"schemaOrgTag": "carbohydrateContent",
"total": 41.018837212570325,
"hasRDI": true,
"daily": 13.672945737523442,
"unit": "g",
"sub": [
{
"label": "Carbs (net)",
"tag": "CHOCDF.net",
"schemaOrgTag": null,
"total": 28.26049207088021,
"hasRDI": false,
"daily": 0,
"unit": "g"
},
{
"label": "Fiber",
"tag": "FIBTG",
"schemaOrgTag": "fiberContent",
"total": 12.758345141690114,
"hasRDI": true,
"daily": 51.033380566760464,
"unit": "g"
},
{
"label": "Sugars",
"tag": "SUGAR",
"schemaOrgTag": "sugarContent",
"total": 23.094590746701503,
"hasRDI": false,
"daily": 0,
"unit": "g"
},
{
"label": "Sugars, added",
"tag": "SUGAR.added",
"schemaOrgTag": null,
"total": 0,
"hasRDI": false,
"daily": 0,
"unit": "g"
}
]
},
{
"label": "Protein",
"tag": "PROCNT",
"schemaOrgTag": "proteinContent",
"total": 79.89013180918606,
"hasRDI": true,
"daily": 159.78026361837212,
"unit": "g"
},
{
"label": "Cholesterol",
"tag": "CHOLE",
"schemaOrgTag": "cholesterolContent",
"total": 222.72,
"hasRDI": true,
"daily": 74.24,
"unit": "mg"
},
{
"label": "Sodium",
"tag": "NA",
"schemaOrgTag": "sodiumContent",
"total": 2493.4438789777223,
"hasRDI": true,
"daily": 103.8934949574051,
"unit": "mg"
},
{
"label": "Calcium",
"tag": "CA",
"schemaOrgTag": null,
"total": 210.59581948494295,
"hasRDI": true,
"daily": 21.059581948494294,
"unit": "mg"
},
{
"label": "Magnesium",
"tag": "MG",
"schemaOrgTag": null,
"total": 178.35036124249137,
"hasRDI": true,
"daily": 42.46437172440271,
"unit": "mg"
},
{
"label": "Potassium",
"tag": "K",
"schemaOrgTag": null,
"total": 2260.0005361111926,
"hasRDI": true,
"daily": 48.08511778959984,
"unit": "mg"
},
{
"label": "Iron",
"tag": "FE",
"schemaOrgTag": null,
"total": 7.5542062056209005,
"hasRDI": true,
"daily": 41.96781225344945,
"unit": "mg"
},
{
"label": "Zinc",
"tag": "ZN",
"schemaOrgTag": null,
"total": 4.054876208393468,
"hasRDI": true,
"daily": 36.86251098539516,
"unit": "mg"
},
{
"label": "Phosphorus",
"tag": "P",
"schemaOrgTag": null,
"total": 781.676121833622,
"hasRDI": true,
"daily": 111.66801740480315,
"unit": "mg"
},
{
"label": "Vitamin A",
"tag": "VITA_RAE",
"schemaOrgTag": null,
"total": 355.89245858350233,
"hasRDI": true,
"daily": 39.543606509278035,
"unit": "µg"
},
{
"label": "Vitamin C",
"tag": "VITC",
"schemaOrgTag": null,
"total": 204.97253333341877,
"hasRDI": true,
"daily": 227.74725925935417,
"unit": "mg"
},
{
"label": "Thiamin (B1)",
"tag": "THIA",
"schemaOrgTag": null,
"total": 1.5491302510006304,
"hasRDI": true,
"daily": 129.09418758338586,
"unit": "mg"
},
{
"label": "Riboflavin (B2)",
"tag": "RIBF",
"schemaOrgTag": null,
"total": 0.6357101683340908,
"hasRDI": true,
"daily": 48.90078217954544,
"unit": "mg"
},
{
"label": "Niacin (B3)",
"tag": "NIA",
"schemaOrgTag": null,
"total": 38.93289938559454,
"hasRDI": true,
"daily": 243.33062115996586,
"unit": "mg"
},
{
"label": "Vitamin B6",
"tag": "VITB6A",
"schemaOrgTag": null,
"total": 2.7351100999179208,
"hasRDI": true,
"daily": 210.39308460907083,
"unit": "mg"
},
{
"label": "Folate equivalent (total)",
"tag": "FOLDFE",
"schemaOrgTag": null,
"total": 140.0836344168394,
"hasRDI": true,
"daily": 35.02090860420985,
"unit": "µg"
},
{
"label": "Folate (food)",
"tag": "FOLFD",
"schemaOrgTag": null,
"total": 140.0836344168394,
"hasRDI": false,
"daily": 0,
"unit": "µg"
},
{
"label": "Folic acid",
"tag": "FOLAC",
"schemaOrgTag": null,
"total": 0,
"hasRDI": false,
"daily": 0,
"unit": "µg"
},
{
"label": "Vitamin B12",
"tag": "VITB12",
"schemaOrgTag": null,
"total": 1.1832,
"hasRDI": true,
"daily": 49.300000000000004,
"unit": "µg"
},
{
"label": "Vitamin D",
"tag": "VITD",
"schemaOrgTag": null,
"total": 1.3920000000000001,
"hasRDI": true,
"daily": 9.280000000000001,
"unit": "µg"
},
{
"label": "Vitamin E",
"tag": "TOCPHA",
"schemaOrgTag": null,
"total": 25.169014918992694,
"hasRDI": true,
"daily": 167.7934327932846,
"unit": "mg"
},
{
"label": "Vitamin K",
"tag": "VITK1",
"schemaOrgTag": null,
"total": 125.33893894280406,
"hasRDI": true,
"daily": 104.44911578567006,
"unit": "µg"
}
]
},
"bookmarked": false,
"bought": false
}
]
}

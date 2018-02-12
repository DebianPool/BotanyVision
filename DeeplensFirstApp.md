# Problem: Is plant poisonous?

## Potential Sub Problems
1. Is object being viewed a plant?
	1. If no, Then "Not a Plant."
		* For this exercise, the distinction of "poisonous" is indeterminate for non-plants.
	2. If yes, Are there any other considerations?
		* Is plant alive? If not, is the plant still dangerous? Dead plants, perhaps. Artificial plants, unlikely.
2. What is the minimum amount of data to determine if plant is poisonous?

## Data
### Which type of data is necessary\? 
	1. Historical image data of both poisonous and non poisonous plants?
	2. Levels of descriptors in Data Tables or Database?
	3. Heuristics (Rules of Thumb) e.g. (Poison Ivy does not thorns)

### Data Sources and Thresholds

1. Level I - Perfect Information
	1. Deeplens is fed data of Poison Ivy, Poison Oak, and Poison Sumac. 
		1. Most common look of the Poison plants.
		2. Also, alternate looks: 
			1. Non green colors (Red and Brown)
			2. Poison Ivy with berries or mutations
	2. Deeplens is fed data of non-poisonous plants and trees that are common in Southeastern United States.  
2. Level II - Imperfect Information	
	1. Deeplens is fed data of Poison Ivy, Poison Oak, and Poison Sumac. 
	2. Deeplens is fed data of common non-poisonous plants and trees that are common in Southeastern United States.  
3. Level III - No photo information
	1. Heuristics provided
	2. Humans identify Poison Ivy with eyesight by:
		1. Leaflet clusters of 3.
		2. Hairy vines
		3. Lack of Thorns
		4. White berries
	3. Humans identify Poison Oak with eyesight by:
		1.
		2.
		3.

### Goals
	1. Success Goal. Is Deeplens able to identify: 
		1. Poison Ivy, Poison Oak, and Poison Sumac that would be obvious to humans who 
	have been shown the same photo data?
		2. Poison Ivy, Poison Oak, and Poison Sumac that is not so obvious to humans? Alternatve colors or mutations?
		3. Is Deeplens able to identify a Poison Ivy, Poison Oak, and Poison Sumac that human cannot identify?
	2. Stretch Goal. Is Deeplens able to identify:
		1. Identify Kudzu - Non poisonous vine ubiquitous in South. Also three leaf. Also, invasive 
		2. Oak, Pine, and Magnolia trees.

## The Models (Math) and Algorithms (Computer programs)
* Which models can we use?
	* Is dimensional or data reduction needed?
	* Human Chosen
	1. Regression
		1. Logit model/Logistic regression algorithm
		2. 
	2. Classification
		1. Tree Pruning
		2. 
	* Machine Chosen	
	1. 
	2. 
* Which tools can we use?
	1. Pen and paper.
	2. Software programming languages. R, Python, Julia.
	3. Cloud native services. Amazon 
	4. Open Source. Apache Spark	
* What will we do...?

## Project execution 

1. Obtain data
	1. Get images of plants from internet
	2. Take photos of plants and trees with Apple iPhone.
2. Classify data for experiment	
	* Internet images of plants from internet will be split into four groups.
		1. Poison Ivy, Atlantic Poison Oak, and Poison Sumac image data that will be fed (trained?) to model.
		2. Poison Ivy, Atlantic Poison Oak, and Poison Sumac image data that will not be fed to model.
		3. Non-poisonous plants and trees that are common in Southeastern United States will be fed to model.
		4. Non-poisonous plants and trees that are common in Southeastern United States will not be fed to model.
	* Model will be used to identify Plant photos taken by iPhone.
	* Model will be presented to Deeplens. 
		* Deeplens will be pointed at cut off pieces of plants in order to classify			
3. Store data.
	1. Provision a S3 bucket with different key paths. Internet images. iPhone photos.
		* Bucket -> (Non)Poison -> Plant
	2. Make bucket public.
4. Create Models
	1. First utilize models provided by Sagemaker.
		* 
	2. Then use Python Scikit learn and R.
5. Run Data through Sagemaker
	1. Is Sagemaker able to correctly identify Google Images it did not see?
	2. Is Sagemaker able to correctly identify iPhone plant photos?
	3. Is Deeplens powered by Sagemaker able to correctly identify plants?  	
6. Publish results
	1. S3
	2. Github
	3. API endpoint?			 
	
		 	
By I, Melissambwilkins, CC BY-SA 3.0, https://commons.wikimedia.org/w/index.php?curid=2481847

By JESpencer - Own work, CC BY-SA 4.0, https://commons.wikimedia.org/w/index.php?curid=36302853

By Jarek Tuszyński / CC-BY-3.0 & GDFL, CC BY 3.0, https://commons.wikimedia.org/w/index.php?curid=10787324
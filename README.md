# Social Explorative Attention Networks (SEAN)

This repository provides a reference implementation of *sean* as described in the paper:<br>
> Beyond Personalization: Social Content Recommendation for Creator Equality and Consumer Satisfaction.<br>
> Wenyi Xiao, Huan Zhao, Haojie Pan, Yangqiu Song, Vincent W. Zheng, Qiang Yang.<br>
> Knowledge Discovery and Data Mining, 2019.<br>
> <Insert paper link>

The *sean* algorithm goes beyond personalized content recommendation by considering both content creators and consumers, which motivates us to develop a highly personalized attention based model and explore higher-order social friends.

### Basic Usage

#### Example
To run *sean* on Steemit-En, you can use the following command:<br/>
  ``cd sean``
  
  ``python main.py --walk-length 20 --num-walks 3``

#### Options
You can check out the other options available to use with *sean* using:<br/>
	``python main.py --help``

#### Input
The supported input format is an edgelist:

	node1_id_int node2_id_int 
		
The graph is assumed to be directed and unweighted by default. 

#### Output
The probability of clicking an unseen document by the target user.

### Citing
If you find *sean* useful for your research, please consider citing the following paper:

	@inproceedings{sean-kdd2019,
	author = {Wenyi Xiao, Huan Zhao, Haojie Pan, Yangqiu Song, Vincent W. Zheng, Qiang Yang.},
	 title = {Beyond Personalization: Social Content Recommendation for Creator Equality and Consumer Satisfaction. },
	 booktitle = {Proceedings of the 25nd ACM SIGKDD International Conference on Knowledge Discovery and Data Mining},
	 year = {2019}
	}


### Miscellaneous

Please send any questions you might have about the code and/or the algorithm to <wxiaoae@cse.ust.hk>.

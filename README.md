# CS56-2_DIFFUSION OF FALSE NEWS IN SOCIAL_Capstone5703

## Part 1
Deep reinforcement learning model in the field of influence maximization

How to use a large model:<br>
just running the code:<br>
torch.load('model_name')<br>
Large model in drive:<br>
link：https://pan.baidu.com/s/1NFz9rOI1xyEzvznn2yiyeA <br>
password：m76m <br>


How to use a small model:<br>
First, create the agent class in our Jupyter file(run agent part), and then <br>
agent_name.load('weights_model')<br>

Then beginning to train and test<br>



## Part 2
Using ChatGPT to detect news fake or true<br>

The things sent to the GPT server and return:<br>

In the output file, called output.csv file:<br>
The raw called "text" + the question to GPT is the input for GPT server;<br>
On the other side, the raw called "Generated" is the return from ChatGPT.<br>


## Data description

### GPT section

Dataset used for GPT experiment: <br>
Fake news detection dataset with labels<br>
Original source:<br>
https://www.kaggle.com/datasets/harshitsingh1710/fake-news-detection-dataset-with -labels<br>

### DQN section
Dataset used for reinforcement learning experiment: <br>

ca_GrQc dataset<br>
This dataset shows scientific collaborations between authors of general relativity and quantum cosmology categories. Each node represents an author of a paper, while an edge represents a collaborative relationship between two authors. This data set contains a total of 5242 nodes and 14496 edges. Data covers the time range from January 1993 to April 2003. <br>
The original version of the dataset can be found here: https://networkrepository.com/ca-GrQc.php <br>
Original Paper: Leskovec, J., Kleinberg, J., & Faloutsos, C. (2007). Graph evolution: Densification and shrinking diameters. ACM transactions on Knowledge Discovery from Data (TKDD), 1(1), 2-es. <br>

fb-pages-food dataset<br>
This data set represents the facebook pages related to different foods in the facebook social platform, each node represents each page, and the existence of edges between nodes means that there are mutual likes among pages. This dataset contains a total of 620 nodes and contains 2100 edges. We use this real social network dataset for further research in the experimental section.<br>
The original version of the dataset can be found here: https://networkrepository.com/fb-pages-food.php<br>
Original Paper: Rossi, R., & Ahmed, N. (2015, March). The network data repository with interactive graph analytics and visualization. In Proceedings of the AAAI conference on artificial intelligence (Vol. 29, No. 1).<br><br>
The other .mtx files are used in the future work.

### The description of .mtx file
The header line is usually the first line that begins with at least one % and in many cases two %%, followed by MatrixMarket and in most cases four fields that describe the data stored. <br>
In general, the first line to appear without % represents N M K where N is the number of rows, M is the number of columns, and K is the number of nonzeros in the matrix. For instance, the first line in ca-GrQc.mtx file is 5242 5242 14496 and indicates the number of nodes is N=5242 and number of edges is K=14496.<br>
Each of the remaining rows represents the index of the node, which already indicates the relationship between the two nodes.<br>

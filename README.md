# Flower Classifier Decision Tree

This is one of the first projects that you would do in your first practical course in a Machine Learning course (literally).

Very simple, very easy to understand and has explanations at every step.

Just to understand better and get used to implementations of Decision Trees, you are super-duper encouraged to implement this project yourself.

You can find a visual representation and a detailed description of our decision tree below.

The dataset we are using is iris dataset of sklearn. You will see this dataset on a lot of entry-level projects.

This dataset has information about 150 iris flowers with 4 features describing each flower.

-> Sepal length, sepal width, petal length, petal width. (If these words are not familiar to you, simply google 'iris dataset' and surf the images about it)

It also has a target variable indicating the flowers species: Setosa, Vesicolor, Virginica.

When we load the dataset into a dataframe, it should look like this:

![Ekran görüntüsü 2024-10-24 181326](https://github.com/user-attachments/assets/65fc55e1-2dc2-4bd6-a246-fb930d9e183b)



A Visual representation of the data, where different shades of colors represent different species:

![Figure_1](https://github.com/user-attachments/assets/12c77654-d2d8-4739-9af7-9fbe55e7b2de)



After we train and run the model, we see a perfect score for our 4 evaluation metrics:

![Ekran görüntüsü 2024-10-24 181335](https://github.com/user-attachments/assets/04207158-f0e3-4d12-8ab1-cd26ec4071f6)



Finally, Let's take a look at our Decision Tree:

We can see the visual representation of the decision tree classifier we trained on the iris dataset.
This visualization helps us understand the process the model uses to classify new data points.
The decision tree typically represented as a flow chart-like structure, starting from as single root node at the top and branching out to subsequent nodes as the decision-making process progresses.

![dec_tree](https://github.com/user-attachments/assets/9398806e-1214-4658-b83a-c73b0f2a49ad)


Key elements of the decision tree are nodes, edges and labels.
Decision Tree is composed of nodes. Each node represents a specific condition or decision rule based on a feature of the data. The condition is displayed within the nodes box. 
There are two main types of nodes: 
Internal Nodes: Represents decision points. They typically contain a condition based on a feature. For example: Petal length <= 2.45. 
If the condition is true, decision tree follows the left branch, otherwise, it followes the right branch.
Leaf Nodes: Represents the final decisions or classifications. They indicate the predicted class or category for a given data point based on the decision made at the internal nodes. 

Edges connect the nodes, representing the possible paths a data point can take through the tree based on the decisions made at the each node. Each node has labels that provide information about the decision or classfication made at that node. These labels typically include:
Gini Index: Measures the impurity or disorder at a node. A lower gini value indicates a pure node, where most data points belong to the same class.
Samples: Is the number of data points that reach that node.
Value: represents the distribution of class labels among the data point at that node.
Class: Is the predicted class or category for data points that reach that node. The background color of a node indicates the class distribution of the data points that reach that node. For example: A node with a green-ish color might indicate that most data points reachnig that node belong to the 'versicolor' class. 

To understand how the decision tree makes predictions, follow the paths from the root node to the leaf nodes. each path represents a set of conditions that a data point must satisfy to be classified into a particular category.
To predict the species of a new Iris flower, you would provide the measurements of its sepal length, sepal width, petal length, petal width to the decision tree. The tree would then follow its decision rules and classify the flower based on the values of these features. 
 

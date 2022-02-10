# <b>`DevIncept` 

# Introduction to Machine Learning   🤖 

<font color=green>`Table of Contents` </font>


1. What is Machine Learning?
2. The Big Data Era
3. Types of Machine Learning Problems
4. Steps to solve Machine Learning Problems
5. Data Gathering
6. Data Preprocessing
7. Feature Engineering
8. Algorithm Selection and Training
9. Making Predictions
10. Uses of ML
11. Advantages of ML
12. Disadvantages of ML
13. Libraries for ML
14. Summary

# <b>1.What is Machine Learning?  🤔 

- Machine learning is a branch of artificial intelligence (AI) focused on building applications that learn from data and 
  improve their accuracy over time without being programmed to do so.





- Machine learning is about extracting knowledge from data.





- It is a research field at the intersection of statistics, artificial intelligence, and computer science and is also known as   predictive analytics or statistical learning. Machine learning algorithms are used in a wide variety of applications, such     as   in medicine, email filtering, speech recognition, and computer vision, where it is difficult or unfeasible to develop     conventional algorithms to perform the needed tasks.





![intro](https://www.ubuntupit.com/wp-content/uploads/2019/08/Intro-to-Machine-Learning-A-Machine-Learning-Course-by-Udacity.png)




# 2.The Big Data Era  🤳 

 ### Data




- Data already available Everywhere


- Low storage costs: Everyone has Several GB's for free


- Hardware are more Powerful and cheaper than before




### Devices



- Everyone has a computer fully Packed with Sensors
             * GPS
             * Cameras
             * Microphone
             
             
             
### Services



- Cloud Computing:
          online storage
          Infracture as a service
          
  
  
  
- User Applications:
          Facebook
          Email
          Facebook
          Twitter
          
![intro](https://image.slidesharecdn.com/leadershipinthebigdataerav2-131106025439-phpapp01/95/leadership-in-the-big-data-era-4-638.jpg?cb=1395168758)





# 3.Types of Machine Learning Problems  👇🏻 

###  <font color=blue>SUPERVISED LEARNING</font>


  - Learn through examples of which we know the desired output( what we want to predict)
    
    
    Examples:
         
           Is this a Cat or Dog
           
           Are the Emails are spam or not?
           
           Predict the market value of houses,etc..,
           
           
           
 - CLASSIFICATION : Output is Discrete Variable.Example(cat/Dog,Yes/No)
 - REGRESSION     :Output is continuous .Example(Price,Temperature,etc..,)
 
 
 

 
 
 
 ### <font color=blue>UNSUPERVISED LEARNING</font>
 
 
 - There is no desired output.
 - Learn something about the data.Latent Relationships
 
 
 - Examples:
         I want to find out the anomilies in the credit card usage of my customers
         
         
 `Semi-Supervised Learning :- Semi-supervised learning falls between unsupervised learning (without any labeled training data) and supervised learning (with completely labeled training data). Some of the training examples are missing training labels, yet many machine-learning researchers have found that unlabeled data, when used in conjunction with a small amount of labeled data, can produce a considerable improvement in learning accuracy.`
 
 
 
 

 
 
 ### <font color=blue>REINFORCEMENT LEARNING</font>
 
 - Reinforcement learning is a learning method that interacts with its environment by producing actions and discovers errors or rewards. Trial and error search and delayed reward are the most relevant characteristics of reinforcement learning. This method allows machines and software agents to automatically determine the ideal behavior within a specific context in order to maximize its performance. Simple reward feedback is required for the agent to learn which action is best.

- Due to its generality, the field is studied in many other disciplines, such as game theory, control theory, operations research, information theory, simulation-based optimization, multi-agent systems, swarm intelligence, statistics and genetic algorithms
 
 
 - Examples:
         An Agent interacts with an Environment and watches the result of the interaction.
         Environment gives feedback via a positive or Negative Reward signal.
         
         
         
    
  
 

 

         
![intro](https://miro.medium.com/max/903/0*-068ud_-o3ajwq_z.jpg)
    
         
         
         
    
    
    

 
 
 

 
 
 
 
 
 
 
 
 

          
          




# 4.Steps to solve Machine Learning Problems👀












##### <font color=green>Data Gathering</font> : collecting data from various sources
##### <font color=green>Data Preprocessing</font>: Clean data to have Homogenity
##### <font color=green>Feaure Engineering</font>: Making your data more useful
##### <font color=green>Data structure and Algorithms</font>: Selecting the right Machine Learning Model
##### <font color=green>Making Prediction</font>: Evaluate the Model








# 5.Data Gathering👩🏽‍🤝‍👩🏽👨🏿‍🤝‍👨🏾

 * #### Might depend on Human work:
                        Manual Labelling for Supervised Learning
                        Domain Knowledge.Maybe experts
 * #### May come for free and "sort of"
                        Eg.Machine Translation
                        
 * #### The more the better: 
                      Some algorithms need large amounts of data to be useful 
                      (e.g.Neural Networks)
                      
                      



# 6.Data Preprocessing🎨

####  Is there anything wrong with the data?
       - Missing values
       - Outliers
       - Bad Encoding (for text)
       - wrongly-labeled Examples
       - Biased Data
### >> Fix the data/Remove data!!


![intro](https://serokell.io/files/df/dfsdv4ab.2_(23)_(1).jpg)


# 7.Feature Engineering🧂

#### What is a feature?
   * A feature is an individual Measurable property of a Phenomenon being Oberved
   
   
   

   * Our inputs are represented by a set of Features
   
   
   
   
   
   
   - To classify a spam email features could be:
   
   
                                      - No of words that have been c3han2d like this
                                      
                                      - Language of the email(0-Spanish,1-English)
                                      
                                      - No of Emojis
                                      
                                      
                                      
                                      
                                      
  - Extract more information from extisting data, not adding "new" data per data-set
  
  
                                       - Making it more useful
                                       
                                       - With good features,most algorithms can learn faster
                                       
                                       
                                       
                                       
 - It can be an ART
                                       - Requires thought and knowledge of data
                                       
                                       
                                       
 - Two steps
                                       - varibale Transformation(e.g.dates into weekdays , normalizing)
                                       
                                       
                                       - Feature Creation (e.g. n-grams for texts,if word is capitalized to
                                         detect names , etc.,)
      
      
   ![intro](https://www.kdnuggets.com/wp-content/uploads/feature-engineering-fig1-1.jpg)

# 8.Algorithm Selection and Training⚓

## supervised :
                 
                   

               - Linear Classifier
               
               - Naive bayes
               
               - Support Vector Machines(SVM)
               
               - Decisionn Tree
               
               - Random Forests
               
               - k Nearest Neighbours
               
               - Neural Networks (Deep Learning)

## Unsupervised :
                     
               - PCA
               
               - K Means
               
               - DBSCAN
               
               - t-SNE

# Reinforcement Learning:

               - SARSA lambda
               
               - Q learning

### Goal of Training :

                 - Making the correct prediction as often as Possible
                 
                 
                 
####  > use of metrices for evaluating the Performance and comparing solutions


#### > HyperParamter Tuning: more an art than science

# 9.Making Predictions🚡




![an-introduction-to-machine-learning-and-how-to-teach-machines-to-see-a-presentation-from-tryolabs-23-638.jpg](http://davejulian.net/images/bo3547_01_02.png)

# 10.Uses of ML💌







   1.Image Recognition:- The image recognition is one of the most common uses of machine learning applications. It can also be referred to as a digital image and for these images, the measurement describes the output of every pixel in an image. face recognition is an example of image recognition .

2.Voice Recognition:- Machine learning (ML) also helps in developing the application for voice recognition. It also referred to as virtual personal assistants (VPA). It will help you to find the information when asked over the voice. There are many devices available in today’s world of Machine learning for voice recognition that is Amazon echo and google home is the smart speakers.

3.Predictions:- It helps in building the applications that predict the price of cab or travel for a particular duration and congestion of traffic where can be found. While booking the cab and the app estimates the approximate price of the trip that is done by the uses of machine learning only.

4.Videos Surveillance:- It helps to detect the crime or any miss happening that is going to happen before it happens, and it will create an automatic alert to the guards or people who all are posted there and they can help to avoid any issues or problems.

5.Social Media Platform:- Social Media is being used for providing better news feed and advertisement as per the user’s interest is mainly done through the uses of machine learning only. There are many examples like friend suggestions, page suggestions for Facebook, songs,and videos suggestion on YouTube.

6.Spam and Malware:- Email clients use a number of spam filtering and these spam filters are continuously getting updated and these are mainly done by the uses of machine learning.

7.Search Engine:- There are search engines available while searching to provide the best results to customers. There are many machine learning algorithms created for searching the particular user query like for google.

8.Applications/Companies:- There are many applications and companies that used machine learning for doing their day to day process as it is being more accurate and precise than manual interventions. These companies are Netflix, facebook, google maps, Gmail, Google search etc.

9.Fraud and Preference:- It is being used by the companies to keep track of money laundering like Paypal. It uses the set of tools to help them to check or compare the millions of transactions and make secure transactions.

10.Customer Support:- Most of the reputed companies or many websites provide the option to chat with a customer support representative. So, after asking any query by the customer, it is not compulsory that the answer is given by the human only, sometimes the answers are given by the chatbot which extracts the information from the website and provides the answer to customers. Now they are better and understand the queries quickly and faster and also provides a good result by giving appropriate result and it is done by the uses of machine learning only.



![applications-of-machine-learning.png](https://static.javatpoint.com/tutorial/machine-learning/images/applications-of-machine-learning.png)

# 11.Advantages of ML❕❗

1. Easily identifies trends and patterns
Machine Learning can review large volumes of data and discover specific trends and patterns that would not be apparent to humans. For instance, for an e-commerce website like Amazon, it serves to understand the browsing behaviors and purchase histories of its users to help cater to the right products, deals, and reminders relevant to them. It uses the results to reveal relevant advertisements to them.




2. No human intervention needed (automation)
With ML, you don’t need to babysit your project every step of the way. Since it means giving machines the ability to learn, it lets them make predictions and also improve the algorithms on their own. A common example of this is anti-virus softwares; they learn to filter new threats as they are recognized. ML is also good at recognizing spam.




3. Continuous Improvement
As ML algorithms gain experience, they keep improving in accuracy and efficiency. This lets them make better decisions. Say we need to make a weather forecast model. As the amount of data we have keeps growing, your algorithms learn to make more accurate predictions faster.



4. Handling multi-dimensional and multi-variety data
Machine Learning algorithms are good at handling data that are multi-dimensional and multi-variety, and they can do this in dynamic or uncertain environments.



5. Wide Applications
We could be an e-tailer or a healthcare provider and make ML work for us. Where it does apply, it holds the capability to help deliver a much more personal experience to customers while also targeting the right customers.

# 12.Disadvantages of ML▶

With all those advantages to its powerfulness and popularity, Machine Learning isn’t perfect. The following factors serve to limit it:

1. Data Acquisition
Machine Learning requires massive data sets to train on, and these should be inclusive/unbiased, and of good quality. There can also be times where they must wait for new data to be generated.




2. Time and Resources
ML needs enough time to let the algorithms learn and develop enough to fulfill their purpose with a considerable amount of accuracy and relevancy. It also needs massive resources to function. This can mean additional requirements of computer power for us.





3. Interpretation of Results
Another major challenge is the ability to accurately interpret results generated by the algorithms. We must also carefully choose the algorithms for our purpose.





4. High error-susceptibility
Machine Learning is autonomous but highly susceptible to errors. Suppose we train an algorithm with data sets small enough to not be inclusive. We end up with biased predictions coming from a biased training set. This leads to irrelevant advertisements being displayed to customers. In the case of ML, such blunders can set off a chain of errors that can go undetected for long periods of time. And when they do get noticed, it takes quite some time to recognize the source of the issue, and even longer to correct it.

# 13.Libraries for ML💬

1.Scikit -learn - for handling basic ML algorithms like clustering, linear and logisticregressions, regression, classification, and others.



2.Numpy - NumPy is a very popular python library for large multi-dimensional array and matrix processing, with the help of a large collection of high-level mathematical functions. It is very useful for fundamental scientific computations in Machine Learning.




3.Pandas - for high-level data structures and analysis. It allows merging and filtering of data, as well as gathering it from other external sources like Excel, for instance.



4.Keras - for deep learning. It allows fast calculations and prototyping, as it uses the GPU in addition to the CPU of the computer.




5.TensorFlow - for working with deep learning by setting up, training, and utilizing artificial neural networks with massive datasets.




6.Matplotlib - for creating 2D plots, histograms, charts, and other forms of visualization.




7.NLTK - for working with computational linguistics, natural language recognition, and processing.




8.Scikit -image for image processing.




9.PyBrain - for neural networks, unsupervised and reinforcement learning.




10.Caffe - for deep learning that allows switching between the CPU and the GPU and processing 60+ mln images a day using a single NVIDIA K40 GPU.




11.StatsModels - for statistical algorithms and data exploration.


![intro](https://www.fireblazeaischool.in/blogs/wp-content/uploads/2020/06/Python-Libraries-1024x683.png)


# 14.Summary⏭

What is machine learning? Machine learning is a subfield of artificial intelligence. Instead of relying on explicit programming, it is a system through which computers use a massive set of data and apply algorithms to "train" on--to teach themselves--and make predictions.






When did machine learning become popular? The term "artificial intelligence" was coined in the 1950s by Alan Turing. Machine learning became popular in the 1990s, and returned to the public eye when Google's DeepMind beat the world champion of Go in 2016. Since then, ML applications and machine learning's popularity have only increased.





Why does machine learning matter? Machine learning systems are able to quickly apply knowledge and training from large data sets to excel at facial recognition, speech recognition, object recognition, translation, and many other tasks.





Which industries use machine learning? Machine learning touches industries spanning from government to education to healthcare. It can be used by businesses focused on marketing, social media, customer service, driverless cars, and many more. It is now widely regarded as a core tool for decision making.





How do businesses use machine learning? Business applications of machine learning are numerous, but all boil down to one type of use: Processing, sorting, and finding patterns in huge amounts of data that would be impractical for humans to make sense of.




What are the security and ethical concerns about machine learning? AI has already been trained to bypass advanced antimalware software, and it has the potential to be a huge security risk in the future. Ethical concerns also abound, especially in relation to the loss of jobs and the practicality of allowing machines to make moral decisions like those that would be necessary in self-driving vehicles.





What machine learning tools are available? Businesses like IBM, Amazon, Microsoft, Google, and others offer tools for machine learning. There are free platforms as well.

# ` HAPPY LEARNING!!!!`        


by:
   `Hemachandiran.T |`
   `Shivansh` |
   `Nishi Sus`
   
   
   
   `copyright:Devincept 2021`

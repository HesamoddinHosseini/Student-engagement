![image](https://github.com/HesamoddinHosseini/Student-engagement/assets/89314766/c5363f6f-8112-4852-96cd-d675df3eddf6)




# Abstract:

Engagement is a key indicator of the quality of learning experience, and one that plays a major role in developing intelligent educational interfaces.
Any such interface requires the ability to recognise the level of engagement in order to respond appropriately; however, there is very little existing data to learn from, and new data is expensive and difficult to acquire. 

 For instance, if students feel frustrated and become disengaged (see disengaged samples in Fig. 1), the system should intervene in order to bring them back to the learning process. However, if students are engaged and enjoying their tasks (see engaged samples in Fig. 1), they should not be interrupte

<img width="465" alt="Screen Shot 2024-04-22 at 8 55 47 pm" src="https://github.com/HesamoddinHosseini/Student-engagement/assets/89314766/2f7ed799-f725-4784-9690-489b74105315">


Fig1. Engaged (Left) and Not Engaged (Right) samples
     

# The problem:

Whether it be classrooms in Schools or an Ed-Tech platform, keeping the students engaged & connected is a common pain point which they all face.
Hence, Student Engagement is one of the pain points we are trying to solve. 

# Student Engagement

Student engagement plays a crucial role in education and benefits students, the college, and education partners.
It empowers students with the ability to acquire and practice the necessary skills to build a successful future. Helps in building better relationships with other students, staff, and faculty and helps the students understand governance within the institution’s education system. As a result, it improves student personality and enhances their skills that are necessary for driving change.

# The Bigger Picture

The goal of student engagement is said to be achieved when education partners also benefit. With the implementation of student engagement plans, there will be better bonding between education partners. This provides a better understanding of student’s varying needs to boost the campus experience and promotes a more responsive education system.

# Engagement Recognition from Images

## Engagement Recognition Dataset:

Data Collection To recognize engagement from face images, we use student engagement dataset. This dataset consists of two main classess: (1) Engaged - 1076 images belonging to 3 different subclasses: confused - 369 images, engaged - 347 images, frustrated - 360 images (2) Not Engaged - 1044 images belonging to 3 different subclasses: Looking away - 423 images, bored - 358 images, drowsy - 263 images.

Please find dataset from the following link:

https://www.kaggle.com/datasets/joyee19/studentengagement

or

https://drive.google.com/drive/folders/1o3-hu0Ut36TAy5b65Ua05K8ClIo_Njeg?usp=share_link

Dataset Samples:

<img width="673" alt="Screen Shot 2024-04-23 at 7 20 20 am" src="https://github.com/HesamoddinHosseini/Student-engagement/assets/89314766/53234d2a-0891-46d4-89d1-943a23b1ac7f">


Fig2. Randomly selected images of student engagement dataset including engaged and not Engaged


## Engagement Recognition using Deep Learning:

For this task, we have used developed CNN model introduced by Nezami et al. (2020), which is shown schematically in Fig 3.

The model contains two convolutional (Conv.) layers, followed by two max pooling (Max.) layers with stride 2, and two fully connected (FC) layers, respectively. A rectified linear unit (ReLU) activation function is applied after all Conv. and FC layers. The last step of the CNN model includes a softmax layer, followed by a cross-entropy loss, which consists of two neurons indicating engaged and disengaged classes. To overcome model over-fitting, we apply a dropout layer after every Conv. and hidden FC layer. 

<img width="966" alt="Screen Shot 2024-04-23 at 7 46 14 am" src="https://github.com/HesamoddinHosseini/Student-engagement/assets/89314766/d93c28dc-3e3f-4d3d-baf4-182bf00f9a87">

Fig3. The architecture of the CNN MODEL. We denote convolutional, max-pooling, and fullyconnected layers with “Conv”, “Max”, and “FC”, respectively


## Reference

1. Mohamad Nezami, O., Dras, M., Hamey, L., Richards, D., Wan, S., Paris, C. (2020). Automatic Recognition of Student Engagement Using Deep Learning and Facial Expression. In: Brefeld, U., Fromont, E., Hotho, A., Knobbe, A., Maathuis, M., Robardet, C. (eds) Machine Learning and Knowledge Discovery in Databases. ECML PKDD 2019. Lecture Notes in Computer Science(), vol 11908. Springer, Cham. https://doi.org/10.1007/978-3-030-46133-1_17

2. https://www.kaggle.com/datasets/joyee19/studentengagement/data

##
Hesamoddin Hosseini

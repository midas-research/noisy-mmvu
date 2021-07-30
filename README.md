# Overview

<div style="text-align: justify">
In this challenge, we present a novel but challenging task of video understanding in a multi-
modal noisy environment. While image based object detection and recognition has improved
significantly in the last decade, the same has not been replicated in the video domain. Unlike
images, understanding videos has proven to be difficult due to the added complexities of
extra dimension and complicated sequence of motions. One of the major obstacle in learning
better techniques that can understand complex actions in videos is the sheer lack of large
scale annotated data. Large annotated datasets such as ImageNet [9] and Open Image [20]
have propelled research in image understanding. The issue with doing this for videos is the
massive cost of annotating millions of videos, which is why only a handful of large scale
video datasets have been produced such as Kinetics 400/600/700 [18, 6, 7], AVA [15] and
Youtube8M [5]. An alternative to annotating such large video datasets is to accumulate the
data from the web using specific search queries. However, this automatic annotation comes
at a cost of variable noise in the data and annotation. As such, there is an ever growing need
to generate better techniques for video action understanding based on such noisy datasets
</div>

## Task Descriptions

In this grand challenge we propose three different tasks.

### Task 1: Multi-modal Noisy Learning for Action Recognition

The first task is to use the noisy action dataset to perform video action understanding. For
this task, participants can use all available modalities of the data (raw video data and the
meta data) to perform noisy visual representation learning. The goal of this task is to generate
robust learning methods that can generate meaningful visual representations for video action
recognition. The participants are free to utilize any combination of the modalities made
available to them.
In this task, the participants will have to
pre-train their methods using the noisy action
dataset, and then transfer this learning to a smaller target dataset. We will use UCF-101
dataset as target in this challenge. The participants can use the UCF-101 dataset itself for
fine-tuning the pre-trained models. The final evaluation will be done on the UCF-101 test set. The transfer learning will demonstrate how generalized the visual understanding technique
is and how reasonable the noisy dataset is for visual understanding tasks. There will be two
sets for algorithmic development and training at scale, 25k and 100k splits.

**Mini-set task** This sub-task is for quick algorithm development and faster testing for the
participants. This sub-task will only contain 25K videos with about 200 action classes.

**Full-set task** This sub-task is focused on a large scale algorithm development where the
participants will train their methods on 100K videos. This task will allow participants to
verify their approach on a wider distribution.

### Task 2: Multi-modal Noisy Learning for Video Retrieval

In this task, the participants will be required train models to perform text to video retrieval.
For this task, participants can use all available modalities of the data (raw video data and
the meta data) to perform noisy visual representation learning. The goal of this task is to
generate robust learning methods that can generate meaningful visual representations for
text to video retrieval. The participants are free to utilize any combination of the modalities
made available to them. The participants will finally test the representation quality by fine
tuning on the MSR-VTT dataset. The final evaluation will be done on its test set. Similar
to the first task, there will be two different splits which the participants can utilize.

### Task 3: Multi-modal Noisy Video Understanding

We invite researchers and participants to demonstrate effectiveness of learning from multi-
modal noisy datasets for tasks in video understanding other than those mentioned above. This
task will not be counted towards the leaderboard statistics, however novel and extraordinary
approaches will receive a special mention. Participants can use any split of the dataset
provided.

## About The Dataset

We plan to release the Noisy-Actions-2M dataset to the public in this grand challenge. To
make the challenge realistic, we will provide a small scale version containing approximately
100, 000 videos for training, from our originally collected dataset of 2M videos. This will
include the following meta information: (Weak) class labels, title, description, comments and
tags. Around 39, 000 of these videos have geo-location information. The samples will have
multi-labels with average number of labels per video as 6.825 and all examples cover roughly
7000 labels. Each sample also has on an average 11.97 tags assigned to it, with the total
number of tags being 1.4 million in the whole dataset. The average number of comments
per video is 5.57. We will also provide a mini-noisy-action subset which has around 25K
videos covering around 5000 action labels. This will ensure the participation from interested
researchers with limited computational resources. The evaluation of task 1 will be done on
the test set of UCF-101 [28] and the task 2 will be evaluated on the test set of MSR-VTT
[34]. We will also provide features for videos in the 25K and the 100K split, extracted using
4R(2+1)D-d network trained on the Kinetics [18] dataset. More details of Noisy-Actions-2M
is provided in the supplementary dataset documentation.

## Important dates

- Paper submission: <strong>July 30th, 2021</strong>
- Author Notification: <strong>August 26th, 2021</strong>
- Camera-Ready: <strong>September 2nd, 2021</strong>
- Workshop: <strong>October XX, 2021</strong>

All deadlines are at midnight(23:59) anywhere on Earth.

## Instructions

We use the same formatting template as ACM Multimedia 2021. Submissions can be of varying length from 4 to 8 pages, plus additional pages for the reference pages. There is no distinction between long and short papers. All papers will undergo the same review process and review period. All contributions must be submitted through CMT.

Use the following link: [https://cmt3.research.microsoft.com/ACMMM2021/](https://cmt3.research.microsoft.com/ACMMM2021/)
Select the track: “1st International Workshop on Trustworthy AI for Multimedia Computing”.
The accepted workshop papers will be published in the ACM Digital Library.

## Schedule

| Time  | Event                        |
| ----- | ---------------------------- |
| 9:00  | Opening remarks              |
| 9:10  | Invited talk 1               |
| 9:45  | Invited talk 2               |
| 10:20 | Invited talk 3               |
| 10:55 | Invited talk 4               |
| 11:30 | Invited talk 5               |
| 12:05 | Lunch break                  |
| 14:00 | Invited talk 6               |
| 14:30 | Oral 1                       |
| 15:00 | Oral 2                       |
| 15:30 | Oral 3                       |
| 15:45 | Poster Session and tea break |

## Organizers

<div style="display: flex">
  <div style="width:22.5%">
    <a href="http://people.rennes.inria.fr/Teddy.Furon/website/Welcome.html">
    <img alt="Mubarak Shah" src="pics/teddy2.jpeg">
    </a><br>
    <a href="http://people.rennes.inria.fr/Teddy.Furon/website/Welcome.html">Mubarak Shah</a><br>
    University of Central Florida (UCF)
  </div>
  
  <div style="width:2.5%">
  </div>
  
  <div style="width:22.5%">
    <a href="http://www.cs.ucf.edu/~liujg/">
    <img alt="Mohan S Kankanhalli" src="pics/jingen2.jpg">
    </a><br>
  <a href="http://www.cs.ucf.edu/~liujg/">Mohan S Kankanhalli</a><br>
    National University of Singapore 
  </div>
 
  
  <div style="width:2.5%">
  </div>
  
  <div style="width:22.5%">
    <a href="https://www.crcv.ucf.edu/person/rawat/">
    <img alt="Shin’ichi Satoh" src="pics/rawat.jpg">
    </a><br>
  <a href="https://www.crcv.ucf.edu/person/rawat/">Shin’ichi Satoh</a><br>
    National Institute of Informatics
  </div>

<div style="width:2.5%">
  </div>
  
  <div style="width:22.5%">
    <a href="https://www.crcv.ucf.edu/person/rawat/">
    <img alt="Yogesh Rawat" src="pics/rawat.jpg">
    </a><br>
  <a href="https://www.crcv.ucf.edu/person/rawat/">Yogesh Rawat</a><br>
    University of Central Florida (UCF)
  </div>
</div>

<div style="width:2.5%">
  </div>

<div style="display: flex">
  <div style="width:22.5%">
    <a href="http://wzhang.fun/">
    <img alt="Rajiv Ratn Shah" src="pics/wei2.jpg">
    </a><br>
    <a href="http://wzhang.fun/">Rajiv Ratn Shah</a><br>
    Indraprastha Institute of Information Technology Delhi
  </div>

  <div style="width:2.5%">
  </div>
  
  <div style="width:22.5%">
    <a href="https://www-users.cs.umn.edu/~qzhao/index.html">
    <img alt="Roger Zimmermann" src="pics/qi2.jpg">
    </a><br>
  <a href="https://www-users.cs.umn.edu/~qzhao/index.html">Roger Zimmermann</a><br>
    National University of Singapore
  </div>

  <div style="width:2.5%">
  </div>
  
  <div style="width:22.5%">
    <a href="https://www-users.cs.umn.edu/~qzhao/index.html">
    <img alt="Shruti Vyas" src="pics/qi2.jpg">
    </a><br>
  <a href="https://www-users.cs.umn.edu/~qzhao/index.html">Shruti Vyas</a><br>
    Center for Research in Computer Vision
    University of Central Florida
  </div>

  <div style="width:2.5%">
  </div>
  
  <div style="width:22.5%">
    <a href="https://www-users.cs.umn.edu/~qzhao/index.html">
    <img alt="Mohit Sharma" src="pics/qi2.jpg">
    </a><br>
  <a href="https://www-users.cs.umn.edu/~qzhao/index.html">Mohit Sharma</a><br>
    Indraprastha Institute of Information Technology Delhi
  </div>

  <div style="width:2.5%">
  </div>
  
  <div style="width:22.5%">
    <a href="https://www-users.cs.umn.edu/~qzhao/index.html">
    <img alt="Aayush Rana" src="pics/qi2.jpg">
    </a><br>
  <a href="https://www-users.cs.umn.edu/~qzhao/index.html">Aayush Rana</a><br>
    Center for Research in Computer Vision
    University of Central Florida
  </div>

</div>

## Volunteers

<div style="display: flex">
  <div style="width:22.5%">
    <a href="https://www.linkedin.com/in/raj-aaryaman-p-4b3a70101">
    <img alt="Raj Aaryaman Patra" src="pics/teddy2.jpeg">
    </a><br>
    <a href="https://www.linkedin.com/in/raj-aaryaman-p-4b3a70101">Raj Aryaman Patra</a><br>
    National Institute of Technology Rourkela
  </div>
  
  <div style="width:2.5%">
  </div>
  
  <div style="width:22.5%">
    <a href="https://www.linkedin.com/in/harshal-desai-863027147">
    <img alt="Harshal Desai" src="pics/Harshal.jpg">
    </a><br>
  <a href="https://www.linkedin.com/in/harshal-desai-863027147">Harshal Desai</a><br>
    National Institute of Technology Jamshedpur
  </div>

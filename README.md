# Dogs vs Cats (Classification)

이 경쟁에서는 이미지에서 개 또는 고양이가 들어 있는지 여부를 분류하는 알고리즘을 작성합니다. 이
것은 사람에게는 쉽습니다. 다만, 컴퓨터에게는 조금 더 어려울 것입니다.


![woof_meow](https://user-images.githubusercontent.com/55519278/75346721-ac03ba00-58e2-11ea-919c-2efa4885d959.jpg)


## The Asirra data set (2014)

웹 서비스는 종종 사람들이 해결하기 쉽지만 컴퓨터로는 어려운 문제로 보호됩니다. 이러한 도전을 종종  CAPTCHA  (Computers and Humans Apart에 알리기위한 완전 자동화 된 공공 튜링 테스트) 또는 HIP (Human Interactive Proof)라고합니다. HIP는 전자 메일 및 블로그 스팸을 줄이고 웹 사이트 암호에 대한 무차별 공격을 방지하는 등 여러 가지 목적으로 사용됩니다.

Asirra (액세스 제한을위한 동물 종 이미지 인식)는 사용자에게 고양이와 강아지의 사진을 식별하도록 요청하여 작동하는 HIP입니다. 이 작업은 컴퓨터에서는 어렵지만 연구에 따르면 사람들이 빠르고 정확하게이를 수행 할 수있는 것으로 나타났습니다. 

Asirra는 노숙자 반려 동물의 집을 찾는 데 전념하는 세계 최대 사이트 인 Petfinder.com 과의 파트너십 덕분에 독특  합니다. 그들은 Microsoft Research에 3 백만 개가 넘는 고양이와 개 이미지를 미국 전역의 수천 개의 동물 보호소에서 수동으로 분류하여 제공했습니다. 
Kaggle은 다행스럽게도 재미와 연구를 위해이 데이터의 일부를 제공합니다. 

이 경쟁에 대한 데이터를 제공해 주신 Microsoft Research에 감사드립니다.


training 자료에는 25,000 개의 개와 고양이 이미지가 들어 있습니다. 
본 github 에 업로드한 train 데이터는 고양이 이미지100개 (총 12500개) , 개 이미지100개 (총 12500개) , 테스트 데이터 100개 (총 12500개)

전체 데이터 다운로드
https://www.kaggle.com/c/dogs-vs-cats/data

이 파일에 대해 알고리즘을 학습하고 test1.zip (1 = dog, 0 = cat)의 레이블을 예측하세요.

작성자는 MobileNetv2,ResNet18 그리고 sequential 모델을 가지고 예측해보았습니다.


# Dogs vs Cats (Classification)

In this competition, you'll write an algorithm to classify whether images contain either a dog or a cat.  This is easy for humans, dogs, and cats. Your computer will find it a bit more difficult.

Deep Blue beat Kasparov at chess in 1997.
Watson beat the brightest trivia minds at Jeopardy in 2011.
Can you tell Fido from Mittens in 2013?

## The Asirra data set
Web services are often protected with a challenge that's supposed to be easy for people to solve, but difficult for computers. Such a challenge is often called a CAPTCHA (Completely Automated Public Turing test to tell Computers and Humans Apart) or HIP (Human Interactive Proof). HIPs are used for many purposes, such as to reduce email and blog spam and prevent brute-force attacks on web site passwords.

Asirra (Animal Species Image Recognition for Restricting Access) is a HIP that works by asking users to identify photographs of cats and dogs. This task is difficult for computers, but studies have shown that people can accomplish it quickly and accurately. Many even think it's fun! Here is an example of the Asirra interface:

Asirra is unique because of its partnership with Petfinder.com, the world's largest site devoted to finding homes for homeless pets. They've provided Microsoft Research with over three million images of cats and dogs, manually classified by people at thousands of animal shelters across the United States. Kaggle is fortunate to offer a subset of this data for fun and research. 

## Image recognition attacks
While random guessing is the easiest form of attack, various forms of image recognition can allow an attacker to make guesses that are better than random. There is enormous diversity in the photo database (a wide variety of backgrounds, angles, poses, lighting, etc.), making accurate automatic classification difficult. In an informal poll conducted many years ago, computer vision experts posited that a classifier with better than 60% accuracy would be difficult without a major advance in the state of the art. For reference, a 60% classifier improves the guessing probability of a 12-image HIP from 1/4096 to 1/459.

## State of the art
The current literature suggests machine classifiers can score above 80% accuracy on this task [1]. Therfore, Asirra is no longer considered safe from attack.  We have created this contest to benchmark the latest computer vision and deep learning approaches to this problem. Can you crack the CAPTCHA? Can you improve the state of the art? Can you create lasting peace between cats and dogs?

Okay, we'll settle for the former. 


## Acknowledgements
We extend our thanks to Microsoft Research for providing the data for this competition.


The training archive contains 25,000 images of dogs and cats. 
Train your algorithm on these files and predict the labels for test1.zip (1 = dog, 0 = cat).
full datasets down load : https://www.kaggle.com/c/dogs-vs-cats/data

# COSE461-NLP 9조 프로젝트 소스코드 Readme
## 한국어
다음 웹페이지의 소스코드를 일부 참고했습니다.  
https://nbviewer.jupyter.org/github/cyc1am3n/Deep-Learning-with-Python/blob/master/Chap03-getting_started_with_neural_networks/Chap03-Extra-classifying_korean_movie_review.ipynb  
test디렉토리와 data디렉토리를 ipynb 소스파일이 있는 디렉토리내에 위치하도록 합니다.  
Korean_analysis_fasttext.ipynb 소스 코드 세 번째 셀 블록의 경로 변수들의 수정이 필요합니다. 각 디렉토리 경로명은 /로 끝나야합니다.  
KAGGLE_TEST_BASE_DIR 의 값을 test 디렉토리 경로로 설정합니다.  
BASE_DIR 의 값을 ipynb 소스파일이 있는 디렉토리로 설정합니다.  
MODEL_SELECTION 변수의 값을 조정하여 어떠한 딥러닝 모델을 사용할지 결정할 수 있습니다.  
MODEL_SELECTION : 0 = LSTM, 1 = neural network, 2 = CNN  
기본으로 pre-trained fasttext 모델이 아닌, 트레이닝 데이터에 대하여 학습한 fasttext모델을 사용합니다.  
pre-trained fasttext 모델을 사용하기 위해서는
https://fasttext.cc/docs/en/crawl-vectors.html 에서 Korean: bin 파일을 다운받아 압축을 풀고 ipynb 소스파일이 있는 디렉토리 아래 data 디렉토리에 넣어야 합니다.  
이때, 다운받고 압축풀어 data 디렉토리에 넣은 파일의 이름은 wiki.ko.bin 혹은 cc.ko.300.bin 이어야 합니다.  
이후 USE_PRETRAINED_FASTTEXT 변수를 True 로 바꾸면 pre-trained fasttext 모델을 사용하여 학습을 합니다.  
이후 Korean_analysis_fasttext.ipynb 을 모두실행 시키면 됩니다.  

## 영어
2번째 Cell Block에 있는 path_dir을 교수님께서 주신 data를 압축 해제한 후 나온 EmotionLines의 주소로 바꿔주면 됩니다.  
단 꼭 path_dir은 /로 끝나야합니다.  
이후 .ipynb 파일들을 모두실행 시키면 됩니다.

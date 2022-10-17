# scaledYOLOv4


# 사용법
1. 환경 셋팅 (python3.8, cuda10.1설치)
2. pip install -r requirements.txt (라이브러리 설치)

# activation function == Leaky ReLu 사용 (mish-cuda 사용X)

# common.py == miss-cuda(예외처리)
try:
    from mish_cuda import MishCuda as Mish
except:
    class Mish(nn.Module):
    

  
# coco.dataset == bsd2022.yaml 사용

output 출력층 tensor형태 numpy형태로 변환시켜준 뒤 cpu에 올려 사용하기
![캡처](https://user-images.githubusercontent.com/76443227/196104078-e55fef03-d1cd-4b87-b411-10b2a1682526.PNG)
![1](https://user-images.githubusercontent.com/76443227/196104087-81750eec-f26d-4efe-a74f-9a7fc95418ae.PNG)




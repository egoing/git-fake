# 소개
교육용으로 간단하게 여러개의 커밋을 만들어야 하는 경우 귀찮음을 줄여주는 프로그램입니다. 아래 영상을 통해서 사용법과 설치방법을 접할 수 있습니다. 

https://youtu.be/RG7JIzcgWPw

# 사용법
```
git fake
```
위의 내용은 아래의 작업을 자동으로 합니다. 
```
echo date > foo.txt
git add foo.txt
git commit -m "content `date`
```

생성되는 파일을 바꾸고 싶을 때
```
git fake -f content.txt
```

파일의 내용을 바꾸고 싶을 때 
```
git fake -c 1
```

파일의 내용을 교체하지 않고, 추가하고 싶을 때 
```
git fake -a
```

# 설치방법
1. git-fake 파일을 /usr/local/bin 에 위치시킵니다. ($PATH로 등록한 디렉토리에 위치시켜도 됩니다)
2. 실행권한을 줍니다. ```sudo chmod a+x git-fake```


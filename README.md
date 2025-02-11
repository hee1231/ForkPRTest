# Fork & Pull Request Test
포크 & 풀리퀘 테스트 레포지토리입니다. 테스트가 끝나면 삭제합니다.

- [Fork](#fork)
- [GUI](#gui)
- [CLI](#cli)
- [공통](#공통)
- [확인](#확인)

## Fork
1. 레포지토리 상단의 Fork를 클릭해주세요.
![image](https://user-images.githubusercontent.com/79434205/174788495-376dc53c-99e2-4070-af7f-6a8d082c9c0d.png)

2. create fork를 클릭해주세요.
![image](https://user-images.githubusercontent.com/79434205/174788669-6055d5ff-aa32-48ad-a025-af10f5d52b15.png)

3. 내 레포지토리에서 확인했을 때 이렇게 뜨면 성공입니다.  
![image](https://user-images.githubusercontent.com/79434205/174788891-da926dc6-3661-4730-a4a7-7631d9a0b8b7.png)

4. 다음 과정은 [GUI](#gui), [CLI](#cli) 중 편한 방법으로 따라해 주시면 됩니다.  
   원본 레포지토리가 아닌 포크한 레포지토리에서 진행해야 합니다.

## GUI
1. main이라고 적힌 녹색으로 표시된 부분을 클릭해주세요.  
![image](https://user-images.githubusercontent.com/79434205/174797482-5d365edf-e26b-4660-b84a-13cb3ef7930f.png)

2. find or create a branch... 라고 적힌 부분에 본인의 이름을 적은 후, 녹색으로 표시된 부분을 클릭해주세요.
   (main 브랜치인지 꼭 확인해 주세요.)  
![image](https://user-images.githubusercontent.com/79434205/174797324-d41950b4-e48b-4b97-8b24-730f8cd17583.png)![image](https://user-images.githubusercontent.com/79434205/174797294-b13ef646-270a-491a-9812-7f81951be7b1.png)

3. 본인 이름의 브랜치가 하나 생성됩니다.  
![image](https://user-images.githubusercontent.com/79434205/174797658-a912bf53-ed84-451c-a151-a548ca872c6b.png)

4. README.md 파일을 클릭하시고, 녹색으로 표시된 부분을 클릭한 후, [확인](#확인)에 있는 본인의 이름 옆에 (확인) 이라고 적어주세요.  
![image](https://user-images.githubusercontent.com/79434205/174798571-f53d1384-edf3-4ec7-8c92-93532a0c0715.png)

5. 본인 이름의 브랜치인지 확인한 후에 녹색으로 표시한 commit change 버튼을 눌러주세요.  
![image](https://user-images.githubusercontent.com/79434205/174777732-11c0417b-fe33-4225-9b89-33d536ff9151.png)

6. 원래 레포지토리의 최신 변경 사항을 반영하고 싶으면 fetch upstream 을 누르고 fetch and merge 누르시면 됩니다.  
자주 안 해주면 머지할 때 오류가 나기도 하므로 한 번씩 해주세요.
![image](https://user-images.githubusercontent.com/79434205/174790960-b455b96b-cdd1-40e0-befb-c24443ed9c93.png)

7. 본인의 브랜치를 확인해보면 상단에 녹색으로 표시한 contribute 가 보이실 겁니다. 클릭해주시고 open pull request를 클릭해주세요.
![image](https://user-images.githubusercontent.com/79434205/174798157-3d091870-24c0-476e-82b2-8c6a098d0e0b.png)

8. 다음 과정은 [공통](#공통)입니다.


## CLI
1. 폴더를 새로 생성해 주시고, 그 폴더에서 Git Bash를 실행합니다.  
![image](https://user-images.githubusercontent.com/79434205/174777146-b24735a6-b97d-47b1-b254-b456a75b128c.png)

2. 레포지토리 상단의 녹색 code 버튼을 누르고, 녹색으로 표시한 버튼을 눌러서 레포지토리 링크를 복사합니다.  
![image](https://user-images.githubusercontent.com/79434205/174789484-92baab01-a129-4197-826b-19d51dd769df.png)

3. Bash 창에 아래와 같이 한 줄씩 입력합니다. 
```bash
git clone 복붙한 링크
cd ForkPRTest
```
(만약 해당 폴더에 바로 클론하고 싶으면 링크 뒤에 .을 붙이면 됩니다.)
```bash
git clone [복붙한 링크] .
```

4. 아래와 같이 입력합니다.
```bash
git checkout -b "본인 이름"
```
![image](https://user-images.githubusercontent.com/79434205/174789899-1848a9cc-d9f3-4919-950c-969391bf847c.png)

5. Bash 창에 아래와 같이 입력했을 때,
```bash
git branch
``` 
이렇게 떠야 합니다.  
![image](https://user-images.githubusercontent.com/79434205/174779671-e57a1ddc-100b-4f66-926c-ef800d268c9c.png)  

6. README.md 파일을 열어서 [확인](#확인)에 있는 본인의 이름 옆에 (확인) 이라고 적어주세요.  
7. README.md 파일 수정 및 저장이 끝나면 Bash에서 아래와 같이 입력해주세요.
```bash
git add README.md
```

8. 아래와 같이 입력해 주세요. 커밋 메시지는 따옴표로 감싸주어야 하고 내용은 자유입니다. 
```bash
git commit -m "커밋 메시지"
```

9. 아래와 같이 입력해 주세요. 브랜치 이름에는 따옴표를 적지 않습니다.
```bash
git push --set-upstream origin [브랜치 이름]
```

10. 포크한 레포지토리에 원본 레포지토리의 최신 변경 사항이 반영되지 않은 경우, push가 안 될 수 있습니다.  
그럴 때는 아래와 같이 한 줄씩 입력해 주세요.
```bash
git remote add upstream [원본 레포지토리 링크]
git fetch upstream
```
이렇게 뜨면 원본 레포지토리의 최신 변경 사항이 반영됩니다. 이후에는 git fetch upstream만 해도 됩니다.
![image](https://user-images.githubusercontent.com/79434205/174796035-0387a6ce-99b2-4a92-b04b-08665ae16e04.png)  
이후 다시 푸시해주시면 됩니다.

11. 아래처럼 뜨면 성공입니다.  
![image](https://user-images.githubusercontent.com/79434205/174791651-10d99b5a-1b03-4652-8d33-3380b294b8f5.png)

12. 다시 레포지토리로 돌아가면 이렇게 뜰 겁니다. 녹색으로 표시된 compare & pull request 버튼을 눌러주세요.
![image](https://user-images.githubusercontent.com/79434205/174783635-14e80c36-3c05-4049-934c-afa28c0a7232.png)

13. 다음 과정은 [공통](#공통)입니다.

## 공통
1. 별 문제가 없다면 Able to merge 라고 뜰 것입니다. create pull request 버튼을 눌러주세요.
![image](https://user-images.githubusercontent.com/79434205/174792374-f36e414f-ca83-466e-a1c6-f7f4a69b7e9c.png)

2. merge pull request 버튼을 눌러주세요.
![image](https://user-images.githubusercontent.com/79434205/174792698-d1a8e5db-5925-479d-9553-6823914b82b4.png)

3. comfirm merge 버튼을 눌러주세요.
![image](https://user-images.githubusercontent.com/79434205/174793375-31d53aed-fe86-4568-b917-58e958a790e0.png)

4. merge가 완료되고 녹색으로 표시된 부분을 눌러서 브랜치를 삭제합니다.
![image](https://user-images.githubusercontent.com/79434205/174793023-a31a2bbe-e8ae-416a-accc-1467cd1f221c.png)

5. main 브랜치에서 README.md를 확인해 보세요.

## 확인
본인 이름 옆에 (확인) 적어주시면 됩니다!
- 김도희
- 김보람
- 여다희
- 이혜원 (확인)

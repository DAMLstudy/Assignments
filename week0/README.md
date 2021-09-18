# 0주차
## Install Git Bash
- [install url](https://git-scm.com/downloads)
- Window 운영체제 환경에서 Git과 Linux Command 를 사용하기 위해 Git Bash를 설치합니다.

## Command Line Interface & Linux Command
- [why cli & linux](https://velog.io/@hwanieee/CLI-%EC%99%80-Github)

## How to push a code to Github
- 항상 모든 코드 작업은 main branch에서 pull 한 후 진행 합니다.
```
(....) $ git checkout main
(main) $ git pull
``` 

- 코드를 작업할 branch를 생성합니다.
```
(main) $ git checkout -b feature/week0
(feature/week0) $
```

- 코드를 작업합니다.
```
(feature/week0) $ vim README.md
```

- 작업이 완료된 코드를 staging area에 `add`하여 git에서 tracking 할 수 있게 합니다.
```
(feaure/week0) $ git add README.md
```

- local repository에 `commit`하여 변경 사항을 반영합니다.
```
(feature/week0) $ git commit README.md
```


- remote repository (Github)에 `push`하여 변경 사항을 반영합니다. 
```
(feature/week0) $ git push origin feature/week0
```

- pull request를 열고 코드 리뷰를 거쳐 main branch에 merge 합니다.


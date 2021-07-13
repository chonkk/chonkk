- 👋 Hi, I’m @chonkk
- 👀 I’m interested in ... Make the future better than
- 🌱 I’m currently learning ... springboot, Hibernate, Thyleaf ...
- 📫 How to reach me ... chonkk@hotmail.com &nbsp;&nbsp;  [chonkk.blog.me](https://chonkk.blog.me)  &nbsp;&nbsp; [chonkk.github.io/resume](https://chonkk.github.io/resume)

<!---
chonkk/chonkk is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
- 그레이들 명령어를 통한 리프레쉬<br/>
./gradlew build --refresh-dependencies
- Maven 프로젝트에서 Gradle 프로젝트로 변환<br/>
 gradle init --type pom
- 브렌치 관련<br/>
git branch RB_1.0 master  --> master에서 RB_1.0 브렌치 생성<br/>
git branch -D utility  --> utility branch 삭제<br/>
git branch -m master mymaster  --> master branch 를 mymaster로 이름 변경<br/>
git checkout gh-pages  --> 현재 브렌치에서 gh-pages브렌치로 이동<br/>
git checkout -b utility  --> 브렌치 생성과 체크아웃을 동시에 <br/>
git branch -v --> 현재 브렌치 확인<br/>
- 다른 사람의 원격 저장소에서 내 저장소로 복사해올때[마지막에 . 이 있음]<br/>
git clone https://github.com/xxx/xxx .<br/>
git remote remove origin<br/>
gh repo create xxxx --public<br/>
git push -u origin master

- 원격 저장소에 repository를 새로 생성할 필요가 있을때...[Github CLI]<br/>
gh repo create your_repo_name
- 원격 저장소와 히스토리정보가 맞지 않을땔, fatal: refusing to merge unrelated histories<br/>
git pull origin main --allow-unrelated-histories

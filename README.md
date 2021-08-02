- 👋 Hi, I’m @chonkk
- 👀 I’m interested in ... Make the future better than
- 🌱 I’m currently learning ... springboot, Hibernate, Thyleaf ...
- 📫 How to reach me ... chonkk@hotmail.com &nbsp;&nbsp;  [chonkk.blog.me](https://chonkk.blog.me)  &nbsp;&nbsp; [chonkk.github.io/resume](https://chonkk.github.io/resume)

<!---
chonkk/chonkk is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
- Docker Compose 기본 커맨드<br/>
-- -f 옵션은 여러 개의 설정 파일을 사용할 때
docker-compose -f docker-compose-local.yml up<br/>
docker-compose -f docker-compose.yml -f docker-compose-test.yml up<br/>
-- 보통 -d 옵션을 사용하여 백그라운드에서 컨테이너<br/>
docker-compose up -d<br/>
-- 정의되어 있는 모든 서비스 컨테이너를 한 번에 정지시키고 삭제
docker-compose down

- docker 실행
docker run [OPTIONS] IMAGE[:TAG|@DIGEST] [COMMAND] [ARG...]<br/>
docker run -d -p 3306:3306 -e MYSQL_ALLOW_EMPTY_PASSWORD=true --name mysql mysql:5.7
- ps 명령어는 실행중인 컨테이너 목록<br/>
docker ps -a<br/>
- 컨테이너 중지하기 (stop)<br/>
docker stop [OPTIONS] CONTAINER [CONTAINER...]<br/>
- 컨테이너 제거하기 (rm)<br/>
docker rm [OPTIONS] CONTAINER [CONTAINER...]<br/>
- 이미지 목록 확인하기 (images)<br/>
docker images [OPTIONS] [REPOSITORY[:TAG]]<br/>
- 이미지 다운로드하기 (pull)<br/>
docker pull ubuntu:14.04<br/>
- 이미지 삭제하기 (rmi)<br/>
docker rmi [OPTIONS] IMAGE [IMAGE...]<br/>
- 컨테이너 로그 보기 (logs)<br/>
docker logs [OPTIONS] CONTAINER<br/>
docker logs --tail 10 ${WORDPRESS_CONTAINER_ID}<br/>
docker logs -f ${WORDPRESS_CONTAINER_ID}<br/>
- 컨테이너 명령어 실행하기 (exec)<br/>
docker exec [OPTIONS] CONTAINER COMMAND [ARG...]<br/>


- yarn 설치(NPM)<br/>
npm install -g yarn

- 메이븐 빌드(테스트 스킵)<br/>
mvn clean install<br/>
mvn --projects backend spring-boot:run<br/>
mvn package -Dmaven.test.skip=true<br/>
mvn package -DskipTests<br/>
mvn clean spring-boot:run -Drun.profiles=docker

- node.js 다운로드<br/>
https://nodejs.org/ko/ 

- npm 버전확인<br/>
npm -v

- vue-cli3 설치<br/>
npm i -g @vue/cli <br/>
vue --version

- vue 프로젝트 생성<br/>
vue create [프로젝트명] --no-git <br/>
vue init webpack my-project

- [프로젝트명] 경로로 이동 후 vuejs 실행~~<br/>
npm run serve

- git repository <br/>
echo "# example-repo" >> README.md<br/>
git init<br/>
git status<br/>
git add README.md<br/>
git commit -m "first commit"<br/>
git branch -M main<br/>
git remote add origin git@github.com:outsideris/example-repo.git<br/>
git push -u origin main<br/>
git log

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
git remote -v
git remote remove origin<br/>
gh repo create xxxx --public<br/>
git push -u origin master

- 원격 저장소에 repository를 새로 생성할 필요가 있을때...[Github CLI]<br/>
gh repo create your_repo_name
- 원격 저장소와 히스토리정보가 맞지 않을땔, fatal: refusing to merge unrelated histories<br/>
git pull origin main --allow-unrelated-histories

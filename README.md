- ๐ Hi, Iโm @chonkk
- ๐ Iโm interested in ... Make the future better than
- ๐ฑ Iโm currently learning ... springboot, Hibernate, Thyleaf ...
- ๐ซ How to reach me ... chonkk@hotmail.com &nbsp;&nbsp;  [blog.naver.com/chonkk](https://blog.naver.com/chonkk)  &nbsp;&nbsp; [chonkk.github.io/resume](https://chonkk.github.io/resume)

<!---
chonkk/chonkk is a โจ special โจ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
- Gradle Wrapper ๋ฒ์  ๋ณ๊ฒฝ<br/>
./gradlew wrapper --gradle-version 6.8.1

- Docker Compose ๊ธฐ๋ณธ ์ปค๋งจ๋<br/>
-- -f ์ต์์ ์ฌ๋ฌ ๊ฐ์ ์ค์  ํ์ผ์ ์ฌ์ฉํ  ๋
docker-compose -f docker-compose-local.yml up<br/>
docker-compose -f docker-compose.yml -f docker-compose-test.yml up<br/>
-- ๋ณดํต -d ์ต์์ ์ฌ์ฉํ์ฌ ๋ฐฑ๊ทธ๋ผ์ด๋์์ ์ปจํ์ด๋<br/>
docker-compose up -d<br/>
-- ์ ์๋์ด ์๋ ๋ชจ๋  ์๋น์ค ์ปจํ์ด๋๋ฅผ ํ ๋ฒ์ ์ ์ง์ํค๊ณ  ์ญ์ 
docker-compose down

- docker ์คํ
docker run [OPTIONS] IMAGE[:TAG|@DIGEST] [COMMAND] [ARG...]<br/>
docker run -d -p 3306:3306 -e MYSQL_ALLOW_EMPTY_PASSWORD=true --name mysql mysql:5.7
- ps ๋ช๋ น์ด๋ ์คํ์ค์ธ ์ปจํ์ด๋ ๋ชฉ๋ก<br/>
docker ps -a<br/>
- ์ปจํ์ด๋ ์ค์งํ๊ธฐ (stop)<br/>
docker stop [OPTIONS] CONTAINER [CONTAINER...]<br/>
- ์ปจํ์ด๋ ์ ๊ฑฐํ๊ธฐ (rm)<br/>
docker rm [OPTIONS] CONTAINER [CONTAINER...]<br/>
- ์ด๋ฏธ์ง ๋ชฉ๋ก ํ์ธํ๊ธฐ (images)<br/>
docker images [OPTIONS] [REPOSITORY[:TAG]]<br/>
- ์ด๋ฏธ์ง ๋ค์ด๋ก๋ํ๊ธฐ (pull)<br/>
docker pull ubuntu:14.04<br/>
- ์ด๋ฏธ์ง ์ญ์ ํ๊ธฐ (rmi)<br/>
docker rmi [OPTIONS] IMAGE [IMAGE...]<br/>
- ์ปจํ์ด๋ ๋ก๊ทธ ๋ณด๊ธฐ (logs)<br/>
docker logs [OPTIONS] CONTAINER<br/>
docker logs --tail 10 ${WORDPRESS_CONTAINER_ID}<br/>
docker logs -f ${WORDPRESS_CONTAINER_ID}<br/>
- ์ปจํ์ด๋ ๋ช๋ น์ด ์คํํ๊ธฐ (exec)<br/>
docker exec [OPTIONS] CONTAINER COMMAND [ARG...]<br/>


- yarn ์ค์น(NPM)<br/>
npm install -g yarn

- ๋ฉ์ด๋ธ ๋น๋(ํ์คํธ ์คํต)<br/>
mvn clean install<br/>
mvn --projects backend spring-boot:run<br/>
mvn package -Dmaven.test.skip=true<br/>
mvn package -DskipTests<br/>
mvn clean spring-boot:run -Drun.profiles=docker

- node.js ๋ค์ด๋ก๋<br/>
https://nodejs.org/ko/ 

- npm ๋ฒ์ ํ์ธ<br/>
npm -v

- vue-cli3 ์ค์น<br/>
npm i -g @vue/cli <br/>
vue --version

- vue ํ๋ก์ ํธ ์์ฑ<br/>
vue create [ํ๋ก์ ํธ๋ช] --no-git <br/>
vue init webpack my-project

- [ํ๋ก์ ํธ๋ช] ๊ฒฝ๋ก๋ก ์ด๋ ํ vuejs ์คํ~~<br/>
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

- ๊ทธ๋ ์ด๋ค ๋ช๋ น์ด๋ฅผ ํตํ ๋ฆฌํ๋ ์ฌ<br/>
./gradlew build --refresh-dependencies<br/>
- ํ์คํธ ์คํต<br/>
gradle build -x test<br/>
- Maven ํ๋ก์ ํธ์์ Gradle ํ๋ก์ ํธ๋ก ๋ณํ<br/>
 gradle init --type pom
- ๋ธ๋ ์น ๊ด๋ จ<br/>
git branch RB_1.0 master  --> master์์ RB_1.0 ๋ธ๋ ์น ์์ฑ<br/>
git branch -D utility  --> utility branch ์ญ์ <br/>
git branch -m master mymaster  --> master branch ๋ฅผ mymaster๋ก ์ด๋ฆ ๋ณ๊ฒฝ<br/>
git checkout gh-pages  --> ํ์ฌ ๋ธ๋ ์น์์ gh-pages๋ธ๋ ์น๋ก ์ด๋<br/>
git checkout -b utility  --> ๋ธ๋ ์น ์์ฑ๊ณผ ์ฒดํฌ์์์ ๋์์ <br/>
git branch -v --> ํ์ฌ ๋ธ๋ ์น ํ์ธ<br/>
- ๋ค๋ฅธ ์ฌ๋์ ์๊ฒฉ ์ ์ฅ์์์ ๋ด ์ ์ฅ์๋ก ๋ณต์ฌํด์ฌ๋[๋ง์ง๋ง์ . ์ด ์์]<br/>
git clone https://github.com/xxx/xxx .<br/>
git remote -v<br/>
git remote remove origin<br/>
gh repo create xxxx --public<br/>
git push -u origin master

- ์๊ฒฉ ์ ์ฅ์์ repository๋ฅผ ์๋ก ์์ฑํ  ํ์๊ฐ ์์๋...[Github CLI]<br/>
gh repo create your_repo_name
- ์๊ฒฉ ์ ์ฅ์์ ํ์คํ ๋ฆฌ์ ๋ณด๊ฐ ๋ง์ง ์์๋, fatal: refusing to merge unrelated histories<br/>
git pull origin main --allow-unrelated-histories

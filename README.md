- 👋 Hi, I’m @chonkk
- 👀 I’m interested in ... Make the future better than
- 🌱 I’m currently learning ... springboot, Hibernate, Thyleaf ...
- 📫 How to reach me ... chonkk@hotmail.com &nbsp;&nbsp;  [chonkk.blog.me](https://chonkk.blog.me)  &nbsp;&nbsp; [chonkk.github.io/resume](https://chonkk.github.io/resume)

<!---
chonkk/chonkk is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
- 다른 사람의 원격 저장소에서 내 저장소로 복사해올때[마지막에 . 이 있음]<br/>
git clone https://github.com/xxx/xxx .
git remote remove origin
gh repo create xxxx --public
git push -u origin master

- 원격 저장소에 repository를 새로 생성할 필요가 있을때...[Github CLI]<br/>
gh repo create your_repo_name
- 원격 저장소와 히스토리정보가 맞지 않을땔, fatal: refusing to merge unrelated histories<br/>
git pull origin main --allow-unrelated-histories

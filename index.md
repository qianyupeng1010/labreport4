# Lab Report 4
1. Setup: Delete any existing forks of the repository you have on your account<br>
<img width="838" alt="截屏2023-05-22 下午4 51 08" src="https://github.com/qianyupeng1010/labreport4/assets/130001791/b9f3da52-9781-4d93-b24a-ac98a03b0a2f"><br>
I opened the setting of Lab 7 repository, then click the delete botton.<br>

2. Setup: Fork the repository<br>
<img width="785" alt="截屏2023-05-22 下午5 07 50" src="https://github.com/qianyupeng1010/labreport4/assets/130001791/2dd80e3c-0583-44ce-9744-a942b46ebfca"><br>
Click the link to lab7 repository and click fork botton. By doing this, I created a fork of lab7 in my Github account.<br>

3. Log into ieng6<br>
<img width="805" alt="截屏2023-05-22 下午6 17 01" src="https://github.com/qianyupeng1010/labreport4/assets/130001791/aa067694-628c-4ae5-8b4c-916607b8b48a"><br>
Type `ssh cs15lsp23bb@ieng6.ucsd.edu` and press `<enter>`. I did not need to type in password because I already set up SSH keys for ieng6 in lab. By doing this, I am remotely logged into CSE server.<br>

4. Clone your fork of the repository from your Github account<br>
Type `git clone git@github.com:qianyupeng1010/lab7.git` and press `<enter>`. By doing this, I cloned a new fork of repository lab7.<br>
<img width="786" alt="截屏2023-05-22 下午6 15 38" src="https://github.com/qianyupeng1010/labreport4/assets/130001791/dadcfe5b-c515-4d2b-9771-de17936159fe"><br>

5. Run the tests, demonstrating that they fail<br>
Type `cd lab7` and press`<enter>`to enter `lab7` repository. Type `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java`  and press `<enter>` to compile all java files. Then type `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests` and press `<enter>` to run `ListExamplesTests`. It shows 2 tests run and 1 test fail.<br>

<img width="988" alt="截屏2023-05-22 下午6 24 46" src="https://github.com/qianyupeng1010/labreport4/assets/130001791/eab50777-044c-4f96-9ca0-56b571fcba86"><br>

6. Edit the code file to fix the failling test<br>
Type `vim ListExamples.java` and press `<enter>`, it allows me to see the text editor of ListExamples.java. Then type `41j`( do not need to press `<enter>`) , it moves down the cursor 41 lines down. Then type `11l` (do not need to press `<enter>`), it will move the cursor 11 characters to the right, and we reached the place where we need to edit. Then type `x`(do not need to `enter`), it will delete character `1` in the code. Then type `i`(do not need to press `<enter>`, this will change `vim` to insert mode. Then type `2` and press `esc`, this will insert `2` after `index` and quit insert mode. Then type `:wq`, this save and quit `vim`.<br>

<img width="447" alt="截屏2023-05-22 下午6 29 10" src="https://github.com/qianyupeng1010/labreport4/assets/130001791/92807392-104c-4590-b2f8-728e24d7c718"><br>
7. Run the test, demonstrating that they now succeed<br>
<img width="761" alt="截屏2023-05-22 下午9 04 41" src="https://github.com/qianyupeng1010/labreport4/assets/130001791/e14d449f-d6e3-4f7c-89bf-df214952fe51"><br>
Recompile the java file by typing `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java`, press `<enter>`. Then type `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests` and press `<enter>` to run ListExamplesTests. It will show 2 test run and both passes.<br>

8. Commit and push the resulting change to your Github account<br>
Type `git add ListExamples.java` into terminal and press `<enter>`, this will add my changes to ListExamples.java.<br>
Type `git commit -m "bug has been fixed"` in to the terminal and press `<enter>`. This will commit the changes with commiter message "bug has been fixed".<br>
Type `git push` and press `<enter>`. This will upload local repository contents to remote Github Repository.

<img width="725" alt="截屏2023-05-22 下午9 14 34" src="https://github.com/qianyupeng1010/labreport4/assets/130001791/15ad463b-fe2c-4373-9c18-6cddc0d53e76">

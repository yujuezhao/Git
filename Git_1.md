## learn Git 2019.5.29

#### link github account

1. create SSH key

   ```ssh-keygen -t rsa -C "email@gmail.com"```

2. [set SSH key on github](https://images2015.cnblogs.com/blog/1192146/201707/1192146-20170714173851775-474031887.png)

3. `git config --global user.name "yujuezhao"`

4. `git config --global user.email "yujuezhao1997@126.com"`

***

#### delete folder of repository on github

1. `git pull origin master`

   > fatal: not a git repository (or any of the parent directories): .git

   * fix: `git init`

   > fatal: 'origin' does not appear to be a git repository
   > fatal: Could not read from remote repository.
   >
   > Please make sure you have the correct access rights
   > and the repository exists.

   * fix: `git remote add origin git@github.com:yujuezhao/deeplearning-course`

2. `dir -la`
3. ` git rm -r --cached 4、Convolutional\ Neural\ Networks\\Week3\\Car-detection-with-YOLOv2`

4. ` git commit -m 'delete4、Convolutional Neural Networks\Week3\Car-detection-with-YOLOv2'`

5. ` git push -u origin master`


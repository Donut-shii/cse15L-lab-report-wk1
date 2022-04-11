# Week 2: Lab report 1
## Step 1:
__Download Visual Code Studio__ using the following link: 
[Link][1]
[1]: https://code.visualstudio.com/ 
and choose the version meant for your computer. Home page should look like this: 
![Image1](step1.png)

## Step 2:
- Look up course specific account through
[Link][2]
[2]: https://sdacs.ucsd.edu/~icc/index.php 
- should look something like cs15lwi22aoq where the ‘aoq’ refers to the course-specific account
- open a termnial (should be on top of the computer screen) in Visual Code
- use the a command with the following format:
```$ ssh cs15lwi22aoq@ieng6.ucsd.edu``` in the terminal 
- ssh command outputs a password request
- type password (input is invisible for security purposes) then press enter
- result should look like following screenshot: 
![Image2](step2.png)

## Step 3:
__Try running some commands__ such as cd, ls, pwd, mkdir, and cp. The specific command used in the screenshot is ```ls -lat```, which outputs a list of computer files in Unix or Unix-like systems (in this case, in MacOSX)
![Image3](step3.png)

## Step 4:
- Create folder called test
- Create java file in folder called WhereAmI.java 
- Save the following text content in file:
```
class WhereAmI {
  public static void main(String[] args) {
    System.out.println(System.getProperty("os.name"));
    System.out.println(System.getProperty("user.name"));
    System.out.println(System.getProperty("user.home"));
    System.out.println(System.getProperty("user.dir"));
  }
}
```
- run following command: java WhereAmI.java 
- __move files using the scp command__ by running ```scp WhereAmI.java cs15lwi22alg@ieng6.ucsd.edu:~/```
- type password (should be the same as when you logged in to ssh)
 
 ![Image4](step4.png)







# Lab Report 5

## Part 1: Debugging Scenario

### Student's Post

---

**Code:**

![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/9b503219-1946-4f11-b921-5a16999665af)

**Output:**

![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/2c864945-2131-455b-8ef7-5f37edf9949d)

**Problem Description:**

Hey everyone, I'm having trouble with my Java program. I'm trying to run it, but it's giving me this weird error message. The error message says something about an `ArrayIndexOutOfBoundsException`. I think it might be related to how I'm accessing elements in my array, but I'm not sure. Can anyone help me figure out what's going wrong?

### TA's Response

---

Hi there! Thanks for reaching out. It looks like you're encountering an `ArrayIndexOutOfBoundsException`, which typically occurs when you're trying to access an index in an array that doesn't exist. Please check your `for` loop. How many times would the `for` loop run and how many indexes are in your `numbers` array? 



### Student's Response

---

**Fixed Code:**

![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/f60ed29f-73fb-443d-9ecd-f689183432ab)

**Fixed Output:**

![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/ea750b95-27fc-4e35-b563-cc2b349b7be7)

**Response:**

Thanks for the help. I realized that the `i <= numbers.length` would loop the `for` loop 6 times when the `numbers` array was 5 indexes long. I believe this resulted in the `for` loop to access an index that did not exist. After changing to `i < numbers.length`, my output no longer had the `ArrayIndexOutOfBoundsException` error, ultimately fixing my bug.

### Setup Information

---

#### **File Directory and Structure**

**Path `pwd`:**

![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/6bc5ac6a-56b9-49ac-a6eb-8335dd75bfef)

**File Directory `ls`:**

![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/6044763f-56f4-4ac4-9181-5499c3f3b9f8)

**Contents of Each File Before Fixing Bug:**

`Main.java`:

![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/9b503219-1946-4f11-b921-5a16999665af)

`test.sh`:

![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/ee8d8a2d-8f01-4ce8-8727-3d4b2f799f57)

**Full Command Line to Trigger the Bug**

![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/ff445dbd-a82a-4884-8ddb-3d332b699bef)

**Description of What to Edit to Fix Bug**

To fix this bug, the user must make sure the number of times the loop is run is **equal** to the size of the respective array. In the `Main` class, because the size of the `numbers` array is 5, the `for` loop condition, `i <= numbers.length`, needs to change to `i < numbers.length` to decrease the number of times looped from 6 to 5.

**Contents of Each File After Fixing Bug:**

`Main.java`:

![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/b89b807e-8234-401c-814f-e8c0866127d0)

`test.sh`:

![image](https://github.com/williamlinplayzlegitpiano/15Llabreports/assets/55766910/eeb82ec5-2742-4475-be45-43c332bc1bc9)


## Part 2: Reflection

I feel very fortunate to attend this CSE 15L class because these labs have been the most hands-on and informative sessions I have attended in my two years at UCSD. One thing most memorable to me is how loose the environment is during labs. I have an 8am lab, and it is extremely difficult for me to drag myself out of my cozy bed to attend any of these labs. However, I look forward to every session and attend them the best of my ability since the people and tutors around me are so friendly and welcoming.

One specific thing I found fascinating in lab is the use of `vim`. Of course, it is much more tedious than using an editor like VSC. However, I have a friend who is also in CSE 15L this quarter who was able to use `vim` to edit his code last minute on the road to his hockey game. Without `vim`, he would have 100% lost marks on his CSE 12 PA, showing an extremely practical use of this tool.


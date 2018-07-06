# Table of Contents
1. [Problem](README.md#Problem)
2. [Input Dataset](README.md#Input-Dataset)
3. [Details of challenge](README.md#details-of-challenge)
4. [Instructions](README.md#Instructions)
5. [Grading](README.md#Grading)
6. [Tips on getting an interview](README.md#Tips-on-getting-an-interview)
7. [Instructions to submit your solution](README.md#instructions-to-submit-your-solution)
8. [Questions?](README.md#Questions?)

# Problem

Imagine you are a data engineer working at online pharmacy. You are asked to calculate total number of UNIQUE prescribers and total drug cost for each drug. For easier view, you are asked to arrange the results in descending order based on total drug cost. 

Disclosure: the projects that Insight Data Engineering Fellows wok on over the program are much more complicated and complex than the coding challenge. This coding challenge only tests you on basics. 

# Input Dataset

The original dataset was obtained from the Centers for Medicare & Medicaid Services but has been cleaned and simplified to match the scope of the coding challenge. It provides information on prescription drugs prescribed by individual physicians and other health care providers. The dataset identifies prescribers by their ID, last name, and first name.  It also describes the specific prescriptions that were dispensed at their direction, listed by drug name as well as the cost of the medication. 

# Instructions

We design this coding challenge to assess your ability to code and your understanding of computer science fundamentals. They are prerequisites for becoming a data engineer. To test those, we are asking you to pick a programing language of your choice (preferably Python, Scala, Java, C/C++, or Ruby because they are commonly used in the Data Engineering field), but you are only allowed to use the default data structures that come with the programming language, except for I/O libraries. For example, you can code in Python, but no Pandas or any other external libraries. ***The objective here is to see if you can implement the solution using the basic data structure building blocks. Also, it results in a large chunk of code which allows us to assess your code quality.*** 

# Grading 

For the output file that your program will create, `top_cost_drug.txt`, the fields on each line should be separated by `,`

Each line of this file should contain these fields:
* drug_name, the exact drug name as shown in the input dataset
* num_prescriber, the number of unique prescribers who prescribe the drug
* total_cost, total cost of the drug after combining all the prescribers

Confused? Check out the sample input and output files below.

For example

If below is the input file


The output results should be like this,


# Tips on getting an interview

## Writing clean, scalable and well-tested code

As a data engineer, it’s important that you write clean, well-documented code that scales for large amounts of data. For this reason, it’s important to ensure that your solution works well for a large number of records, rather than just the above example.

<a href="https://drive.google.com/file/d/1fxtTLR_Z5fTO-Y91BnKOQd6J0VC9gPO3/view?usp=sharing">here</a> is the large dataset containing over 24 million records. Note, we will use it to test the full functionalities of your code

It's also important to use software engineering best practices like unit tests, especially since data is not always clean and predictable.

Before submitting your solution you should summarize your approach and run instructions (if any) in your `README`.

You may write your solution in any mainstream programming language such as C, C++, C#, Go, Java, Python, Ruby, or Scala. Once completed, submit a link to a Github repo with your source code.

In addition to the source code, the top-most directory of your repo must include the `input` and `output` directories, and a shell script named `run.sh` that compiles and runs the program(s) that implement the required features.

If your solution requires additional libraries, environments, or dependencies, you must specify these in your `README` documentation. See the figure below for the required structure of the top-most directory in your repo, or simply clone this repo.

## Repo directory structure

The directory structure for your repo should look like this:

    ├── README.md 
    ├── run.sh
    ├── src
    │   └── pharmacy-counting.py
    ├── input
    │   └── itcont.txt
    ├── output
    |   └── top_cost_drug.txt
    ├── insight_testsuite
        └── run_tests.sh
        └── tests
            └── test_1
            |   ├── input
            |   │   └── itcont.txt
            |   |__ output
            |   │   └── top_cost_drug.txt
            ├── your-own-test_1
                ├── input
                │   └── your-own-input-for-itcont.txt
                |── output
                    └── top_cost_drug.txt

**Don't fork this repo** and don't use this `README` instead of your own. The content of `src` does not need to be a single file called `pharmacy-counting.py`, which is only an example. Instead, you should include your own source files and give them expressive names.

## Testing your directory structure and output format

To make sure that your code has the correct directory structure and the format of the output files are correct, we have included a test script called `run_tests.sh` in the `insight_testsuite` folder.

The tests are stored simply as text files under the `insight_testsuite/tests` folder. Each test should have a separate folder with an `input` folder for `itcont.txt` and an `output` folder for `top_cost_drug.txt`.

You can run the test with the following command from within the `insight_testsuite` folder:

    insight_testsuite~$ ./run_tests.sh 

On a failed test, the output of `run_tests.sh` should look like:

    [FAIL]: test_1
    [Thu Mar 30 16:28:01 PDT 2017] 0 of 1 tests passed

On success:

    [PASS]: test_1
    [Thu Mar 30 16:25:57 PDT 2017] 1 of 1 tests passed



One test has been provided as a way to check your formatting and simulate how we will be running tests when you submit your solution. We urge you to write your own additional tests. `test_1` is only intended to alert you if the directory structure or the output for this test is incorrect.

Your submission must pass at least the provided test in order to pass the coding challenge.

# Instructions to submit your solution
* To submit your entry please use the link you received in your coding challenge invite email
* You will only be able to submit through the link one time 
* Do NOT attach a file - we will not admit solutions which are attached files 
* Use the submission box to enter the link to your GitHub repo or Bitbucket ONLY
* Link to the specific repo for this project, not your general profile
* Put any comments in the README inside your project repo, not in the submission box
* We are unable to accept coding challenges that are emailed to us 

# Questions?
Emails us at cc@insightdataengineering.com

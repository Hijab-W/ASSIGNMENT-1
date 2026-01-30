# Assignment 1

The goal of this assignment is to give you hands-on experience using modern
generative AI tools. Each question is designed to be practically unmanageable
within the assignment time limit without the assistance of modern GenAI systems
—- this is intentional. You’re expected to explore, experiment, and develop
intuition for what these tools can (and can’t) do.  

Generative AI tools are quickly becoming foundational in knowledge work,
creativity, and software development. Knowing how to use them effectively is now
as essential as knowing how to code, write, or analyze data. You’ll need
practical experience to understand their strengths, limits, quirks, and how to
guide them with good prompts.

## Submission Instructions

All submissions will be made through GitHub Classroom. You’ll write code, text, or generate files using GenAI tools, and place your answers in the submission/ folder of your private repository.

Step-by-Step Instructions:

1. Join the GitHub Organization

    If you don't already have a GitHub account, create one at https://github.com/join

    You will be invited to join the course's GitHub organization via an invitation link (shared by your instructor).

    Accept the invite to join the organization -- this gives you access to assignments and allows grading access for instructors.

2. Accept the Assignment

    Go to the GitHub Classroom link for this assignment (provided by your instructor).

    Click “Accept this assignment.”

    GitHub will create a private repository for you inside the course organization.

    You’ll be redirected to your repo (it will be named something like `assignment1-[your-username])`.

3. Clone the Repository

    You can complete the work on your local machine or whatever environment you choose.

    To clone locally:

        git clone https://github.com/Rotman-MMA-GenAI-2026/assignment1-[your-username].git
        cd assignment1-[your-username]

4. Enter Your Information

    Modify the existing `ID.txt` file in the submission folder with your:
    - Name on first line
    - Email on second line  
    - Student ID on third line

5. Answer Each Question

    Each question specifies the output format and the filename to use (e.g., `q1.txt`,
    `q2.txt`, `q3.txt`, etc.) that will be used for automatic grading. In
    addition, each question will specify additional scratch work to place in the
    `q<num>/` directory.  This scratch work will be used by the grader for
    any manual marking required (e.g. remarks).  If this scratch work is not present
    then the question will not be eligible for remarking.  Output files and scratch work
    go in the appropriate place in the `submission/` folder.  Make sure file
    names match exactly.  Data used for each of the questions is located in the
    `data/` folder.
    
5. Commit and Push Your Work

    Use git to save your work to the online repo:

        git add submission/<file X>
        git commit -m "Completed GenAI assignment question X"
        git push origin main

    Repeat this any time you add or update files.

    Note: A GitHub Action will automatically run tests on each push to verify that
    all required submission files are present and properly formatted. You can check
    the status of these tests in the "Actions" tab of your repository.  If any tests
    fail, review the error messages in the test output to identify missing or
    incorrectly named files.  Fix any issues and push again to re-run the tests.
    Make sure all tests pass before the deadline.  Failed tests due to not following the instructions will impact your grade.


7. Final Submission

    Once all tasks are complete and pushed to GitHub, you’re done.

    **We will grade directly from your private repository.  No additional upload or notification is needed.**


## Question 1 (5 marks)


Write a maximum of 500 word essay on your personalized assigned topic listed in `q1-essay_topics.csv`. The topic is generated based on the student bio you provided to the MMA program.  The essay will be marked by an LLM on the following points:

* The essay is about the topic
* The essay has no spelling or grammar errors
* The essay is well-written and easy to understand

The essay should be named `q1.txt` and be less than 500 words total and placed in
the submission folder. 
Save and place any prompts/conversation history/code you used to
generate your final answer in the `q1/` folder.

## Question 2 (5 marks)

Your task is to **generate a clear, concise, and professional email** requesting a meeting with a company executive. The content of the email should be based on the specific meeting topic **assigned to you** in the file `q2-email_topics.csv` located in the root of your repository.

Requirements:

* First line should be "Subject: [email subject line]"
* Address the email to a generic executive (e.g., "Dear [Executive Name],").
* Clearly state the purpose of the meeting and why it's important.
* Keep the tone formal and respectful.
* Follow typical professional email conventions.
* The email should be **between 100 and 150 words**.

The email should be named `q2.txt` and placed in the submission folder.
Save and place any prompts/conversation history/code you used to
generate your final answer in the `q2/` folder.

## Question 3 (5 marks)

You task is to answer 5 questions assigned to your student id about the
[One Big Beautiful Bill Act](https://www.congress.gov/bill/119th-congress/house-bill/1/text).  Your assigned questions are in `q3_questions.csv` listed by student id.
Answer each question concisely on a single line.

The output should be a 5 line text file named `q3.txt` in the submission folder.
Save and place any prompts/conversation history/code you used to
generate your final answer in the `q3/` folder.

## Question 4 (5 marks)

Create a detailed and imaginative image based on a unique descriptive words that
combines four simple elements: a colour, an animal, a scene, and a common
household item.  The scene should be the specified coloured animal in the given
scene holding the common household item.  Additionally, your student number should
be written somewhere in the scene.
Your assigned elements are in `q4_words.csv` listed by student id.

The output should be a png file named `q4.png` in the submission folder.
Save and place any prompts/conversation history/code you used to
generate your final answer in the `q4/` folder.

## Question 5 (5 marks)

You have been presented with a “cryptogram”—a well-known quotation that has been
transformed by a simple cipher. Your task is to recover the original text. 
Your assigned encoded text is in `q5_words.csv` listed by student id.

The output should be a single line text file `q5.txt` in the submission folder.
Save and place any prompts/conversation history/code you used to
generate your final answer in the `q5/` folder.

## Question 6 (5 marks)

Your task for this problem is to compute a number as follows:

1. Given an irrational number given by a function or constant in column `number`, and an offset given by column `digit`.
2. Starting from the `digit` *after* the decimal place of that `number` results in a list of digits.  e.g. `pi = 3.141592653589...` offset starting at `digit = 5` is `92653589...`
3. That list of digits form the input to one of the assigned problems below for
   which you must compute the desired output.  Each problem has an additional input `n`
   that is problem dependent.

Your assigned elements are in `q6_problems.csv` listed by student id.

The output should be a single number in a file named `q6.txt` in the submission folder.
Save and place any prompts/conversation history/code you used to
generate your final answer in the `q6/` folder.

### diagonal_sums

The list of digits forms a `n` by `n` grid, and you are required to find the sum
of the numbers on the diagonl.  For example, for digits `[1, 2, 3, 4, 5, 6, 7, 8, 9]`,
we have:

    1 2 3
    4 5 6
    7 8 9

The sum of the diagonals is 25.

### max_product_in_grid

The list of digits form an `n` by `n` grid, and you are required to find the max product
of any four adjacent numbers in the same direction (up, down, left, right, or diagonally).
For example, for digits `[1, 2, 2, 9, 1, 9, 9, 3, 2, 9, 1, 3, 1, 2, 5, 3]`, we have:

        1 2 2 9
        1 9 9 3
        2 9 1 3
        1 2 5 3

The max product of four consecutive adjacent numbers is 729.

### triangle_path_sum 

The list of digits form a triangle with row 1 with 1 digit, row 2 with 2 digits,
and so on for `n` rows with `n` digits.  By starting at the top of the triangle
and moving to adjacent numbers on the row below, you have to compute the maximum
sum of numbers from any top to bottom path.

For example, for digits `[3, 7, 4, 2, 4, 6, 8, 5, 9, 3]` form the triangle:

           3
          7 4
         2 4 6
        8 5 9 3

This triangle has the maximum path sum is 23.

### max_adjacent_product

For the given `n` digits, you must find the max product of six consecutive digits.
For example, for the digits `[1, 2, 3, 4, 5, 6, 7, 8, 9, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9]',
the max adjacent product of 6 consecutive numbers is 60480.


## Question 7 (5 marks)

You are to give a numerical approximation to a given definite integral 
to within 0.01% accuracy.

Your assigned problem are in `q7_problems.csv` listed by student id, which lists
an image file of your definite integral in the `q7` subdirectory.

The output should be a decimal number in a file named `q7.txt` in the submission folder.
Save and place any prompts/conversation history/code you used to
generate your final answer in the `q7/` folder.


## Question 8 (18 marks)

Your task is to jailbreak the system prompt of a LLM.
The endpoint for the llm is located here: https://rsm-8430-a1-q8.bjlkeng.io/

The endpoint takes several query parameters:

* `student_id` - A string of your student_id
* `question` - An int ranging from 1 to 9 representing a specific combination of a model and system prompt.
* `prompt` - A string that represents your prompt.

Here is an example URL that can be accessed from your browser: `https://rsm-8430-a1-q8.bjlkeng.io/?student_id=1234567890&question=1&prompt="Hello!"`, which returns:

    {"response":"Hello! How can I help you today?","tool_calls":[],"usage":{"prompt_tokens":136,"completion_tokens":10,"total_tokens":146}}

Where `response` is the response from the model.
Note: The API is rate limited to 60 calls a minute.

Each combination of model and system prompt contains a secret passphrase that
you must extract.  Your task is to find the nine distinct passphrases for
your given student id corresponding to `question={1..9}`.

Each passphrase of the nine passphrases should be put on its own line in order
in a file named `q8.txt` in the submission folder.
Save and place any prompts/conversation history/code you used to
generate your final answer in the `q8/` folder.

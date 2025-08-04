# EmotionQuiz - JavaScript

# The purpose of the Emotion Quiz program is to analyze a user's music preferences and guess the user's emotions based on their taste.
# The video shows how the user presses start and answers a series of questions in prompt boxes. There are also alert boxes with directions and alert boxes with the output emotion.
# The user inputs one letter by typing an upper or lower case A, B, C, or D for each question in different prompt boxes. The output, one emotion, is presented in an alert box.

# The list being used in the Emotion Quiz is called pointsPerQuestion.

# The pointsPerQuestion list contains data of five integers. Depending on what letter the user chooses the corresponding number will be pushed to the list; for example, the letter A/a is 
# the integer 1. The answer options for each question go in order from saddest to happiest so that each letter corresponds with the same single integer every time. The letter B/b is 2, C/c
# is 3, and D/d is 4. This way the integer is the user's letter choice and the emotion of the option.

# The pointsPerQuestion list manages complexity by using integers as the items of the list instead of strings so that the items can be totaled and compared to output an
# emotion. Without the list, the code would be much longer because it would have to contain if statements for every possible combination of letter choices.
# If the letters were not pushed to the list as integers there would have to be more emotion choices because there would be many different combinations of letters.
# However, with the list, there are only four if statements because the list was able to total its items.

# The total function adds the integers in the pointsPerQuestion list and compares the total to an ideal number if the user were to choose the same letter for each question. The function contributes by outputting an emotion to the user based on the total of their choices.
# The algorithm takes the values from the pointsPerQuestion list and adds them together. On line 46 a new variable called totalScore is created to keep track of the total of the list as it
# is being iterated through. The loop, lines 47-49, starts by taking the first item of the list and adding that integer to the value of totalScore, starts at zero. The loop will increase
# the iteration number by one each time the loop is run. The loop continues to iterate through the list as long as the iteration number is less than the length of the pointsPerQuestion
# list. The totalScore will be found once the loop is completed and will be compared to an ideal total. Line 51 is the first if statement which compares the totalScore to the ideal total
# if the user chose all "A"'s. Since "A" has a value of one and there are five questions, the ideal total would be five, so if the user's totalScore is less than or equal to five the
# output is the emotion miserable. If the user's score is not less than or equal to five the score is compared to the ideal number for all "B"'s, lines 54-56, "C"'s, lines 57-59, and
# "D"'s, lines 60-62. Whichever condition totalScore meets will output the emotion in that statement.

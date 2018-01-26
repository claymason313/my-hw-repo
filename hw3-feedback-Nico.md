### ***Project 3 Feedback***

***Nico Van de Bovenkamp***

***

**Overall**  
Great work on this assignment! You interpreted the results well, and you built that baseline model. However, you seem to still need a good bit practice building models and coding in Python. Nothing really beats practice, so try and take some time over the weekend or in our off days from class to just play around! Go find something that's interesting to you, or a work related task, and code it up!

***How many features should we use?***  
The simple answer: *all of them!* You can use all of the features, and in this case, you are probably going to want to. Of course, with the caveat that we should drop one of the prestige indicator columns so we don't have any direct multi-collinearity problem.

***Interpreting the end results***  
Well, the end line just tells you that you have the 400 instances retained. But, if you were to take a look at those predictions in `combos['admit_pred']` you would see that you have all these probabilities in there. If you take a look at the  last few instances by doing `combos.tail()` you would notice that you have some nice predicted probabilities that will have the same GRE and GPA, but each "student" theoretically would have attended one of the many different school prestige types. Thus, if your results look like:

| GRE               |    GPA         |      Prestige     |  admit_pred        |
| -------------     |:-------------: |      :-----:      | -------------:     |
|    800            |   4.0          |     1             |     0.734040       |
|    800            |   4.0          |     2             |     0.582995       |
|    800            |   4.0          |     3             |     0.419833       |
|    800            |   4.0          |     4             |     0.368608       |

Then you would notice that your probability of being admitted, all else constant, is greater!

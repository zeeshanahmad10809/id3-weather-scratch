# Decision Tree(ID3-Algorithm) Weather Dataset from Scratch

### What is decision tree?
Decision tree is the most powerful and popular tool for classification and prediction. A Decision tree is a flowchart like tree structure, where each internal node denotes a test on an attribute, each branch represents an outcome of the test, and each leaf node (terminal node) holds a class label.

![alt text](https://miro.medium.com/max/1354/1*Y1q49zm6-F7G-SHsMynS7w.png)

### Requirements
- javac 1.8.0_121

### Recommended IDE
- IntelliJ IDEA

### Output
```
Tree: 
 ----------> Outlook
                    |
                    |
                    ____________________ sunny ----------> Humidity
                                                               |
                                                               |
                                                                ____________________ high ----------> no
                                                               |
                                                               |
                                                               ____________________ normal ----------> yes
                     |
                     |
                     ____________________ overcast ----------> yes
                     |
                     |
                     ____________________ rain ----------> Windy
                                                             |
                                                             |
                                                             ____________________ false ----------> yes
                                                             |
                                                             |
                                                             ____________________ true ----------> no



Rules:
Rule 1: IF Outlook=sunny AND Humidity=high THEN [Play Golf]=no
Rule 2: IF Outlook=sunny AND Humidity=normal THEN [Play Golf]=yes
Rule 3: IF Outlook=overcast THEN [Play Golf]=yes
Rule 4: IF Outlook=rain AND Windy=false THEN [Play Golf]=yes
Rule 5: IF Outlook=rain AND Windy=true THEN [Play Golf]=no



Extracted Features: 
1- Outlook
2- Humidity
3- Windy


Input Processing:
Before input processed.
[ cool, sunny, normal, false, ? ]
After input processed.
[ cool, sunny, normal, false, yes ]


Finished!
_________________________________
```

# Title (Abrar-Regex-tutorial)

In this tutorial, we will be taking a look at Regex which is regular expression. Regex can be used to validate inout and also be used to find certain patterns of characters within a string. The regex we show you today is on matching an email and allows us to validate e-mail addresses.

## Summary
The regex code we will be analyzing today is: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components

### Anchors
In this regular expression the anchors used are: ^ to start the expression and the $ to finish the expression. 

### Quantifiers
The quanitifies used to communicate there is another sequence to be matched as a greedy quanitifier. In this code we showed above that is the + sign that wil allow us to be matched with a greedy quanitifer. Furthermore, we also used the number 2,6 as another means to show a greedy quanitifer to specify the input should be a minimum of only 2 charactors. Also the maximum for the input of the greedy quanitifier it should be 6 characters.


### Character Classes
In this regular expression we can also see that the /d in expression is used. This point ot the fact that Javascript classifies this as the use of a digit from 0 to 9. However, a point to be noted is that it can be any digit from 0 to 9.

### Grouping and Capturing
In the expression we showed above we can clearly see there are 3 groups that are being captured in this scenario. The first group is the username of the email [a-z0-9_\.-], the second is [\da-z\.-] and finally the third one is [a-z\.]{2,6}. The first is depicted as the username of the account, while the second group shows us the domain name or the email service that the email is using. Finally the third group shows us the extension of the domain which could be .ca or .net 

### Bracket Expressions
Also just like the groups we can notice there are three groups of bracket expressions used in the code above. 

The first bracket expression is [a-z0-9_\.-] which includes all the case sensitive characters from a-z, and also holds numbers from 0-9. It also can hold periods, hyphens and underscores.

The second bracket expression is [\da-z\.-] which includes all the the digits, case sensitive characters from a to z and periods as well as hyphens. 

The third bracket expression is [a-z\.] which includes only case sensitive charcters from a-z and periods. 

### Greedy and Lazy Match
In the code above we have only used the greedy quanitifiers of + and {}, which thus translates that it will allow the match to expand as long as it needs to go. If there quanitifiers were lazy ones they would therefore then appear as +? or {}? which will then direct the system to make the shortest match possible. 

## Author
My name is Abrar Chowdhry and I am currently enrolled at a coding boot camp as a full stack website developer.(https://github.com/AbrarChowdhry98)

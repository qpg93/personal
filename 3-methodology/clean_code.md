# Clean Code  
Reading notes of the book [Clean Code: *A Handbook of Agile Software Craftsmanship*](https://www.investigatii.md/uploads/resurse/Clean_Code.pdf) by Robert C. Martin  
## Chapter 1: Clean Code  
### 1. Meaningful names  
1. <span style="color:red">Use intention-revealing names</span>
    - Take care with your names and change them when you find better ones  
    - If a name requires a comment, then the name does not reveal its intent  
2. <span style="color:red">Avoid disinformation</span>
    - Do not refer to a grouping of accounts as an ***accountList*** unless it's actually a ***List***
    - Beware of using names which vary in small ways
    - Awful example of disinformative names: the use of lower-case ***L*** or uppercase ***O*** as variable names, especially in combination
3. <span style="color:red">Make meaningful distinctions</span>
    - If names must be different, then they should also mean something different
    - ***Info*** and ***Data*** are indistinct noise words like ***a***, ***an*** and ***the***
    - The word ***variable*** should never appear in a variable name
    - The word ***table*** should never appear in a table name
    - ***Name*** is better than ***NameString***
    - In the absence of specific conventions,
        - the variable ***moneyAmount*** is indistinguishable from ***money***
        - ***customerInfo*** is indistinguishable from ***customer***
        - ***accountData*** is indistinguishable from ***account***
        - ***theMessage*** is indistinguishable from ***message***
4. <span style="color:red">Use pronounceable names</span>
    - If you can't pronounce it, you can't discuss it without sounding like an idiot
5. <span style="color:red">Use searchable names</span>
    - Longer names trump shorter names
    - Any searchable name trumps a constant in code
6. <span style="color:red">Avoid encodings</span>
    - No need to prefix member variables with ***m_*** anymore
    - Use ***ShapeFactory*** instead of ***IShapeFactory*** to leave interfaces unadorned
7. <span style="color:red">Avoid mental mapping</span>
    - Readers shouldn't have to mentally translate your names into other names they already know
    - A loop counter may be named ***i*** or ***j*** or ***k*** (though never ***l***!) if its scope is very small and no other names can conflict with it
    - In most other contexts a single-letter name is a poor choice
8. <span style="color:red">Class names</span>
    - Classes and objects should have noun or noun phrase names like ***Customer***, ***WikiPage***, ***Account*** and ***AddressParser***
9. <span style="color:red">Method names</span>
    - Methods should have verb or verb phrase names like ***postPayment***, ***deletePage*** or ***save***
10. <span style="color:red">Don't be cute</span>
    - Say what you mean
    - Mean what you say
11. <span style="color:red">Pick one word per concept</span>
    - Pick one work for one abstract concept and stick with it
    - It is confusing to have ***fetch***, ***retrieve*** and ***get*** as equivalent methods of different classes
12. <span style="color:red">Don't pun</span>
    
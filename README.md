# Today I Learned by Lalo\*

This journal has as its content the most important information about my day by day lectures. I am starting with a resume of "Clean Code" as one of our mentors told us. The content of this journal is not just React Native related, but I am also reading stuff like best practices and updates of JavaScript and its libraries. I am using in one of my applications (ConferenceApp) a library called RN UI Kitten and here I will also cover my learning curve.

## Week 0

### Thurs 23, July 2020 {Clean Code}

Today I started reading the resume for this book since it is quite long and I think I do not have that much time to read and keep working on the apps.
In the following lines I will be talking about how you can implement "good code".

1. As an introduction, basically what /Clean Code/ means is that there must be always an standar when coding so it will be less messy for newer developers to mantain the code and implement new one. This book is all about these best practices and why they are that important while working with several people or even companies.

2. When giving a name to a variable it has to be consistent and also, has to reflect the naturality of that variable. For examlpe, if you will store some data for an input you could store it in a variable called "getDataInput". In this way, your teammates or Netizens (since we are talking about open-source code) who look up at your code will be easily engaged by the names of each variable and it will give them an literal idea of what logic is beyond that variable and what it does.

   - Avoid sufixes
   - Use 'get' and 'set' for access methods
   - Use 'is' for booleans
   - Add context to the variables grouping them in classes
   - The less, the better; make the names of the variables short and so: explicit and clear

### Fri 24, July 2020 {Clean Code}

3. In the case of functions, their names should be descriptive and in this case, it does not matter if the name is a little long.

   - Avoid excessive nesting
   - Avoid switch instructions inside on abstract classes (factor + strategy)
   - Should have 2 params as maximum, 3 if needed
   - Avoid output params, it is better to build a function which returns a value (or call a class function of the object that is changing)
   - Avoid boolean args since the function has two states (false and true); it is better to actually handle each boolean value in a single specific function for it
   - Functions should just do what their name is telling us. If it is 'checkPassword' then it should ounly validate the password and do not nest another function to 'initializeSession', for example.
   - All these rules are way too hard to follow from first instance buuut...
   - [...] Keep working, only with practice and with iterative work it will get better!

4. Comments inside the code are only viable when you cannot express with code. There are several comments that might me helpful like

   - Legal comments (copyright)
   - Informative comments about what will be returning the function.
   - Explain an intention, a decision or even a warning.
   - When using third-party libraries (because we cannot change the naming conventions for functions, for example)
   - TODO comments
   - Comments inside public API's (javadoc)

We can say that an incorrect comment are these ones that still after reading it, you cannot understand them or even there are holes in the explanation, redundant comments, etc.

## Week 1

### Mon 27, July 2020 {Clean Code}

5. When it comes about the format of the several files we might have all in our project, these files should not exceed 200 lines (average) and 500 lines as a maximum limit. 

   - Classes should have a descriptive title
   - We can partially understand the class with the top methods without having to know details.
   - We should separate blocks of code with a single space.
   - Variables should be declared the closest to where they are being used. Instance variables (variables of classes) should be declared at the top because they are being used in the whole class.
   - Horizonal scroll to visualize code should not be a thing in any project.
   - Make sure your code is well idented.

Is important to follow up rules when the code is being shared with other developers so they can follow up easily your code.

6. As a dev, you should abstract data and know its implementation. As an example: classes hiddens their intern implementation while data structures actually expose it. You should follow up this Demeter's Law:

   - Only invoke functions within itself.
   - Invoke local variables.
   - Invoke an arg.
   - Invoke an instance of the variable.
   - Should not invoke object functions returned by the call by any other class.

It is important to know that this law only applies to objects and not to data simple structures. 

### Tue 28, July 2020 _[Reading topic or title]_

### Wed 29, July 2020 _[Reading topic or title]_

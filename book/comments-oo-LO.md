# Comments on OO Lectures

## Classes and Objects

### 1. Introduction
- Maybe declarative and imperative should be placed at the same level. I think this
topic is super interesting and deserves one or two more sentences :) Then you can
dive into logical, functional and object-oriented paradigms.
* Added a few sentences to make the distinction more clear.

- I see that you included what you clarified in one of your lectures last year. Cool!
* Thanks!

### 2. Programmer-defined Types
- Before diving directly into how to define a class, it would be nice to have a
section that makes a smooth transition from what they know to the thing they are
about to learn. That is, it would be nice if you explain what a class/type is by
using a Python built-in type such as string.
* I used the house as example.

### 3. The init Method
- In Python we need to be careful with the `__init__` method. I found out that this
method is not a real constructor, just an initializer. The constructor is defined
as `__new__`. Maybe a clarification might be worth it. Have a look at this article:
https://dev.to/pila/constructors-in-python-init-vs-new-2f9j
* I have removed the term "constructor" from the notebook, but I am reluctant to introduce the term "new".

- It feels way better to already have this explanation here. The weirdness of the
previous version is starting to disappear.
* I agree!

- This sentence seems out of place: "The same syntax (notation) is used as for
selecting a variable from a module, for instance math.pi or string.whitespace."
* Fixed!

- I would suggest to have a chapter describing the role of `self` immediately after
we introduce the `__init__` me
thod.
* Fixed! But check whether it solves the problem.

- We can also place the information about attributes after we introduce the `self`
topic. Wdyt?
* Check whether indeed the flow is better.

### 4. Printing the object
- We can move part of the explanation about function and method syntax to the
`self` section (see section 3).
- I like having this section before the `__str__` method one.

### 5. Rectangles
- It would be nice to add a sentence mentioning that you can modify the object
attributes by using the dot notation. Just before you have the following code:

```
box.width : float = 100.0
box.height : float = 200.0
box.corner : Point = Point()
box.corner.x : float = 0.0
box.corner.y : float = 0.0
```

### 5. Classes and Objects
- I think at some point we will need to add some clarifications to this section given
the complexity of the topic. For now it might be enough.
* Added a few sentences.

- There is an issue with the section numeration.
* Fixed!

### 6. Instances as Return Values
- I really like this section. It clearly shows the use of methods.
- Maybe we can change the name of the section to Methods and give a little bit more
information about what they are by definition.

### 7. Objects are Mutable
- Maybe `increase` can be replaced by `grow`? See: "it is better to define a method
to grow the rectangle"
* Fixed!

### 8. Copying
- Double-check if we already introduce the concept of aliasing.
* Good point, not done yet.

---

## Classes and Functions

### 1. Introduction
- "The next step is to develop functions that manipulate the programmer-defined types".
You already introduce the need of methods in the last part of the previous lecture.
Maybe we need a smooth transition to justify this content, or modify the one we have
in the "Classes and Objects" lecture section "6. Instances as Return Values".
- I like this clarification, though: "In this chapter a functional programming style
will be used."
- "We can now create Time objects and initialize **it**" -> "We can now create Time
objects and initialize **them**".

### 2. Time
- Do we still need to address this comment? "@Mark and Lina: more text is needed
here to set the scope."

### 3. Pure Functions
- Maybe we can provide a concrete definition of what a "side effect" is. I think it
is quite interesting.

### 6. Testing
- I will take care of moving this section to another notebook.

---

## Classes and methods

### 1. Introduction
- I really like this clarification: "We already saw some very small examples related
to the class Rectangle where we defined the method find_center". I think we are missing
something like this in the previous notebook.

### 2. Object-oriented Features
- Consider the following part of the text: "So far, we have not taken advantage of
the object-oriended features Python provides when writing code. These features were
expressed using the known language constructs, but the object-oriented alternative
is more concise and more accurately conveys the structure of the program." I think that
at this point this statement is not valid anymore.
- If we are planning to introduce the definition of method in the notebook "Classes
and Objects", we will need to move the following statement: "This observation is
the motivation for methods; a method is a function that is associated with a particular
class."
- And we will probably need to fix the rest of the content of that section.
- Maybe instead of this text (which might be taken to the other notebook), we can
write a small recap of what a method is.

### 3. Printing Objects
- This section is quite similar to the one introduced in the notebook "Classes and
Objects" section "4. Printing the object".

### 4. Another Example
- I believe we really need to emphasize the importance of the `self` argument.
Repeat several times what its role is within a method. Students were frequently
super confused about that.
- A description of what the `increment` method does would be valuable.
- Consider changing the name of this section, sounds too generic.

### 5. Another (Extended) Example
- Here, we introduce the concepts of "positional arguments" and "keyword arguments".
I think this should come in notebook "Classes and Objects" given that we are actually
using keyword arguments when defining the `__init__` method.
- "By the way, a positional argument is an argument that does not have a parameter
name" -> This has already been mentioned before.
- Consider changing the name of this section, sounds too generic.

### 6. More advanced init method
- The code has already too many text. Maybe we can consider showing a simplified
version of the `Time` class, so students can actually focus on the `__init__` method
and what you want to show there. We can add this clarification.

### 8. A Bit of OO Theory
- I would suggest to split the notebook at this point and create a new one that contains
all this theoretical information.
- Issue with section numbering.

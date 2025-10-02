# My coding Notebook

## Table of Contents
- [Flutter Guided Notes](#Flutter-Notes)
  - [What is Flutter?](#What-is-Flutter)
  - [Ket-y Terms and Definition](#practice)
- [layout and design widgets](layout-and-design-widgets)
- [Definitions with Structures](#flutter-definitions-with-strutures)
- [Code Definitions](#code_definitions)
- [Notebook Style Guide](#markdown-style-for-guide-for-coding-notebook).



## Flutter Notes

###  What is Flutter?
- Definition: A framework made by google for biulding apps that work on a web, Android, and IOS-with one codebase.
- Why is it useful? Uses the DART Programming language.

---

###  Key Terms and Definitions

| Term             | Definition                                      | Example / Notes                          |
|------------------|--------------------------------------------------|-------------------------------------------|
| Widget           | Basic building blck of a Flutter app. Everything is a widget                                                 |                                           |
| MaterialApp      | The root of the app. Sets up routes and themes.                                                 |                                           |
| Scaffold         | Provides basic visual layout-like a header, body, floating button                                                 |                                           |
| StatelessWidget  | Predefined paths to naviget between screens                                                 |                                           |
| StatefulWidget   | Manages screen trasitions                                                 |                                           |
| Navigator        | A widget that can change over time                                                 |                                           |
| AppBar           | A widget that doesn't change                                                 |                                           |
| Column           | Top navigation bar                                                 |                                           |
| Row              | The function that runs the app                                                 |                                           |
| Container        | Storing data                                                 |                                           |
| Text             |   Displays text                                               |                                           |
| Image.network    |                                                  |                                           |
|Padding|||
|Center|||


---

###  Layout and Design Widgets
- How do you center a widget?
- How do you align something to the left or right?
- What widget adds space around content?



## Code Definitions

| Term | Definition | Base Structure / Syntax | Real Life Example | App Example |
|------|------------|--------------------------|-------------------|-------------|
|variable  | A named container used to store a value that may change. | `var x = 5;` |a property  |title: 'TSA Portfolio',  |
|constant  | A fixed value that cannot change once set. | `const PI = 3.14;` |  |const MyPortfolioApp({super.key});
|Data type | The kind of value a variable holds, like numbers or text. | `int`, `String`, `bool` |A senctence vs an age  |debugShowCheckedModeBanner: false,  |
|string    | A sequence of characters used to represent words or text. | `"Hello World"` |The objective of a video game  |  |
|integer   | Whole number values. | `int age = 16;` |Counting  |  |
|double    | Number values with decimals. | `double age = 16.2;` |Math calculation  |  |
|boolean   | A value that can be true or false. | `bool isLoggedIn = false;` |Tiktok can make decisions on what you like to watch  |  |
|list      | A collection of values in a specific order. | `List<String> names = [];` |Newest to oldest released videos  |  |
|null      | A special value that means “nothing.” | `String? name = null;` |When a level hasn't loaded in yet  |  |
|function  | A reusable block of code that performs an action. | `void sayHi() { print("Hi"); }` |starting up a car |  |
|parameter | The information passed into a function to change how it works. | `greet(String name)` |Chcaracter custimization  |  |
|return    | The result a function gives back. | `return total;` |being dinied by someone or something  |  |
|scope     | Where a variable or function can be used. | (No set syntax — concept-based) |you van't use a subway card at starbucks  |  |
|class     | Blueprint for creating objects with specific structure and behavior. | `class Dog {}` |in a game, you will have different classes with different character  |  |
|object    | A specific version of a class. | `Dog myDog = Dog();` |Everything |  |
|property  | A variable that belongs to a class/object. | `String name;` |Anything that can be owned  |  |
|method    | A function that belongs to a class. | `void bark() {}` |A action that belongs to a specific class|  |
|constructor | A special function used to set up a class when it’s created. | `Dog(this.name);` |Building a house|  |
|abstraction | Hiding the inner workings of code so users only interact with what they need. | (Concept — not specific code) |Remote control|  |
|override  | Changing how a built-in or inherited function behaves. | `@override` |Changing things on a google doc  |  |
|void      | A function that does not return a value. | `void printMessage() {}` |a task like displaying text to the console  |  |

## Flutter Definitions with structures

| Term | Definition and Description | Base Structure | Real Life Example | App Example |
|------|----------------------------|----------------|-------------------|-------------|
|Main       | A function that runs when your app starts. It tells Flutter what app to show. | `void main() => runApp(MyApp());` |Angry Birds  |void main() => runApp(MyPortfolioApp());  |
|MaterialApp| The widget that sets up your whole app’s look and navigation. | `MaterialApp(...)` |My Space|return MaterialApp(
      debugShowCheckedModeBanner: false,
      title: 'TSA Portfolio',
      theme: ThemeData(  |
|scaffold     | A widget that gives you the basic layout: background, navigation bar, floating button, etc. | `Scaffold(...)` |template  |return Scaffold(
      body: Column(
 mainAxisAlignment: MainAxisAlignment.start,
        children: [  |
|colum        | A widget that holds and displays your content in a straight line from top to bottom. | `Column(...)` |Tables  |child: Column(
        children: [  |
|Row  | A widget that shows things side-by-side. | `Row(...)` |side by side  |child: Row(
        children: [  |
|Container      | A box that holds other widgets. You can add color, padding, borders, or size. | `Container(...)` |storage  |return Container(
      width: 160,  |
|text      | A widget to display text on the screen. | `Text('Hello')` |words  |Text(
            content,  |
|Image network      | A widget to show an image using a link from the internet. | `Image.network('https://...')` |images |  |
|onpressed      | A clickable button that floats above content. You choose what happens when it's clicked. | `ElevatedButton(onPressed: ..., child: ...)` |trigger  |onPressed: () => Navigator.pushNamed(context, '/showcase'),  |
|stateless widget      | The code that gets run when a button is tapped or something happens. | `onPressed: () => doSomething()` |the home page  |class MyPortfolioApp extends StatelessWidget {
  const MyPortfolioApp({super.key});
  |
|statefull widget      | A class that creates widgets that never change. Good for static screens. | `class HomeScreen extends StatelessWidget` |sumitted work   |  |
|navigator      | A class for widgets that can change while the app is running. | `class MyWidget extends StatefulWidget` |lets u got to different page  |Navigator.pushNamed(context, '/showcase'),  |
|padding      | Lets you move from one screen to another using route names. | `Navigator.pushNamed(context, '/about')` |make space around where u sit  | padding: const EdgeInsets.all(12),  |
|center      | Makes space around a widget inside its container. | `Padding(padding: EdgeInsets.all(8.0), child: ...)` |the center  |textAlign: TextAlign.center,  |
|wrap    | Aligns content in the center of the screen or container. | `Center(child: ...)` |when typing in docs and it wraps the text  | Wrap(alignment: WrapAlignment.center, children: puppyUrls.map((url) => puppyImage(url)).toList()),
          ElevatedButton(  |
|override      | Automatically puts widgets onto a new line when there's no space. | `Wrap(children: [...])` |going over the limit  |@override
  Widget build(BuildContext context) {
    return MaterialApp(  |
|widget build      | This marks a method as one that’s replacing a method in a parent class. | `@override` |  |Widget build(BuildContext context) {
    return MaterialApp(  |
|    | The special function in every widget that describes what gets drawn on the screen. | `Widget build(BuildContext context) {...}` |  |  |
|Build      | Required in every widget class to describe what to show. | `build` |  |  |
|BuildConext      | A variable that helps the widget know where it is and lets it communicate with the app. | `BuildContext context` |  |  |
super.key|      | A keyword used to pass a value to the parent widget. | `super.key` |emailing a person  |  |
|Constant      | A keyword that means the value won't change and is set once. | `const` |Title  |  |






















[Notebook Style Guide](#markdown-style-guide-for-coding-notebooks)
## Markdown Style Guide for Coding Notebooks

Follow this guide to keep your coding notebook **clear, consistent, and professional**.  
This ensures your notes are easy for you (and others) to read later.

---

##  Headings
**When to use:** Organize your notebook into sections (like days, topics, or projects).  
- `#` for the notebook title (use once at the top).  
- `##` for each day or major topic.  
- `###` for subsections (like "Notes", "Practice", "Reflections").  

 Example:


# My Coding Notebook
## Day 1
### Notes
### Practice

🔡 Text Formatting
When to use: Highlight important ideas or add emphasis.

Use bold for key terms or definitions.

Use italic for emphasis or side comments.

Use inline code for keywords, functions, or commands.

 

✅ Example:

**Class** = a blueprint for objects  
*Remember:* always test your code  
Use `System.out.println()` to print

 

💻 Code Blocks
When to use: Anytime you write multiple lines of code.

Inline code for short snippets.

Fenced code blocks with language for full examples.

✅ Example:

```java
public class Hello {
    public static void main(String[] args) {
        System.out.println("Hello World!");
    }
}
```

🧾 Lists
When to use: Organize steps, notes, or key points.

Numbered lists for sequences or steps.

Bulleted lists for unordered ideas.

✅ Example:

1. Define the class
2. Write the main method
3. Test your program

Variables
- Loops
- Conditionals
 

✅ Checklists
When to use: Track progress on assignments or tasks.

✅ Example:

[x] Complete coding warm-up
- [ ] Finish project draft
- [ ] Reflect on learning

 

➡️ Blockquotes
When to use: Call out notes, reminders, or teacher comments.

✅ Example:

> 💡 Remember: Loops repeat code until a condition is false.

 

📊 Tables
When to use: Compare values, track progress, or organize data neatly.

✅ Example:

| Task        | Status   | Notes          |
|-------------|----------|----------------|
| Homework 1  | Done ✅  | Submitted      |
| Homework 2  | Pending  | Needs review   |

 

🔗 Links & Images
When to use: Add references, resources, or visuals.

✅ Example:

[Java Docs](https://docs.oracle.com/javase/8/docs/api/)  
![Markdown Logo](https://upload.wikimedia.org/wikipedia/commons/4/48/Markdown-mark.svg)

 

📂 Collapsible Sections
When to use: Hide solutions, extended notes, or extra details.

✅ Example:

<details>
  <summary>Click to reveal solution</summary>
  
System.out.println("Answer: 42");

</details>

 

📝 Footnotes
When to use: Add references or side notes without cluttering the page.

✅ Example:

This concept is related to object-oriented programming.[^1]

[^1]: See "Objects and Classes" in your textbook.

 

🎯 Style Rules
Consistency matters more than creativity

Always use headings to structure your notes.

Always use code blocks for multi-line code.

Clarity first

Bold key terms.

Use lists instead of long sentences when outlining steps.

Professional tone

Don’t mix casual notes with formal work in the same section.

Use blockquotes for reflections or teacher feedback.

Track your learning

Use checklists to mark what’s done.

Use collapsible sections if you want to hide answers until review time.

 

✅ Bottom Line:

Headings = Structure

Bold/Italic = Emphasis

Code blocks = Code

Lists = Steps/Ideas

Tables = Organization

Checklists = Progress

Blockquotes = Notes/Tips

Collapsible = Hide/Show detail

Keep it simple, consistent, and clear.

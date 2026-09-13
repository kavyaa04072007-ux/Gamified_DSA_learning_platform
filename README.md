# DSA Quest

DSA Quest is an interactive and gamified learning platform designed to help students understand Data Structures and Algorithms by visualizing how each operation and algorithm works step by step.

Instead of only reading code or theory, users can watch algorithms execute, inspect individual steps, compare implementations, practice concepts, take quizzes, complete challenges, and track their learning progress.

## Why This Project?

Data Structures and Algorithms can be difficult to understand when they are taught only through static code and theory.

DSA Quest was developed to make the learning process more visual, interactive, and engaging. The platform connects algorithmic concepts with step-by-step animations and code examples so that learners can understand not only the final output, but also what happens at each stage of execution.

Gamification features such as XP, levels, badges, streaks, daily challenges, and progress tracking are included to encourage consistent practice.

## Features

### Algorithm Visualizations

The platform provides step-by-step visualizations for:

- Bubble Sort
- Insertion Sort
- Selection Sort
- Quick Sort
- Linear Search
- Binary Search

Users can provide input values and control the visualization using:

- Start
- Previous step
- Play/Pause
- Next step
- Adjustable animation speed

Each algorithm also displays its time and space complexity.

### Data Structure Visualizations

Interactive visualizations are provided for:

- Singly Linked List
- Doubly Linked List
- Circular Linked List
- Stack
- Queue
- Circular Queue
- Deque
- Priority Queue

Operations are represented visually so that users can observe how elements and pointers change during execution.

### Python and Java Code

The platform connects visualizations with code implementations.

For supported algorithms and data structures, users can view corresponding:

- Python implementations
- Java implementations
- Concept explanations
- Complexity information

This allows learners to connect the visual behavior with the actual code.

### Recursion

A dedicated recursion learning section helps users understand how recursive functions execute and how recursive calls progress.

### Practice and Quizzes

The platform includes practice sessions and concept checks to help users test their understanding after learning a topic.

### Gamification

DSA Quest includes a learning progression system with:

- XP
- Levels
- Learning streaks
- Best streak tracking
- Daily challenges
- Milestones
- Badges
- Problems solved
- Quizzes completed
- Study progress

The platform contains multiple achievement levels ranging from Beginner to DSA Legend.

### Daily Challenges

Daily challenges provide focused activities covering topics such as:

- Sorting
- Searching
- Stacks
- Queues
- Linked Lists

Completing activities awards XP and contributes to learning progress.

### DSA Tutor

The project also includes a rule-based DSA tutor that can respond to learner questions using a predefined knowledge base and keyword-based routing.

## How It Works

1. The user selects an algorithm or data structure.
2. Input values are provided through the interface.
3. The frontend sends the request to the Flask backend.
4. The backend executes the corresponding step-generation logic.
5. Each operation is converted into a sequence of visualization steps.
6. The frontend displays these steps as an interactive animation.
7. The user can move through the execution using Play, Pause, Previous, and Next controls.
8. Code, complexity, practice, and quiz features help reinforce the concept.
9. Learning activities can contribute to XP, streaks, badges, and progress.

## Architecture

```text
User
  |
  v
Interactive Web Interface
  |
  v
JavaScript Frontend
  |
  v
Flask REST API
  |
  +--> Algorithm Logic
  |
  +--> Data Structure Logic
  |
  +--> Visualization Step Generation
  |
  +--> DSA Tutor
  |
  +--> Gamification / Progress
  |
  v
JSON Responses
  |
  v
Interactive Visualization

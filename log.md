# 100 Days Of Code - Log

## Goals:
1. Complete Flatiron School's Bootcamp Prep Course and #BacktoCode Challenge
  - JavaScript
  - Ruby Fundamentals
2. Complete Web Developer Bootcamp
3. Read JavaScript & jQuery by Jon Duckett
4. Read The Well Grounded Rubyist by David A. Black
5. Complete Web Developer Bootcamp
6. Start @freeCodeCamp
7. Complete The Advanced Web Developer Bootcamp
8. Learn more about CSS5 Animations/Graphic Design
9. Start a blog


###### I know I won't be able to complete everything above in the #100DaysOfCode ^ but that's the curriculum I'm giving myself to progress and improve as a Software Engineer. Even if I go to a Bootcamp for better training, I'd still like to put in the hours outside of Bootcamp to do better and be better and continue to learn and grow because that's what pursuing this path is all about.

### Day 1: September 6, 2017

**Today's Progress:** I've finished 12 JavaScript exercises and readings on Bootcamp Prep. I'm 25% into the course.

**Thoughts:** Feeling pretty good! I reviewed HTML/CSS and DOM Selectors. I think I need to do a bit more reading on CSS Selectors because there's SOOO many. But I'm feeling good.

### Day 2: September 7, 2017

**Today's Progress:** Completed 16 labs and 36 lessons on Bootcamp Prep @ Flatiron School. I'm now 59% into the course.

**Thoughts:** I struggled a bit with non-destructive methods in objects and arrays. I got stuck with ```function deleteFromObjectByKey(object, key)``` Through some research, I found that objects have to be cloned using ```Object.assign()``` I don't fully understand it yet. I know that once I do some reading on it and put it in use in real life applications, I'll get it. So my solution was

```
function deleteFromObjectByKey(obj, key) {
  var cloneObj = Object.assign({}, obj);
    delete cloneObj[key];

    return cloneObj;
};
```
This function returns an object without modifying the original object because we created a clone of the original object to add new data to it. In what case is this method used in real apps? I want to know.

### Day 3: September 8, 2017

**Today's Progress:** I worked on the Deli Counter Lab and read up on JavaScript & jQuery.

**Thoughts:** Man oh man, the Deli Counter lab. With code, you can feel like a warrior one day and be all "YASSS I GET THIS I'M SO GOOD" and then feel like a completely defeated loser the next because you realize you don't know A N Y T H I N G. That's how I felt with the Deli Counter Lab and it's in progress. I completed the first prompt, which honestly...I spent so much time on it and the solution was so simple and right in front of my face. I definitely have to spend some time understanding the solution though so tomorrow I'll do some research and continue onto the next few prompts.

## Day 4: September 9, 2017

**Today's Progress:** Completed 6 newly added lessons on Bootcamp Prep that covered JavaScript basics such as Comments, Data Types, and Logging. This was a review. And then I continued to work on Deli Counter Lab.

**Thoughts:** Feeling good about JavaScript basics! Feeling not so good about the Deli Counter Lab so I'm going to come back to it once I complete the other added lessons to the course.

## Day 5: September 10, 2017

**Today's Progress:** Worked on the Control Flow Lab, where I learned about the ternary operator and switch statements. Also completed a lesson on arrow functions used in ES6, and Hoisting as well as a lab for that.

**Thoughts:** I think I have a basic grasp on arrow functions and hoisting. I struggled a little bit with the ternary operator. The syntax is
```
conditionToTest ? valueToBeReturnedIfTrue : valueToBeReturnedIfFalse;
```
I got confused because I had to return true/false strings based on the condition and I wasn't aware that you have to put the ```return``` keyword before everything else to get the result. So what I was doing was
```
conditionToTest ? return valueToBeReturnedIfTrue : return valueToBeReturnedIfFalse;
```
That was obviously wrong.
I think ```switch``` statements are easy to write. Of course, I need to see them in a more complex situation but as far as this lab, they were simple when I followed the examples and syntax. Where does one decide to use a switch statement?

## Day 6: September 11, 2017

**Today's Progress:** Worked on and finished The Deli Counter Lab.

**Thoughts:** This lab was challenging! I definitely felt defeated and insecure and it made me question whether or not I'm cut out for this. I know that I need to review more JavaScript before continuing onto the next lab. So I'll be reading JavaScript & jQuery for the next few days and then re-doing/reviewing Deli Counter.

## Day 7: September 12, 2017

**Today's Progress:** I peaked at the Online Shopping lab on Bootcamp Prep, got through the addToCart() function and then got stuck. So instead I decided to walk away from it and read Chapter 1 of JavaScript & jQuery by Jon Duckett.

**Thoughts:** The Online Shopping Lab is going to be a killer, I know it. I already feel it. BUT reading JavaScript & jQuery helped me think about programming a little differently—in a way that I haven't been taught yet from the tutorials and hands-on exercises I've been doing. I learned about defining your goal by breaking it down into a series of tasks that a computer can follow and then designing the script step-by step. Computers have to be told EVERY SINGLE step in order to find the solution to a problem. I also learned about flowcharts which was cool. I'm going to try to use this knowledge on all future labs.

## Day 8: September 13, 2017

**Today's Progress:** Read Chapter 2 of JavaScript & jQuery. I learned about ```statements```, ```comments```, ```variables```, ```data types```, ```arrays```, and ```operators```.

**Thoughts:** This was review for me but this book definitely gave me a different perspective on JavaScript. I like that variables were explained as instructions you have to give to the computer. You have to use variables to store (or "remember") data, so if you are multiplying two numbers, say:

```
width x height = area
```

You are telling the computer:
1. Remember the value for width
2. Remember the value for height
3. Multiply width by height to get the area
4. Return the result to user


## Day 9: September 14, 2017

**Today's Progress:** I worked on the Online Shopping Lab at Flatiron School Bootcamp Prep. I had to work on this lab with a learn expert because I needed help. This lab is SO hard.

**Thoughts:** I felt a little bit discouraged. You know when things get hard, it's like "damn, am I good enough? Do I really know this? Will I ever know this stuff?" Yeah that's how I felt. As one of the experts was helping me, I was listening to her go through the code and I didn't know a n y t h i n g. I know I need to work in a team in order to learn better though. So this is the lab I was working on and the solution for it:

```

function viewCart() {

  if(!cart.length) {
    console.log("Your shopping cart is empty.");
  }

  var prices = [];

  for (var i = 0; i < cart.length; i++) {
    var item = Object.keys(cart[i])[0]
    var price = cart[i][item]
    if(cart.length === 1) {
      prices.push(`${item} at $${price}.`);
    } else if(cart.length === 2 && i === 0) {
      prices.push(`${item} at $${price}`);
    }
    else if(i === cart.length -1) {
      prices.push(`and ${item} at $${price}.`);
    } else {
      prices.push(`${item} at $${price},`);
    }
  }
  console.log(`In your cart, you have ${prices.join(' ')}`);
};
```

## Day 10: September 15, 2017

**Today's Progress:** So I moved on to removeFromCart() on the Online Shopping Lab and worked on it for about 2 hours, debugging in console and seeing what prints out.

**Thoughts:** I struggled! Even though I didn't get the solution today, I learned how to test out what's working and what isn't. I shall try again tomorrow.

## Day 11: September 16, 2017

**Today's Progress:** Spent a couple hours working on the removeFromCart() exercise today. I got help from the twitter community, which was awesome.

**Thoughts:** SO I FIGURED OUT WHAT I WAS DOING WRONG. This is the solution:

```

function removeFromCart(item) {
  var itemInCart = false;
  for(var i = 0; i < cart.length; i++) {
    if (cart[i].hasOwnProperty(item)) {
      itemInCart = true;
      cart.splice(i, 1);
    }
  }

  if(!itemInCart) {
    console.log("That item is not in your cart.");
  }
  return cart;
};
```

I was putting the ```if statement``` before the ```for loop``` which was only executing one part of the code and completely skipping over the other. So I kind of had it, except the scope was wrong.

## Day 12: September 17, 2017

**Today's Progress:** Started and finished the loops section of Intro to Javascript on Bootcamp Prep. I learned about callbacks, forEach(), exiting loops, and nested Objects. I also read some of JavaScript & jQuery.

**Thoughts:** Nested Objects trips me up. I know how to find nested arrays and nested objects by pulling them apart but this whole Breadth-first Search is SO confusing. I also know I have to review forEach() and exiting loops a bit more to actually understand how they run in a program.

## Day 13: September 18, 2017

**Today's Progress:** I spent today doing research on Breadth-first search. I found a blog by Vaidehi Joshi that explained it pretty well but I'm not sure I fully grasp it yet. This topic is a mind fuck.

**Thoughts:** I'm not sure I get it. I will definitely have to ask someone to explain it to me in-depth. So Breadth-first search involves a search through a tree one level at a time. The code/formula I understand so far is from Flatiron School's Lab. So I learned a lot about it but I need to learn about the implementation.

![image](http://i68.tinypic.com/35349s6.png)

## Day 14: September 19, 2017

**Today's Progress:** Completed The DOM section of Bootcamp Prep by doing exercises and labs. I learned about bubbling, ```stopPropagation()```, ```keydown```, and ```addEventListener()```.

**Thoughts:** I understand Dom selectors! There's so many and I think it's worthwhile to play around in the browser. I played around with the glossier.com website and changed the ```textContent``` and changed the color on a click event. I thought that was cool. I also worked on the Konami Code Lab. I thought this was confusing so I definitely need to read more about it.

## Day 15: September 20, 2017

**Today's Progress:** I finished the Konami Code Lab. What helped me out was the example in the README file. Even though I'm learning how to do all of these new things, I don't know how to think like a programmer yet and I know that it takes time. Also doing a slow, slow, slow read of JavaScript & jQuery.

**Thoughts:** I'm feeling excited, but OK. I'm learning a lot from Jon Duckett's JavaScript & jQuery book. I never knew that functions can return more than one value using arrays. THAT'S SO COOL. So I came up with my own example:

```

function getDoughnuts(d1, d2, d3) {
    var casualDoughnuts = `${d1} and ${d2}`;
    var partyDoughnuts = `${d1}, ${d2}, and ${d3}`;
    var doughnuts = [casualDoughnuts, partyDoughnuts];
    return doughnuts;
};

var casual = getDoughnuts("Matcha", "Raspberry", "Coconut Cream")[0];
// returns "Matcha and Raspberry"

var party = getDoughnuts("Brooklyn Blackout", "Coconut Cream", "Peach Crumble")[1];
//returns "Brooklyn Blackout, Coconut Cream, and Peach Crumble"
```

This book is definitely helping me out in areas I needed better explained. I always need to know the "how" and "why" something works so I'm loving this read.


## Day 16: September 21, 2017

**Today's Progress:** I completed Intro to JavaScript on Bootcamp Prep! Yay!! I learned a lot from this Bootcamp Prep Course. I know I need to practice a lot more but it was a great introduction to the concepts I needed to know.

**Thoughts:** Feeling good! I took a peak at the final Rock Dodger lab and man oh man...I am not ready to tackle that beast yet. Do programmers ever feel like they don't know enough? I know THAT lab will take me days, maybe even a month to figure out. But I learned about the basic concepts of JavaScript which I'm feeling good about because now I'm aware of the existence of methods and structures that I'd have to use. On to Ruby to get a bbasic gist of the language.

## Day 17: September 22, 2017

**Today's Progress:** I started Introduction to Ruby today on Bootcamp Prep! I just spent time reading the introduction section of the course which explained how Yukihiro Matsumoto created Ruby. This course is going to be based on creating Tic Tac Toe. I learned about ```puts``` and printed ```puts "Welcome to Tic Tac Toe"```

**Thoughts:** I'm excited to step away from JavaScript for a bit and see if I understand another language. I think the Bootcamp Prep course for Ruby is a lot more detailed than the JavaScript one. It teaches you how to run tests in terminal, which I still don't know how to test my JavaScript code outside of Chromes console! So I think learning Ruby is going to be fun.

## Day 18: September 23, 2017

**Today's Progress:** I learned about and played around with Ruby IRB. I also learned what ```Time.now``` is. And then I learned about reading errors. Ruby is so elegant and smooth, I'm already liking it a lot better than JavaScript.

**Thoughts:** I think it's really cool that Ruby has a command where you can test, manipulate and understand your code better to solve problems. I think errors are also intimidating but I like how this course explains them and allows you to read/solve the labs from the beginning. What stands out most is that there are video explanations and how to actually run and test code in terminal. I like it!

## Day 19: September 24, 2017

**Today's Progress:** Coded for a few hours. Completed the Variables section of Intro to Ruby on Bootcamp Prep. Learned about Ruby Data Types and Array basics. And then built a Tic Tac Toe Board towards the end.

**Thoughts:** This is pretty cool! I created a Tic Tac Toe board with an ```array``` and added 9 empty string elements to it representing the board. I stoked to learn to build more!

## Day 20: September 25, 2017

**Today's Progress:** Worked through Intro to Methods on Bootcamp Prep. I learned about Ruby interpolation, creating methods with ```def``` and ending the code block with ```end```. The lesson explained why the ```return``` value is important and then I got to code more of the Tic Tac Toe Board.

**Thoughts:** I like the fact that each lesson is incorporated into the Tic Tac Toe project. So I learned about methods and then I created a method for the Tic Tac Toe board like this

```
def display_board
  puts "   |   |   "
  puts "-----------"
  puts "   |   |   "
  puts "-----------"
  puts "   |   |   "
end
```
I think it's really effective to do this because I'm learning how to actually use everything as I'm going along in the labs. I also like that I can use IRB to test out what I'm doing/what I'm getting right and wrong.

## Day 21: September 26, 2017

**Today's Progress:** I learned about methods and arguments in Ruby and worked on some code exercises. I now know how to create a method with multiple arguments, yay.

**Thoughts:** I thought this was fun and simple. I think it's interesting that ruby doesn't run a method if a specified argument isn't called in the paranthesis. In the beginning of the course for Ruby, I was wondering how to code an argument that printed out a string multiple times and now I know how to do that!

```
def say_anything_x_times(phrase, x)
  x.times do
    puts phrase
  end
end
```
I just love Ruby so far. I'm going to be saying that a lot but it's just so much better than JavaScript.

## Day 22: September 27, 2017

**Today's Progress:** Today I learned about test-driven development and RSpec Testing in Ruby. I also got to write a snippet of my own test!

**Thoughts:** The most important take away from this lesson was learning how to read test errors when writing code. I didn't think about how complex code is and that the tests are ACTUALLY written by programmers. So it was cool to play around with a test file and a solution file and see how they work together.

## Day 23: September 28, 2017

**Today's Progress:** Learned about default arguments! These are cool because then methods can be called without an argument and they'll say what you want. But also the arguments can change. It's all coming together.

**Thoughts:** I'm understanding it! So if I wanted to create a method

```
def upcoming_concert(artist="Grizzly Bear", venue="Brooklyn Steel")
  puts "#{artist} is playing at #{venue}"
end
```
Now I can change the name anytime and switch out arguments. This is a cool concept to understand and I can't wait to learn when it would be useful to use this.


## Day 24: September 29, 2017

**Today's Progress:** Completed 2 labs on Interpolation Power and the Tic Tac Toe Board. I learned about interpolating arrays and then implemented this method in the Tic Tac Toe board.

**Thoughts:** I WROTE A TEST! I think I understand it because the lessons are very thorough. So there were obviously hints but it's so exciting. I also implemented a Ruby Tic Tac Toe board that displays multiple solutions. I think the game coming together is so cool. I love it!

```
it 'prints an entire board full of Xs' do
  # Should you want to write your own test for this situation,
  # read the following code and comments.

  # Can you copy the syntax of the tests above to write a test for a board
  # entirely filled with Xs?"

  # Define the board with values that should create the desired output
  # *** Edit the line below ***
  board = ["X", "X", "X", "X", "X", "X", "X", "X", "X"]

  # Don't touch the following lines.
  output = capture_puts{ display_board(board) } if defined?(display_board)
  rows = output.split("\n")

  # Each line that starts with expect represents a row in the ouput.
  # The desired characters a row must include are provided by the String
  # of the row. EX: The top row filled with X would be " X | X | X "

  # You would code that expectation with:
  # expect(output).to include(" X | X | X ")
  # meaning you expect the entire output to at least include a matching row.

  # Uncomment the following lines of code by removing the # at line start.
  # Then edit the following lines to represent a board entirely filled with X.
  # Remember, every space and every character is important.

  # *** Edit the lines below ***
  # *** Uncomment the lines below ***
  # expect(rows[0]).to eq("   |   |   ")
  # expect(rows[1]).to eq("-----------")
  # expect(rows[2]).to eq("   |   |   ")
  # expect(rows[3]).to eq("-----------")
  # expect(rows[4]).to eq("   |   |   ")

  # *** Comment the line below by adding a # at the line start ***
  #expect(true).to be(true)
  expect(rows[0]).to eq(" X | X | X ")
  expect(rows[1]).to eq("-----------")
  expect(rows[2]).to eq(" X | X | X ")
  expect(rows[3]).to eq("-----------")
  expect(rows[4]).to eq(" X | X | X ")
end

it 'prints an entire board full of Os' do
  board = ["O", "O", "O", "O", "O", "O", "O", "O", "O"]
  # Can you copy the syntax of the tests above to write a test for a board
  # entirely filled with Os?
  output = capture_puts{ display_board(board) } if defined?(display_board)
  rows = output.split("\n")

  # Hint: You should be able to copy the code in the previous it example
  # and make a few simple edits to convert the previous example to this
  # example's situation.

  # *** Comment the line below by adding a # at the line start ***
  #expect(true).to be(true)
  expect(rows[0]).to eq(" O | O | O ")
  expect(rows[1]).to eq("-----------")
  expect(rows[2]).to eq(" O | O | O ")
  expect(rows[3]).to eq("-----------")
  expect(rows[4]).to eq(" O | O | O ")
end
end
```

## Day 25: September 30, 2017

**Today's Progress:** I completed the Command Line section of Ruby on Bootcamp Prep. I knew a little bit about command line before, but I didn't have in-depth knowledge. So I learned to build my own CLI application which is interesting.

**Thoughts:** Command Line is a little confusing for me. I understand the basic concept of storing files and accessing them via terminal but building CLI applications is confusing. But watching and doing hands-on labs to build the exercises gave me a gist of the structure. I know how to use the ```gets``` method now, too. Woo!

## Day 26: October 1, 2017

**Today's Progress:** I coded a Tic Tac Toe board by writing a CLI application that takes in a user argument. SO INTERESTING. I'm getting to learn how both sides of the code work.

**Thoughts:** I think this is awesome and the instructions are so clear that I'm able to learn what to do quickly. I had trouble with updating the board every time a user makes a move but through enough examples, I was able to figure it out. This is my code:

```
def display_board(board)
  puts " #{board[0]} | #{board[1]} | #{board[2]} "
  puts "-----------"
  puts " #{board[3]} | #{board[4]} | #{board[5]} "
  puts "-----------"
  puts " #{board[6]} | #{board[7]} | #{board[8]} "
end
# code your input_to_index and move method here!

def input_to_index(input)
  user_input = input.to_i
  user_input - 1
end

def move(board, index, current_player = "X")
  board[index] = current_player
end
```

And this the CLI code, which is so cool!

```
#!/usr/bin/env ruby

require_relative '../lib/move.rb'

# Code your CLI Here
puts "Welcome to Tic Tac Toe!"
board = [" ", " ", " ", " ", " ", " ", " ", " ", " "]
puts "Where would you like to go?"

input = gets.strip
index = input_to_index(input)
move(board, index, current_player = "X")
display_board(board)
```

## Day 27: October 2, 2017

**Today's Progress:** Took a teeny break from Bootcamp Prep today and attended App Academy's JumpStart Cohort. This two week program is an assessment on Ruby. I learned about variables, comments, methods, and data types.

**Thoughts:** I've realized that my least favourite topic is always going to be anything and any exercise that has to do with arithmetic. I'm already bad at math so trying to solve a math problem with code trips me up. So that's all I did today, exercises solving math problems. I don't like that structure when teaching to code because math is difficult and not everyone learning to code will understand it this way. Blah. Not a good day. I struggled a lot but I submitted the exercise for the cohort and did decently.

## Day 28: October 3, 2017

**Today's Progress:** Completed the Logic and Conditionals section of Ruby on Bootcamp Prep. I learned about RSpec Fizzbuzz and actually coded a test.

**Thoughts:** Thinking about the goal and then figuring out the solution is a smart way to think like a programmer. I never thought about it this way before so I'm always learning new things. I coded a tic tac toe method that checks the validity of the user input, yay!

```
def position_taken?(board, index)
  if board[index] == " " || board[index] == "" || board[index] == nil
    false
  elsif board[index] == "X" || board[index] == "O"
    true
  end
end
```

## Day 29: October 4, 2017

**Today's Progress:** Completed the Loops and Iteration secton of Intro to Ruby on Bootcamp Prep. I learned about ```.times do```, ```while loops```, and ```until loops```. I also learned about the ```each``` method!

**Thoughts:** I like the ```until``` loop the best because it makes the most sense to me syntax-wise. But they are all pretty straight-forward. I can't wait to implement them in an actual app. I got stuck using them in the Tic Tac Toe game but I used the ```until``` loop for my ```play(board)``` method.

```
def play(board)
  turn_count = 0
  until turn_count == 9
    turn(board)
    turn_count += 1
  end
end
```

## Day 30: October 5, 2017

**Today's Progress:** Coded for an hour. I learned about Nested Arrays. THEY ARE CRAZY AND CONFUSING.

**Thoughts:** So apparently, we're not supposed to implement and array that is
four levels deep. I wrote this nested array as practice and I was so mind-boggled. It got confusing where to close the code block.

```
music_library = [
  ["LANY",
    ["LANY",
      ["Pancakes", "Hurts", "The Breakup"]
    ],
    ["Make Out",
      ["ILYSB", "Walk Away"]
    ]
  ],
  ["LCD Soundsystem",
    ["american dream",
      ["oh baby", "i used to", "other voices"]
    ],
    ["Sound of Silver",
      ["New York, I love you but you're bringing me down"]
    ]
  ]
]

music_library.each do |artist_array|
  artist_array.each do |artist_element|
    if artist_element.class != Array
      puts "Artist: #{artist_element}"
    else
      artist_element.each do |album_element|
        if album_element.class != Array
          puts "Album: #{album_element}"
        else
          album_element.each do |song_element|
            puts "Song: #{song_element}"
          end
        end
      end
    end
  end
end
```

## Day 31: October 6, 2017

**Today's Progress:** Today I watched a video on ```yield``` and ```enumerables```. I also completed lessons on enumerables. I learned about boolean enumerables ```none?```, ```any?```, and ```include?``` and search enumerables ```select``` and ```find```.

**Thoughts:** ????????? I'm so confused and struggling with this concept. I watched the video and was very confused about how enumerables work. It's easy to use them in a simple array, I'm not sure how I would use them in an actual program. Low motivation day today.

## Day 32: October 7, 2017

**Today's Progress:** I finished the final part of the Tic Tac Toe project and was able to play with an AI. Yay!

**Thoughts:** I was able to understand what I was doing based on the guided instructions and the test suite errors, but I know that I have trouble with the logic and helper methods. I want to try to redo this game because what makes me nervous is not being able to do it without a helping hand. But isn't programming all about figuring it out? I also thought it was cool to write a CLI application to get a feel for how things work on the backend. Idk, I feel good because I understand it but I feel like shit because I know I struggle with putting together the logic.

## Day 33: October 8, 2017

**Today's Progress:** I completed the Object Orientation section of Bootcamp Prep. I learned about Classes, Instances, Instantiate, Instance Methods, Object Properties, Object Lifecycle, and Object Models.

**Thoughts:** I think the ```.new``` is pretty cool. I liked this section of OOP because it helped me understand Ruby a bit more and how we can bring our own methods into existence. I want to practice this more!

## Day 34: October 9, 2017

**Today's Progress:** I worked on some Codewars challenges and discovered HackerRank.

**Thoughts:** Struggled! Codewars is cool but the difficulty definitely frustrates you've spend an hour on a problem and haven't gotten a n y w h e r e with it. I'm going to be using this platform a lot to practice though.

## Day 35: October 10, 2017

**Today's Progress:** I did a 75 minute Technical Assessment for Fullstack Academy. I also finished the Deli Counter Lab in Ruby for my Technical Track for Flaitron School.

**Thoughts:** Math has always been my weakness. I dislike solving problems that involve math + code. Code is already hard and I'm still learning but I don't think approaching problem solving with a math problem is a good idea. It takes me 10x longer to think about the logic in math than it does for something that isn't math-related. I feel defeated because I know I got a lot of it wrong. I thought the Deli Counter Lab was fine though, I've done it in JavaScript before but it was interesting to write it in Ruby. My personality interview is on Friday for Flatiron School, fingers crossed!

## Day 36: October 11, 2017

**Today's Progress:** Watched an hour long video lesson on Object Oriented Programming. Finished Flatiron School's Bootcamp Prep completely! So now I have a BASIC grasp of Ruby and Javascript.

**Thoughts:** This video definitely broke down OOP a lot better than the labs and lessons. I THINK I understand it but I'm going to watch this video once again. I think Avi Flombaum does a great job at explaining Object Orientation which is harder for someone who's new to this to understand. I also like Ruby a lot more than JavaScript. Now I'm debating starting The Web Developer Bootcamp from the start OR fCC? Hmm...

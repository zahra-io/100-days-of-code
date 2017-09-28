# 100 Days Of Code - Log

## Goal:
1. Complete Flatiron School's Bootcamp Prep Course and #BacktoCode Challenge
  - JavaScript
  - Ruby Fundamentals
2. Complete Web Developer Bootcamp
3. Read JavaScript & jQuery by Jon Duckett
4.  @freeCodeCamp
5. Start a Programming/Computer Science blog and post once a week.

###### Started a clean slate for everything. I created a new Github account, a new account on Flatiron's Learn.co website, I'm starting over with my 100-days-of-code log because I felt that I needed to organize everything and create a new curriculum. I started Learn.co back in January when I FIRST started coding so the labs were already done and when I tried to re-do them, it got confusing. I have a better idea of what I'm doing and why I'm learning to code so here's to reaching goals!

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

```width x height = area
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

**Thoughts:** Feeling good! I took a peak at the final Rock Dodger lab and man oh man...I am not ready to tackle that beast. Do programmers ever feel like they don't know enough? I know THAT lab will take me days, maybe even a month to figure out. But I learned about the basic concepts of JavaScript which I'm feeling good about because now I'm aware of the existence of methods and structures that I'd have to use.

## Day 17: September 22, 2017

**Today's Progress:** Ruby - Introduction to Ruby

**Thoughts:**

## Day 18: September 23, 2017

**Today's Progress:** Ruby Fundamentals - Debugging, Variables

**Thoughts:**

## Day 19: September 24, 2017

**Today's Progress:** Ruby Methods Section

**Thoughts:**

## Day 20: September 25, 2017

**Today's Progress:** Ruby - Command Line Applications

**Thoughts:**

## Day 21: September 26, 2017

**Today's Progress:** Ruby - Command Line Applications

**Thoughts:**

## Day 22: September 27, 2017

**Today's Progress:** Ruby - Command Line Applications

**Thoughts:**

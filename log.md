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

# 100 Days Of Code - Log

## Goal:
1. Complete Flatiron School's Bootcamp Prep Course and #BacktoCode Challenge
  - JavaScript
  - Ruby Fundamentals
2. Complete Web Developer Bootcamp
3. Read JavaScript & jQuery by Jon Duckett
4. Start a coding blog/improve technical writing skills.
5. @freeCodeCamp

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

**Today's Progress:** Completed 6 newly added lessons on Bootcamp Prep that covered JavaScript basics such as Comments, Data Types, and Logging. This was a review. And then I worked on the Deli Counter Lab and read up on JavaScript & jQuery.

**Thoughts:** Man oh man, the Deli Counter lab. With code, you can feel like a warrior one day and be all "YASSS I GET THIS I'M SO GOOD" and then feel like a completely defeated loser the next because you realize you don't know A N Y T H I N G. That's how I felt with the Deli Counter Lab and it's in progress. I completed the first prompt, which honestly...I spent so much time on it and the solution was so simple and right in front of my face. I definitely have to spend some time understanding the solution though so tomorrow I'll do some research and continue onto the next few prompts.

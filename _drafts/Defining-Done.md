---
layout: post
comments: false
title: Defining Done As Boolean
---

Often in software development environments its been asked to developers whether they are done with their task or not. And its pretty obvious question for managers to ask to developers, nothing wrong or unexpected. Developers tend to answer this question as "yes, I am done" and if anything that can be wrong and unexpected here is what they mean by *done!*

{% include image.html img="images/defining-done.jpg" caption="Image Courtesy: http://www.quickmeme.com" %}

What developer mean by done can vary from developer to developer and we can not predict what actually done by him/her. Is *done* a boolean that clearly means either not at all done or actually finished everything? And again what is mean by 'actually finished everything'? As definition of *done* varies from person to person, there are always chances of understanding/assumptions gaps between developers' *done* and managers' *done* and business persons' *done* and its consequences can disturb the whole product delivery chain and can attract negative attention towards that developer.

So here I have listed some of the *done*'s in order from totally wrong to almost right:
## Just Works
Many times, rather most of the times developers say they are done once they have written a code that just works. So they write code for new feature, run it and see if its working. Is this right definition of *done*? Of course not. Why? Because code that just works is not approved by clean coders as final code. To know about how code that just works is not perfect solution, have a look at [my previous post](https://d4ttatraya.github.io/Dirty-Code).

## Works and Clean, Unit Tested
So, code that just works is not enough to say that we are done with feature. We should write that code matching standards of existing code and it should be clean; that is readable, testable, modifiable. Also we should add unit tests to make sure that code is working as intended in various test cases. Even if we did this, we are not done to say 'I am *done!*'

## Works and Clean, Unit Tested and Passes Automated Tests
Once we have code that works, code that is clean and code that is unit tested, we have to look for next criteria to get feature done. And that criteria is to pass all the already written automated tests. These automated tests can be integration tests and acceptance tests. Integration tests make sure that newly written code is integrated with existing system correctly and breaks nothing.

## Works and Clean, Unit Tested and Passes Automated Tests and QA Approved
Once we have finished all the above steps, still we are not done. What is remaining now? After finishing all the above steps, we should handover working system to QA and wait for his/her feedback, either bugs, modifications or approval. When QA approves our newly implemented feature, then and then only we can say that "I am *done!*", finally. So now we can say that our ***done* is boolean where not at all done or doesn't work or all above definitions falls under value-0 and only this definition falls under value-1**.  
As Uncle Bob says-  
*Done means done, no complete, no done-done.*

## Bonus
So many times its mentioned that we should always re-factor or clean the existing code, we can add this too in our definition of *done*. We should not say *done* until we re-factor(if required) existing code related to our newly written feature.

Every company has their own definition of *done*, but if any company doesn't then they should get it defined immediately and should ask their employees to follow it.  
If you have already defined your own *done* or have defined it now, then don't forget to put your definition in comments below!

*References:  
Uncle Bob's Clean Coder Book and [Talk About Professionalism](https://www.youtube.com/watch?v=BSaAMQVq01E)*


# Simple Copyleft License v1
An easy to understand license which protects the values of open source code without making the use of it too restrictive or permissive.

# Why?
Because lots of projects are by default selecting the GPL license instead of lesser restrictive and easier to understand licenses because they think that this is somehow good for the open source movement/community and/or their software.

## Why should I not use GPLv3 or GPLv2.1, etc?
You can if you agree with their values, but those licenses forces any users of your code to also use that license for their whole software [just because they did a few function calls to your code (if you didn't use LGPL)](https://www.gnu.org/licenses/gpl-faq.html#IfLibraryIsGPL).

For example if an indie developer wants to sell a game that they made which used a GPL licensed library for something minor like decoding a certain image format; then they also has to distribute the source code for the WHOLE game under the GPL license [(which allows anyone to freely redistribute the source code in public)](https://www.gnu.org/licenses/gpl-faq.html#DoesTheGPLRequireAvailabilityToPublic).

Hence such indie developers would have to avoid all GPL licensed libraries if they want to be able to make a fair living. Which in my view makes it bad to use such a restrictive license in most open source projects.

## My vision of the open source movement

To me the open source movement should be about collectivly helping the world become a better place by sharing source code and urging any improvement of that code to be shared back. Not to force everyone to open source their whole projects whenever they want to take advantage of open source implemantations of certain features (instead of waisting their time, money and energy reimplementing those features from scratch).

Society will progress much faster when people have better reasons to reuse existing code than reasons to reimplement it.

## The SCL license promotes good values

* It promotes the original authors to always be remembered and credited.
* It promotes sharing the source code of improved versions.
* It promotes using the code freely in any system whithout having to apply the license to the whole system.

# An example SCL license looks like this

`nameOfLibraryOrSoftware.license` file with content like this:
```
START OF LICENSE - Simple Copyleft License v1 (SCLv1)

You have the permission to use this code in any project as long as these terms are met:

1. A copy of this license-file has to be distributed together with the project in its root folder; Without any changes made to it other than the adding of authors (using UTF-8 encoding) after the line "Authors of edited versions" and after any other authors already named there.

2. If the code has been modified then the source code has to be easily acquirable free of charge by anyone who is interested in it.

3. You don't hold any of the authors responsible for anything.

Original project name:
Name Of Library Or Software

Original short description:
The description.

Original authors:
Whomever

Authors of edited versions:

END OF LICENSE
```
## Understanding the license

No one can take advantage of the SCL licensed code in a project without sharing the license file bound to that particular part of the code. The same license file which gives credits to the original project and authors.

And if they did modify parts of that code then they must also share this with whomever is interested. It must be easily acquirable and free of charge, for example by bundling this part of the source together with the binary release, distributing it via a public website or sharing it by request.

But any code that they are using to interface with the SCL licensed code (function calls to it etc) is however not bound by the license and does not need to be shared. So if they are using the code without having made modifications to it then they do not need to share it, just the license file.

This way a project can use lots of different SCL licensed libraries and not have to worry about sharing their proprietary source code which are using those libraries.

### Some advantages

* The license is written in an easy to understand language.
* It's short and easy to comprehend.
* It's direct and does not need a big paragraph to explain why authors are not liable or resposible for anything.
* Nothing in it can be misunderstood or angled in different ways.
* The license files all go in the root folder of a project using SCL licensed code, using the same .license extension but different filenames. This makes it very easy to see which parts of the code belogs to SCL licenced code and the needed credits are contained within these files.

# That's all for now

I'll come back and edit when I feel like it.
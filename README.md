# Simple Copyleft Licenses

Easy to understand [copyleft](https://en.wikipedia.org/wiki/Copyleft) licenses which protects the values of open source projects without making the use of them too restrictive or [permissive](https://en.wikipedia.org/wiki/Permissive_software_license).

This is the home of these two licenses:
* Simple Copyleft Code License v1 (SCCLv1)
* Simple Copyleft General License v1 (SCGLv1)

One is to be used for the code in a project and the other one for projects without code or to add a license bound to the other files in a project.

# Simple Copyleft Code License v1

## Why was it created?
Because lots of projects are by default selecting the GPL license instead of lesser restrictive and easier to understand licenses because they think that this is somehow good for the open source movement/community and/or their software.

### Why should I not use GPLv3 or GPLv2.1, etc?
You can if you agree with their values, but those licenses forces any users of your code to also use that license for their whole software [just because they did a few function calls to your code (if you didn't use LGPL)](https://www.gnu.org/licenses/gpl-faq.html#IfLibraryIsGPL).

For example if an indie developer wants to sell a game that they made which used a GPL licensed library for something minor like decoding a certain image format; then they also has to distribute the source code for the WHOLE game under the GPL license [(which allows anyone to freely redistribute the source code in public)](https://www.gnu.org/licenses/gpl-faq.html#DoesTheGPLRequireAvailabilityToPublic).

Hence such indie developers would have to avoid all GPL licensed libraries if they want to be able to make a fair living. Which in my view makes it bad to use such a restrictive license in most open source projects.

### My vision of the open source movement
To me the open source movement should be about collectivly helping the world become a better place by sharing source code and urging any improvement of that code to be shared back. Not to force everyone to open source their whole projects whenever they want to take advantage of open source implemantations of certain features (instead of waisting their time, money and energy reimplementing those features from scratch).

Society will progress much faster when people have better reasons to reuse existing code than reasons to reimplement it.

### The SCCLv1 license promotes good values
* It promotes the original authors to always be remembered and credited.
* It promotes sharing the source code of improved versions.
* It promotes using the code freely in any system without having to apply the license to the whole system.

## An example SCCLv1 license looks like this
`nameOfLibraryOrSoftware.codeLicense` file with content like this:
```
START OF LICENSE - Simple Copyleft Code License v1 (SCCLv1)

You have the permission to use, modify and redistribute this code in any project as long as these terms are met:

1. A copy of this license-file has to be distributed together with the project in its root directory; Without any changes made to it other than the adding of authors (using UTF-8 encoding) after the line "Authors of edited versions" and after any other authors already named there.

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
No one can take advantage of the SCCLv1 licensed code in a project without sharing the license file bound to that particular part of the code. The same license file which gives credits to the original project and authors.

And if they did modify parts of that code then they must also share this with whomever is interested. It must be easily acquirable and free of charge, for example by bundling this part of the source together with the binary release, distributing it via a public website or sharing it by request.

But any code that they are using to interface with the SCCLv1 licensed code (function calls to it etc) is however not bound by the license and does not need to be shared. So if they are using the code without having made modifications to it then they do not need to share it, just the license file.

This way a project can use lots of different SCCLv1 licensed libraries and not have to worry about sharing their proprietary source code which are using those libraries.

### Some advantages
* The license is written in an easy to understand language.
* It's short and easy to comprehend.
* It's direct and does not need a big paragraph to explain why authors are not liable or resposible for anything.
* Nothing in it can be misunderstood or angled in different ways.
* The license files all go in the root directory of a project using SCCLv1 licensed code, using the same .codeLicense extension but different filenames. This makes it very easy to see which parts of the code belogs to SCCLv1 licenced code and the needed credits are contained within these files.

## Using the license
Put the license file in the root of your project directory and give it a filename like this `ProjectName.codeLicense`.

Optionally put a header at top of the source code files bound by it to make it clear which license they're bound to. This can be useful if different parts of the code are using different license files. Example header:
```
/* See ProjectName.codeLicense for license */
```

### Example project directory structure:
```
My Project\
|  Source\
|  |  main.js
|  |  Thirdparty\Libraries\SomeLib\
|  |  |  SomeLib.js
|  |  |  SomeLib.codeLicense
|  MyProject.codeLicense
|  SomeLib.codeLicense (copied here to comply with SomeLib license)
```

## FAQ

### Is the license also bound to other files found in the project directory?
The license is only bound to the files containing the related source code and any compiled versions of that code. That's why the license is using the word "code" which can reference to code in both/any forms. Other files like images, sounds, etc is not bound by the license, which means that they default to being copyrighted unless stated othervise.

### What if I want the license to cover all the other files in my project directory?

SCCLv1 is designed to be a license for code only. If you want another similar copyleft license for your other files then I suggest that you use the SCGLv1 license described below.

# Simple Copyleft General License v1

## Why was it created?

Because the license described above will only be bound to the code in a project. Hence if not binding a copyleft license to the other files in a project [then they will by default be copyrighted](https://choosealicense.com/no-permission/).
So if you also want other people to be able to use the other files in your project then I reccomend using this license in addition to the SCCLv1 license. Or if the project doesn't contain any code then just this license.

## An example SCGLv1 license looks like this
`ProjectName.generalLicense` file with content like this:
```
START OF LICENSE - Simple Copyleft General License v1 (SCGLv1)

You have the permission to use, modify and redistribute these files (excluding any files bound by other licenses) in any project as long as these terms are met:

1. A copy of this license-file has to be distributed together with the project in its root directory; Without any changes made to it other than the adding of authors (using UTF-8 encoding) after the line "Authors of edited versions" and after any other authors already named there.

2. You don't hold any of the authors responsible for anything.

Original project name:
Simple Copyleft Licenses

Original short description:
Easy to understand copyleft licenses which protects the values of open source projects without making the use of them too restrictive or permissive.

Original authors:
Joakim L. Christiansen

Authors of edited versions:

END OF LICENSE
```

## Using the license
Put the license file in the root of your project directory and give it a filename like this `ProjectName.generalLicense`.


---
layout: essay
type: essay
title: Consistency is Key
# All dates must be YYYY-MM-DD format!
date: 2021-09-23
labels:
  - Software Engineering
  - IntelliJ
  - ESLint
  - Coding Standards
---

<img class="ui xsmall right floated rounded image" src="../images/jgrasp-wrong.png">

It comes to no surprise to anyone who has spent any significant time with me, I like margins, consistent justification, and contact names exclusively in lowercase letters. So, when it was not only required for this class to configure ESLint for ourselves but also that coding standards was a whole module, it was almost embarrassingly exciting.

## Out with the old, in with the new

I already have prior experience with the .xml extension as in ICS111 and ICS211 the professor required us to use Checkstyle for jGRASP. As these two classes were the foundation of my ICS education and coding, it stressed the importance of coding standards, not just because passing Checkstyle was on the rubric. One massive con about the Checkstyle for jGRASP, especially compared to ESLint with IntelliJ, was that a little button had to be pressed for Checkstyle to run on the current file. This meant that if one was to be rushed or not so careful, a quick click of the button could suddenly mean a lot more extra formatting work that they did not know existed before. A lovely feature of ESLint is that it is spontaneously triggered whilst writing code so wrong coding standards can be swiftly rectified and hopefully not repeated through every iteration of the same instance.

## No standard is bad standard

Although it is a mild annoyance to have to download .eslintrc and run `npm install` everytime, I would rather a few seconds go there than have code with drunk margins. At times I have come across, obviously not mine, code that felt closer to trolling than legitimate as the subversion of coding standards seemed too deliberate to be true. Not only does this make it massively difficult to read and understand the code, i.e. blocks of loops are not properly indented, it is frankly also visually unappealing. I believe a good programmer can not only fulfill objectives through their code but also make it easy for other people to understand their code. It is quite lonely at the top sometimes and sharing is caring when it comes to making code digestible and understandable.

## Work smarter not harder

If it has not been obvious, I am a massive fan of using ESLint. I have no qualms with having consistent code in terms of, including but definitely not limited to, spacings, indentations, var/let/const, curly braces locations, and actually will continue using some sort of coding standards checker on all of my IDEs in the future. Of course, people might say that my reasonings thus far on why I enjoy coding standards very superficial and surface level, but I would like to kindly offer up a rebuttal. Good coding standards oftentimes is a crash course into the format and mechanisms of a programming language that a beginner would probably easily forget. For example, ESLint suggests between var, let, and const depending on the situation and context; also ensures that all objects being declared are being used. There are absolutely no negatives to this. Except possibly to lazy programmers.

After all, consistency is the key to success. As Anthony Robbins said, "It's not what we do once in a while that shapes our lives. It's what we do consistently."

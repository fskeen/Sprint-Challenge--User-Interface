# Sprint Challenge: User Interface and Git - Multi-Page Website

This challenge allows you to practice the concepts and techniques learned over the past week and apply them in a concrete project. This Sprint explored User Interface and Git. During this Sprint, you studied Semantic HTML, CSS Fundamentals, CSS Flexbox Module, and Git. In your challenge this week, you will demonstrate proficiency by creating a multi page website that has some missing HTML elements as well as CSS specificity problems that need to be solved.  You will also create an additional web page that will be linked to from a navigation you will build.

## Instructions

**Read these instructions carefully. Understand exactly what is expected _before_ starting this Sprint Challenge.**

This is an individual assessment. All work must be your own. Your challenge score is a measure of your ability to work independently using the material covered through this sprint. You need to demonstrate proficiency in the concepts and objectives introduced and practiced in preceding days.

You are not allowed to collaborate during the Sprint Challenge. However, you are encouraged to follow the twenty-minute rule and seek support from your PM and Instructor in your cohort help channel on Slack. Your work reflects your proficiency in user interface and your command of the concepts and techniques in semantic HTML, CSS fundamentals, CSS flexbox module, and git.

You have three hours to complete this challenge. Plan your time accordingly.

## Commits

Commit your code regularly and meaningfully. This helps both you (in case you ever need to return to old code for any number of reasons and your project manager.

## Description

In this challenge, you build a missing header (navigation and image) on the home page, update some CSS styling on the home page, and create an additional page (About) which will link from the navigation you created.

In meeting the minimum viable product (MVP) specifications listed below, your web page should look like the solution screen shots of the home and about pages:

[Click here for the home page example](https://tk-assets.lambdaschool.com/39a49225-8ac9-43da-aa90-514fd60ae99a_sprint-challenge-ui-home-example.png)

[Click here for the about page example](https://tk-assets.lambdaschool.com/ede1bb1a-63ff-4801-8c02-3efa2f603190_sprint-challenge-ui-about-example.png)

## Self-Study Questions

Demonstrate your understanding of this week's concepts by answering the following free-form questions.

Edit this document to include your answers after each question. Make sure to leave a blank line above and below your answer so it is clear and easy to read by your project manager

### 1. If you were to describe semantic HTML to the next cohort of students, what would you say?

Semantic HTML is a way to write and structure your HTML content to provide context and meaning to that content. As an example, you can write and separate your HTML content entirely using ```<div>``` tags, like this:
 ```<div>
        <img src="header-banner.jpg">
    </div>
    <div>
      <div>
          <h2>Article #1</h2>
          <p> Proin sed quam sed tellus vestibulum ultrices quis in nunc. Phasellus id dui id tortor tincidunt efficitur. Proin faucibus imperdiet erat, non varius lacus. Maecenas non nisl id turpis egestas tincidunt. Nam condimentum venenatis magna eget finibus. </p>
      </div>
      <div>
          <h2>Article #2</h2>
          <p> Phasellus id dui id tortor tincidunt efficitur. Proin sed quam sed tellus vestibulum ultrices quis in nunc.</p>
      </div>
    </div>
```    
That will _work_, but there is a better way to help people maintaining your code (i.e. you and others), help improve accessibility, AND help improve SEO. Semantic HTML in practice means using tags that describe the actual content you are coding, like this:
Semantic HTML is a way to write and structure your HTML content to provide context and meaning to that content. As an example, you can write and separate your HTML content entirely using ```<div>``` tags, like this:

 ```<header>
        <img src="header-banner.jpg">
    </header>
    <main>
      <section>
          <h2>Article #1</h2>
          <p> Proin sed quam sed tellus vestibulum ultrices quis in nunc. Phasellus id dui id tortor tincidunt efficitur. Proin faucibus imperdiet erat, non varius lacus. Maecenas non nisl id turpis egestas tincidunt. Nam condimentum venenatis magna eget finibus. </p>
      </section>
      <section>
          <h2>Article #2</h2>
          <p> Phasellus id dui id tortor tincidunt efficitur. Proin sed quam sed tellus vestibulum ultrices quis in nunc.</p>
      </section>
    </main>
```
    
It's much clearer now what each part of the code is, right? If you need to update the image in the header, it's easy and quick to find that section of code. Structuring content this way also helps search engines and screen readers know what to prioritize -- which means more people can find your page and more people can enjoy it!

### 2. Name two big differences between ```display: block;``` and ```display: inline;```.
Both ways of laying out content, but they take different attributes and display content differently. By iteslf, `block` will display content that stacks but doesn't wrap, since it doesn't allow other elements to be next to it. You can adjust the width and height of the content that is displayed. `Inline`, on the other hand, _does_ allow wrapping. The dimensions of the "box" are the dimensions of the content, and `inline` does not take the width or height attributes, so you can't adjust them.

### 3. What are the 4 areas of the box model?

Margin - border - padding - content

### 4. While using flexbox, what axis does the following property work on: ```align-items: center```?

It works on the cross axis of whatever ```flex-direction``` is set to. By default (if you don't define anything), ```flex-direction``` is set to ```row```, which the x axis. This means by default, ```align-items: center``` would align the items on the y axis.

### 5. Explain why git is valuable to a team of developers.

Git is handy to use for dev teams for several reasons: Multiple people can collaborate on a project at once, and those contributions can be review, approved, edited, or denied on a case-by-case basis to preserve a working master branch. Git's version of source control involves branching and retaining a record of previous content states, so little information is ever permanently lost or altered. If you push flawed code to a branch, it can be reviewed before being pushed to the master branch. If it unintentionally gets pushed to master, it can be rolled back. GitHub works as a flexible tool to help organize projects and safeguard working code.

You are expected to be able to answer all these questions. Your responses contribute to your Sprint Challenge grade. Skipping this section *will* prevent you from passing this challenge.

## Project Set Up

- [x] Create a forked copy of this project.
- [x] Add your project manager as collaborator on Github.
- [x] Clone your OWN version of the repository (Not Lambda's by mistake!).
- [x] Create a new branch: git checkout -b `<firstName-lastName>`.
- [x] Implement the project on your newly created `<firstName-lastName>` branch, committing changes regularly.
- [x] Push commits: git push origin `<firstName-lastName>`.
 
Follow these steps for completing your project.

- [x] Submit a Pull-Request to merge <firstName-lastName> Branch into master (student's  Repo). **Please don't merge your own pull request**
- [x] Add your project manager as a reviewer on the pull-request
- [ ] Your project manager will count the project as complete by merging the branch back into master.
 


## Minimum Viable Product

Your finished project must include all of the following requirements:

### Home Page

[Review the provided design file for the home page](design-files/home.png).  Notice the navigation and header images are missing.

* [x] Build the HTML and CSS to create the missing navigation and header.
* [x] Link the `About` navigation item to the [about.html](about.html) page

You will also notice there are 10 boxes on the home page that need background colors.  Use this list below to correctly style each box:

* [x] box1: `teal`
* [x] box2: `gold`
* [x] box3: `cadetblue`
* [x] box4: `coral`
* [x] box5: `crimson`
* [x] box6: `forestgreen`
* [x] box7: `darkorchid`
* [x] box8: `hotpink`
* [x] box9: `indigo`
* [x] box10: `dodgerblue`

### About Page

[Review the provided design file for the about page](design-files/about.png). You have been provided the HTML wrapper, footer, and page content for the about page. Create the rest of the missing HTML and CSS to match the design file.

* [x] Copy and paste your home page navigation and header into the about page
* [x] Update the header image with the about page image
* [x] Link the `Home` navigation item back to the `index.html` page.
* [x] Build the rest of the about page layout to match the design

In your solution, it is essential that you follow best practices and produce clean and professional results. Schedule time to review, refine, and assess your work and perform basic professional polishing including spell-checking and grammar-checking on your work. It is better to submit a challenge that meets MVP than one that attempts too much and does not.

## Stretch Problems

After finishing your required elements, you can push your work further. These goals may or may not be things you have learned in this module but they build on the material you just studied. Time allowing, stretch your limits and see if you can deliver on the following optional goals:

* [ ] Build a page of your choosing from the navigation items.  Come up with content and images that fit the theme.  
* [x] Introduce CSS animations to your site. 
* [ ] Build a contact page and create a form with several inputs of your choosing
* [ ] Add responsive breakpoints to your code by using media queries

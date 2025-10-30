# Introduction

Git is a crucial skill to have, whether you’re just a hobbyist or you aim to become a professional web developer. It’s the “save” button on steroids and allows for seamless collaboration. There really aren’t all that many commands for you to learn, but sometimes the real difficulty of Git comes from visualizing what’s happening.

In this lesson, we’ll help with the visualization by diving deeper than just the `git add`, `git commit`, and `git push` commands you’ve mostly been using. We’ll cover topics such as **Remotes**, **Pointers**, and **Changing Git History**. This will expand your understanding of what’s actually going on under the hood with Git.

It is very important to take a look at all of this before progressing any further with the curriculum. The project work is becoming more and more complex, so using a disciplined Git workflow is no longer optional. Hopefully, after going through this lesson, you’ll be much more comfortable changing your Git history and have a better understanding of Git as a whole.

---

## Lesson Overview

This section contains a general overview of topics that you will learn in this lesson.

- History-changing Git commands  
- Different ways of changing history  
- Using remotes to change history  
- Dangers of history-changing operations  
- Best practices of history-changing operations  
- Pointers  

---

## Changing History

So let’s say you’re comfortable writing good commit messages and you’re working with branches to have a good Git workflow going. But nobody is perfect, and as you’re writing some beautiful code something goes wrong! Maybe you commit too early and are missing a file. Maybe you mess up one of your commit messages and omit a vital detail.

Let’s look at some ways we can change recent and distant history to fit our needs. We’re going to cover how to:

- Change our most recent commit  
- Change multiple commit messages  
- Reorder commits  
- Squash commits together  
- Split up commits  

---

## Getting Set Up

Before we get started with the lesson, let’s create a Git playground in which we can safely follow along with the code and perform history-changing operations.

```bash
touch test{1..4}.md
git add test1.md && git commit -m 'Create first file'
git add test2.md && git commit -m 'Create send file'
git add test3.md && git commit -m 'Create third file and create fourth file'

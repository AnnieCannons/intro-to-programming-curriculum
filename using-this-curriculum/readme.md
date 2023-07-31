# Working With AnnieCannons' Curriculum Repositories

A guide for instructors.

## The Problem

There are two kinds of work that can be done on a course's curriculum as it progresses:

1. Material that's specific to a cohort. Maybe it's extra resources for something the students get interested in, like TypeScript or Bash scripts or the blockchain; maybe it's a calendar for what their class will be like if they take Intro to Programming and three Advanced Module courses; maybe ti's a readme with each student's GitHub usernames.
2. Material that _everyone_ could use. A game a particular instructor likes for learning Flexbox, or an extra exercise we came up with to help drill on arrays, or further documentation of our process.

For material that both current and future students could use, we want to ensure that this valuable new material doesn't get lost to time and instructor turnover. So it _has_ to make it into the current students' curriculum, but _also_, vitally, must get into the general curriculum. Otherwise you get a lot of instructor time and effort that only benefits their current cohort and is never used again.

For cohort-specific material, on the other hand, a curriculum can get out of hand in an awful hurry if each cohort's instructors are inserting one-off material into our general material. Try having every single cohort's GitHub usernames, or 11 different articles on the best VS Code extensions. And as we all know, it never feels to anyone of any position that they have the go-ahead to madly delete files that they're only _pretty_ sure we don't need.

## The Solution

The solution is to have two repos: an upstream repo with the agreed-upon and ever-evolving curriculum, and a cohort-specific repo for their students alone.. Changes that will help the curriculum long-term can be pushed back upstream as well to the curriculum repo, while cohort-specific changes can stay with the cohort repo.

## Okay, Then. How?

Let's talk about how to implement this solution.

### First, The General Workflow

We'll discuss setting it all up momentarily, but it'll be helpful to see how the workflow will go first.

#### Adding Cohort-Specific Changes

If you're making a change that is just for the cohort:

1. You'll switch to the `cohort-specific-changes` branch with `git switch cohort-specific-changes`.
2. Run `git pull upstream main` to update it with any new curriculum you don't yet have.
3. Make the changes you want, then `add`, `commit`, and `git push origin cohort-specific-changes` them.
4. Switch back to `main` with `git switch main`.
5. Merge in the changes from the other branch with `git merge cohort-specific-changes`.
6. This still hasn't impacted the `main` branch, but a `git push origin main` will get those changes into the part of GitHub our students are used to checking.

#### Adding Curriculum Material

When we make changes that should go in our general curriculum, the situation is _exactly_ the same for a while, except with the branch names changed. And then some extra steps at the end to get those changes back to the curriculum.

1. Switch to the `curriculum-changes` branch with `git switch curriculum-changes`.
2. Update it with any new curriculum you don't yet have with `git pull upstream main`.
2. Make the changes you want, then `add`, `commit`, and `git push origin curriculum-changes` them.
3. Switch back to `main` with `git switch main`.
4. Merge in the changes from the other branch with `git merge curriculum-changes`.
5. This still hasn't impacted the `main` branch, but a `git push origin main` will get those changes into the part of GitHub our students are used to checking.

_And now, the big difference_: for generalized curriculum, an extra step to get those changes back into the main curriculum repo.

1. Navigate to your cohort-specific repo on GitHub and switch the view to that of the `curriculum-changes` branch.
2. Open a PR from the `curriculum-changes` branch of the cohort-specific repo to the `main` branch of the curriculum repo.
3. Ask another instructor to review your PR and merge it.
4. Celebrate that you just helped shape our long-term curriculum!

This seems _fairly_ straightforward... How hard is it to set up?

### Setting Up

It's not all that complicated, and you only need to do it once!

Ish!

#### Setting Up For A New Cohort (we only need to do this once per cohort)

In order to set this up for a new cohort, you need to do the following:

1. Find the curriculum repo for the class your cohort is taking.
2. Fork it. The owner should remain the AnnieCannons organization, and you can name the new repo something specific to your cohort, like "C11-Intro-To-Programming".
3. Create new branches on GitHub called `curriculum-changes` and `cohort-specific-changes`.

And you've done it: you've found your curriculum repo and made your own cohort-specific repo.

#### Setting Up For A New Instructor To Work Locally (we need to do this once per instructor's computer)

In order to work with the curriculum on your computer, here's what you'll need to do.

1. Clone your _cohort-specific_ repo with `git clone` and navigate into the directory with `cd`.
2. Although the remote has `curriculum-changes`, your local version only has `main`. Run `git switch -t origin/curriculum-changes` to add it as a local branch and set it to track the remote.
3. Run step 2 with the branch name changed to `cohort-specific-changes` to get that local branch.
4. Lastly, add the original curriculum repo as a remote so you can pull curriculum changes that come in. Run `git remote add upstream [the url of the curriculum repo]` except that of course the part of the command where the square brackets are, and their contents as well, should be replaced by (you guessed it) the url of the curriculum repo.

## Conclusion

This will all take a little more work, a bit of getting used to, and a fair bit of discipline to make sure the system works as intended, but the advantages are substantial. Besides the advantage of a well-maintained curriculum—so vital to success as a school—we'll also allow our instructors to get plenty of Git practice, as this author has as well. Those instructors with less Git experience will get to flex their branch-and-PR muscles, some perhaps for the first time, while those instructors with more practical developer experience will get to mentor those with less, helping (as we know) mentor and mentee alike.

And that's how you _do_.

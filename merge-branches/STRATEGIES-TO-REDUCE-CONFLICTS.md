- [Strategies to reduce conflicts](#strategies-to-reduce-conflicts)
  - [Keep lines short](#keep-lines-short)
  - [Keep commits small and focused](#keep-commits-small-and-focused)
  - [Beware stray edits to whitespace (spaces, tabs, line returns)](#beware-stray-edits-to-whitespace-spaces-tabs-line-returns)
  - [Merge often](#merge-often)
  - [Track changes to `main`](#track-changes-to-main)

# Strategies to reduce conflicts

## Keep lines short

If lines are short:
- there are **less characters** in them
- it's **less likely** that something is going to conflict
- it's **easier to identify and fix** conflicts when they arise

## Keep commits small and focused

Don't make commits that are **enormous in scope**, especially if they contain files which are **not related to changes**. Instead, make a commit that does **one single thing**.

## Beware stray edits to whitespace (spaces, tabs, line returns)

Just **stick** with either spaces or tabs and don't make line returns **unnecessarily**.

## Merge often

Merge from your `feature` branch back into your `main` branch **as much as you can**.

Some developers use **feature flags**, so that the feature is present in the main code, but it's not turned on unless a certain flag is triggered. It's a technique that allows us to keep merging back in those `feature` branches into `main` regularly to reduce merge conflicts without actually activating the feature for the public.

## Track changes to `main`

It's a bit like merging often but **in reverse**.

Merging `main` branch periodically into your `feature` branches is a process called **tracking**.
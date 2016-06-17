---
layout: post
title:  "Meteor testing"
date:   2016-06-17 13:00:31 +0200
categories: meteor testing
---

I have spent some time trying to get the new testing framework in Meteor up an running.
Here are some issues I encountered, and how I fixed them.


#### Test cases are loaded but do not run

If you log the `describe` blocks, you get output, but the `it` cases are never run and don't show up in the test runner.
Try removing the --port argument if you use that, or add it if you don't. For some reason this triggers a re-discovering of your tests.
No idea why this happens, further investigation to follow.


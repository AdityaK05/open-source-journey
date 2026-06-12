# Day 5

## Repository

SigNoz

## Repository Link

https://github.com/SigNoz/signoz

## Issue Worked On

#7170 — Tables overlap, enable slider for left panel and also for tables

## Pull Request

https://github.com/SigNoz/signoz/pull/11702

## Problem Statement

The NewWidget panel editor allowed table content to overflow, causing the table preview to overlap the right settings panel instead of scrolling properly.

This resulted in a poor user experience when working with large table datasets.

## Changes Made

### Files Modified

* frontend/src/container/NewWidget/index.tsx
* frontend/src/container/NewWidget/NewWidget.styles.scss
* frontend/src/container/NewWidget/styles.ts

### Improvements

* Added scroll support for the right settings panel.
* Added proper height constraints to both left and right panels.
* Prevented content overflow between resizable panels.
* Ensured tables scroll correctly instead of overlapping adjacent content.
* Preserved existing resize functionality.

## Technical Concepts Learned

### React & Frontend

* Layout debugging
* Scroll container management
* Resizable panel architecture
* Component composition
* UI bug fixing

### CSS

* Flexbox layouts
* Overflow handling
* Height constraints
* Scroll behavior
* Responsive container design

### Open Source

* Reading issue discussions
* Understanding existing architecture
* Fixing real user-facing bugs
* Creating production-quality PRs
* Writing meaningful PR descriptions

## Challenges Faced

* Understanding the NewWidget component structure.
* Identifying the root cause of panel overflow.
* Ensuring scrollbars worked without breaking resize behavior.
* Maintaining consistency with existing OverlayScrollbar usage.

## Outcome

Successfully implemented a UI fix that prevents table content from overlapping adjacent panels and improves usability for large datasets.

## Pull Request Status

* PR Opened
* Awaiting Review
* CI Checks Pending/Passed

## Key Takeaway

Many frontend bugs are not caused by React logic but by layout constraints, container sizing, and overflow behavior. Learning to debug these issues is essential for production frontend engineering.

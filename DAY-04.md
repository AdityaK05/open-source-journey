# Day 4

## Repository

SigNoz

## Repository Link

https://github.com/SigNoz/signoz

## Issue Worked On

#7011 — Handle invalid invitation token gracefully in signup page

## Pull Request

https://github.com/SigNoz/signoz/pull/11647

## Problem Statement

When users visited the signup page with a missing, invalid, or expired invitation token, the application showed unclear errors or exposed raw API error messages. This created a poor onboarding experience for first-time users.

## Changes Made

### File Modified

frontend/src/pages/SignUp/SignUp.tsx

### Improvements

* Added URL token extraction using the existing `useUrlQuery` hook.
* Added validation for missing invitation tokens.
* Added user-friendly error messages for:

  * Missing token
  * Invalid token
  * Expired token
* Improved API error handling.
* Disabled signup submission when no valid token is present.
* Followed existing application patterns using:

  * AuthError component
  * APIError class
  * Existing error state management

## Technical Concepts Learned

### React

* useEffect
* useState
* Form validation
* Error state management

### TypeScript

* Error type narrowing
* API response handling
* Optional properties

### Open Source

* Reading issue discussions
* Understanding existing code patterns
* Following repository conventions
* Creating production-ready pull requests
* Working with maintainers and reviewers

## Challenges Faced

* Understanding SigNoz authentication flow.
* Finding where invitation tokens were processed.
* Matching existing Login page behavior.
* Ensuring valid signup flows were not affected.

## Outcome

Successfully implemented a frontend UX improvement that provides clear guidance to users when invitation tokens are missing, invalid, or expired.

## Pull Request Status

* PR Opened
* Reviewers Assigned
* Awaiting Maintainer Review

## Key Takeaway

Open-source contributions are not just about writing code. A good contribution requires understanding the existing architecture, following project conventions, and minimizing regressions while solving a real user problem.

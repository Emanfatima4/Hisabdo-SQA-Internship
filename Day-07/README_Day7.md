# SQA Internship – Day 7

## Mini QA Test Project – Daraz Pakistan

**Intern:** Eman Fatima  
**Internship:** HisabDo SQA Internship Program  
**Testing Type:** Manual Web Testing + API Testing  
**Application:** Daraz Pakistan Web Application

\---

## 1\. Project Overview

This project represents a complete QA testing cycle performed from a Software Quality Assurance Engineer's perspective.

The publicly available Daraz Pakistan web application was selected as the system under test. Testing covered functional behavior, UI, form validation, positive and negative scenarios, boundary conditions, basic usability, cross-browser compatibility, and API testing.

The overall QA process followed:

> \*\*Plan → Test → Record → Report → Summarize\*\*

\---

## 2\. Testing Objectives

* Verify major website functionality.
* Validate UI elements and product/category presentation.
* Test form validations.
* Perform positive and negative testing.
* Check boundary and edge-case behavior.
* Evaluate basic usability.
* Perform cross-browser testing.
* Test APIs using Postman.
* Add automated Postman assertions.
* Document actual defects with evidence.
* Prepare a complete test execution summary.

\---

## 3\. Testing Areas Covered

### Functional Testing

Major user flows including homepage navigation, search, categories, product listings, product details, login and cart-related behavior were tested.

### UI Testing

Visibility, layout, product cards, images, prices, navigation elements and overall presentation were checked.

### Form Validation

Login and input validation scenarios were tested, including empty and invalid inputs.

### Positive Testing

Valid searches, navigation, categories, products and successful user actions were tested.

### Negative Testing

Invalid, empty, special-character and non-existing input scenarios were tested.

### Boundary Testing

Boundary scenarios included long search input, leading/trailing spaces and minimum-length input.

### Basic Usability Testing

Navigation clarity, back navigation, page consistency and user feedback were observed.

### Cross-Browser Testing

The application was tested in Google Chrome and Microsoft Edge. Major homepage and product-listing behavior was consistent across both browsers.

### API Testing

API testing was performed using Postman with automated assertions and CRUD operations.

\---

# 4\. Test Execution Summary

|Metric|Result|
|-|-:|
|Total Test Cases|58|
|Test Cases Executed|58|
|Passed|54|
|Failed|4|
|Blocked|0|
|Not Executed|0|
|Web Test Pass Rate|93.10%|
|Bugs Found|4|
|Critical Bugs|0|
|High Bugs|0|
|Medium Bugs|4|
|Low Bugs|0|

> Note: All 58 test cases were executed during the Day 7 testing cycle.

\---

# 5\. API Testing Summary

API testing was performed using the public JSONPlaceholder testing API.

|Test Case|Method|Endpoint|Expected Status|Result|
|-|-|-|-|-|
|Get All Posts|GET|`/posts`|200|PASS|
|Get Single Post|GET|`/posts/1`|200|PASS|
|Create Post|POST|`/posts`|201|PASS|
|Update Post|PUT|`/posts/1`|200|PASS|
|Delete Post|DELETE|`/posts/1`|200/204|PASS|

### Automated Assertions

Postman automated assertions were added for:

* Status code validation
* JSON response validation
* Array/object validation
* Required field validation
* Post ID validation
* Created post title validation
* Updated post title validation
* Successful DELETE response validation

### API Execution Result

**5/5 API requests passed successfully.**

The `GET /posts` request returned **200 OK** with all automated assertions passing. The final observed response time was approximately **650 ms**.

\---

# 6\. Bugs Identified

### BUG-001 – Special Character Search

**Module:** Search  
**Severity:** Medium  
**Priority:** Medium

Special-character input such as `@#$%` returned apparently unrelated products instead of handling the input with a clear no-result/relevance response.

### BUG-002 – Long Search Input Layout Overflow

**Module:** Search  
**Severity:** Medium  
**Priority:** Medium

A very long search query caused visible text overflow and disturbed the intended results layout.

### BUG-003 – Incorrect Product Relevance in Pizza Maker Category

**Module:** Categories → Pizza Maker  
**Severity:** Medium  
**Priority:** High

The Pizza Maker category displayed mainly pasta/noodle maker products, indicating a category-to-product relevance issue.

### BUG-004 – Missing Empty Login Validation Feedback

**Module:** Login / Form Validation  
**Severity:** Medium  
**Priority:** Medium

Submitting the login form with required fields empty did not display a clear validation message to the user.

\---

# 7\. Evidence

Screenshots and evidence collected during testing are stored in the `Screenshots` folder.

Evidence includes search results, special-character search behavior, long search input behavior, category/product mismatch, and other functional observations.

The `Evidence\_Log` file maps available screenshots to related test cases and bugs.

\---

# 8\. Tools Used

* Google Chrome
* Microsoft Edge
* Postman
* GitHub
* Microsoft Excel
* Microsoft Word

\---

# 9\. Test Conclusion

The Day 7 mini QA project successfully covered the required web testing areas and API testing fundamentals.

A total of **58 web test cases were executed**, with **54 passed and 4 failed**, resulting in a **93.10% execution pass rate**. Four medium-severity defects were identified and documented.

API testing covered the main CRUD operations using Postman, with automated assertions successfully validating the responses.

Overall, the project demonstrates the complete QA cycle:

> \*\*Plan → Test → Record → Report → Summarize\*\*




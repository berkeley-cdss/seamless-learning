# Seamless Learning Accessibility Workshop
{:.no_toc}

* **Dates**: Monday 8/19/2024 - Tuesday 8/20/2024
* **Times**: 10:10am - 5:30pm
* **Location**: Soda 380, online by request
* **Organizers**: Professors Michael Ball and Lisa Yan, EECS and Data Science

**Attendance**: This workshop is open to all UC Berkeley EECS/Data Science/Statistics ASEs, even if you did not register. If you did not register ahead of time but are interested in attending, please send Michael and Lisa an email or Slack message so that (at minimum) we can plan for extra food.

**Workshop Goals**: 
* Know what assistive technologies are.
* Understand WCAG and accessibility guidelines and compliance processes on campus.
* Successfully make compliant formats of an entire course website OR a chunk of course materials, e.g., 4 weeks of the semester.
* Determine processes creating accessibility-compliant web material for other aspects of your course for the current semester and going forward.
* Contribute to the set of go-to solutions that can be applied to similar classes in EECS, Data Science, and Statistics.

Jump to:
* TOC
{:toc}

## Prework
* Log in to SiteImprove.
* Skim Project Scope Ideas below to get a sense of what you want to do in your team.
* Get access to the necessary set of course materials.
* If your materials involve GitHub: clone your repo, check your permissions and tokens, and know how to push and pull. We suggest having a document of go-to Terminal commands.
* Notify organizers (Michael and Lisa) ahead of time if:
  * (ASAP) You have dietary restrictions.
  * You need to be hybrid on a particular day, or you need to be online, and you didn't mention it on the Google Form.
  * You need to miss a day.

## Workshop Agenda

**Monday 8/19/2024**

| Start Time | Activity |
| ---- | ---- |
| 10:10am  | \[ Talk \] Welcome and Workshop Overview<br/>_Michael Ball and Lisa Yan_ |
| 10:20am  | \[ Talk \] Accessibility and Demos<br/>_Michael Ball_ |
| 10:45am  | \[ Talk \] Web Accessibility Resources on Campus<br/>_Jane Lee, Accessibility Lead, College of Engineering_ |
| 11:30am  | Team-forming and project discussion |
| 12:00pm  | \[ Break \] Lunch |
| 1:00pm  | \[ Talk \] WCAG details and Dev Tools<br/>_Michael Ball_ |
| 1:45pm  | Project work time |
| 3:00pm  | \[ Break \] Coffee and Snacks |
| 3:30pm | Project work time |
| ~5:00pm | **End of Day 1** |
| 5:30pm | Optional Hike |

**Tuesday 8/20/2024**

| Start Time | Activity |
| ---- | ---- |
| 10:10am  | \[ Discussion \] Takeaways from Day 1 |
| 11:00am  | \[ Talk \] Colors and Presentations<br/>_Brandilyn Buckley, Data Science Undergraduate Studies_ |
| 12:00pm  | \[ Break \] Lunch |
| 12:30pm | \[ Talk \] Accessibility on JupyterHub<br/>_Balaji Alwar, DataHub Service Lead, RTL_ |
| 1:00pm  | Project work time |
| 3:00pm  | \[ Break \] Coffee and Snacks |
| 3:30pm | Project work time |
| 4:30pm | \[ Discussion \] Lightning Takeaways |
| 5:15pm | \[ Talk \] Wrap up and Best Practices for the Semester<br/>_Michael Ball and Lisa Yan_ |
| 5:30pm | **End of Day 2** |

## Project

### Overall Workshop Activities

Day 1:
* _Team forming_: Group together by project, not by course.
* By the end of Day 1, know how to run browser/accessibility checkers and begin making manual changes on a few course resources in your project.
* By the end of Day 1, start thinking about what would be a good process to continue this work in Fall 2024.

Day 2:
* _Takeways from Day 1_: At the start of Day 2, share one quick takeaway from Day 1 and one question.
* By the end of Day 2, have a process in place to continue your work in Fall 2024. Such a process should:
  * _Be well-documented._ What should other course staff members know about how to read reports, how to make edits, whom to reach out to?
  * _Be relatively low workload._ As best as possible, try to create processes that concentrate any needed edits to source files, as opposed to raw HTML.
  * _Be realistic and needs-based._ Focus on Fall 2024 first. Then, if time, focus on edits to previous semesters. Note that we don't have all the details about how course materials (beyond websites) will be assessed for compliance, but we can be proactive by including accessibility edits as part of best practices.
* _Lightning Takeaways_: At the end of Day 2, share what you've done (big or small!) and next steps.

Specific suggestions for task breakdown per project are listed below.

### Project Scope Ideas
The below projects are scoped to what we think is realistic for a 1-2 student team to complete in a two-day workshop.

If you have more than 2 people in your course, we suggest that on Day 1 you pair up somehow and *all* get familiar with how to make manual changes on multiple projects. Then, on Day 2, you can split up to determine good processes for continuing your work.

1. berkeley-class-site GitHub pages course websites
  * Convert your course website to use [berkeley-class-site](https://github.com/berkeley-cdss), a WCAG-compliant course website template
  * Add site index maps to your homepage
  * Tweak fixes based on accessibility reports
  * Add back in custom course website components that still comply with accessibility
  * Project breakdown:
    * Day 1: Run the browser checker on a few of your course webpages, make small manual fixes
    * Day 1: Start importing berkeley-class-site template into your course website repo.
    * Day 2: Finish the importing process to berkeley-class-site and make all fixes.
    * Day 2: Backport to previous semesters, or move to another project
  * _Courses_: Data Science course websites, classes on GitHub Pages with few commitments to a custom layout
  * **Prework**: Get fork or write access to your current course's GitHub Pages repo.

1. Custom course websites
  * Include GitHub actions that check for accessibility compliance
  * Implement fixes based on accessibility reports
  * Add site index maps to your homepage
  * _Courses_: Classes with very specific custom layouts for which converting to berkeley-class-site would require a lot of process or logistics changes (in addition to technical changes)
  * **Prework**: Get fork or write access to your current course's website repo.

2. Jupyter Notebooks
  * Make your JupyterHub notebooks compliant with DataHub a11y checker
  * _Courses_: Courses with lots of demo notebooks, Data textbooks, etc.
  * **Prework**: Get fork or write access to course materials notebooks (lecture notebooks, or assignment Otter source notebooks).

3. LaTeX PDFs
  * Find a comfortable workflow for writing LaTeX source files that can build to PDF *and* accessible HTML. It's okay if the latter is manual, as long as it can be generated without too much effort.
  * _Courses_: Courses with lots of course note PDFs or discussion PDFs
  * **Pre-work**: Get edit access to Overleaf or a copy of LaTeX source files.

4. Answer/solution PDF handouts
  * Find a comfortable workflow for writing discussion handouts and solutions directly as HTML.
  * Suggestion: Open-ended and long term project, so we don't recommend it for this workshop. But if you're curious and want to implement this in berkeley-class-site, reach out to us so we can explore a semester-long engineering project.

5. Discussion and/or slides
  * Implement an accessible theme for your class.
  * Install accessibility checkers in PowerPoint or Google Slides.
  * Implement fixes based on accessibility reports.
  * If your course uses lecture slides, suggest fixes to faculty instructors, or identify a process by which ASEs can make fixes supervised by faculty instructors. But you should prioritize discussion materials.
  * Suggestion: This is lower priority than getting website material accessible and compliant, so we don't recommend spending all your time on it for this workshop. But know what processes are in place so you can incorporate this into your content updates during the Fall semester.
  * **Pre-work**: Get edit access to discussion slides.

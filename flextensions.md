# Flextensions

Flextensions is a tool for automating assigment extensions---from student request to instructor approval. Flextensions currently works with Google Forms and Gradescope. Canvas/bCourses support is in active development.

**AY24-25 Student leads**: Edwin Vargas Navarro, Conan Smallwood

## Recent Updates

* [Spring 2025]
  * CS 169L project: Flextensions web interface
  * Teresa Luo and Kevin Sheng will present a poster on Student Support Systems at SIGCSE 2025!
* [Fall 2024]
  * Flextensions tool now in use across all Data Science courses!
  * Two Data Science Honors Thesis on Flextensions in progress: Teresa Luo (Student Support Systems in CS61B) and Conan Smallwood (Data Engineering in Google Cloud)
  * Made huge updates to documentation! Hopefully now more useful.
  * Jordan Schwartz and Charisse Liu presented Flextensions at FIE 2024!
* [Spring 2024]
  * Jordan Schwartz and Yuerou Tang presented Flextensions at SIGCSE 2024!
  * Dana Benedicto finished up her Data Science Honors Thesis on early usage of Flextensions in Data Science courses!

## Project Overview

[minor edits to original Teach-Net post, January 2024]

The education literature tells us that flexible (soft) deadlines reduce student stress, keep students accountable for their own learning (and meta-learning), and ensure that the course grade represents the work that students have submitted rather than being distorted by late penalties (Feldman, 2018). At Berkeley, students are requesting more accommodations than prior to the pandemic for many reasons (DSP accommodations, ASE strike, pandemic, personally affected by global crises, etc.)

With the **Flextensions** system we’ve been developing, students submit a Google Form detailing their extension request—which assignment, how many days requested, and why. If the requested extension is less than an instructor-specified threshold (e.g., 2 days), Flextensions notifies the student by email that it’s been approved. For assignments submitted via Gradescope, the tool automatically updates Gradescope to accept that student’s assignment late. (We’re working on similar automation for bCourses.) If the request is for longer than that threshold, the course staff are notified and can ask the student to either exchange email with or meet with a member of course staff (instructor-settable) before the extension is requested, just to make sure there are no systemic or student-distress issues that may need attention in order to keep the student on track for success. (Anecdotally, a number of students have reported being pleasantly surprised and relieved when their professor meeting wasn’t to chew them out for being late, but to actually check on their well-being.)

In other words, Flextensions helps centralize the majority of administrative work required to track extensions for individual students.

Since the prototype was launched by Computer Science TAs half a decade ago—lecturer Peyrin Kao was a huge student contributor before he joined the faculty—Flextensions has been adopted by many large CDSS and EECS courses including Data 8, C88C, 100, the CS 61 series, CS 161, and CS 169. These courses have redesigned course policies to minimize abuse of the soft deadlines system—of which there’s minimal, particularly at the upper-division level. Ultimately, it’s been a huge benefit to us in our giant STEM courses: ~90% of requests are quick and one-time, and (u)GSIs can immediately identify students who need instructor meetings or more support. We’ve been studying various components of the project, including how it could close learning equity gaps, promote student self-efficacy, and reduce staff logistical burden. We will be working on supporting bCourses assignments in the future.

 So far, we’ve only tried the Flextensions paradigm in CS/Data courses, where assignments are majority autograded. Extensions with non-autograded assignments are currently constrained by staff grading capacity. We’d love to hear if you have ideas for how this could work in natural sciences, social sciences, or humanities courses for a subset of assignments, say, those submitted via online bCourses portals.

## Overview of the Student Experience
Students submit a short Google form to request an extension on a particular assignment, indicating how long they want and a brief reason for the request. Most forms are automatically processed with no staff intervention: for example, DSP-related requests, or extensions shorter than an instructor-specified threshold. In these cases, Flextensions notifies the student by email that the extension was approved, and if Gradescope is being used to accept submissions, Flextensions updates Gradescope to allow a later submission time for the student on that assignment. (We are working on similar automation for bCourses and other online submission systems.) In other cases, Flextensions notifies the student that their extension will be manually approved after they either email more details or meet directly with a TA or instructor -- this ensures a “contact point” so the staff can make sure the student isn’t experiencing more systemic problems. If your course staff uses Slack for communication, Flextensions can also send a Slack message to a designated channel to notify course staff when new requests arrive.

For more information, check out our
[slides](https://docs.google.com/presentation/d/1Fwtr7vfWDEM8JkAQdmATEO67BV2yVOLEjxlWvohEi8c/edit?usp=drive_link)
from the 2024 Teaching and Learning Conference at UC Berkeley, presented by Jordan Schwartz. Please also see our publications below.

## Access GitHub
* [Flextensions GitHub](https://github.com/berkeley-cdss/extensions) Actively maintained by Seamless Learning Team.
* There is also a CS161 extensions GitHub, which we are slowly phasing out. 

## Tool Support
At present, Flextensions is supported by generous time from instructors and course staff using this tool in their classes. We are looking for a way to support this tool more widely for any course instructors, regardless of software fluency.

## History and Faculty involvement

The public Flextensions tool was developed in Spring 2022 CS161: Computer Security, taught by Nick Weaver. Several TAs including Shomil Jain, Peyrin Kao, Vron Vance, and Zephyr Barkan wrote and contributed to the first iteration of this tool, along with an accommodations policy that encouraged student usage. Fuzail Shakir wrote the first Flextensions experience report in his May 2023 MS EECS Technical Report, advised by Armando Fox.

Starting Summer 2023, Flextensions software and maintenance has been integrated into software development and maintenance projects sponsored by the Seamless Learning Team, run by Michael Ball and Lisa Yan.
In Fall 2023, Narges Norouzi was integral in kicking off research projects studying the impact of Flextensions on student learning. Also in Fall 2023, this tool became widely used by almost all Data Science Undergraduate Studies (DSUS) courses; Silas Santini, DSUS Software Engineer, has supported software tool onboarding for different DSUS courses.

## Research and Development

There are two main academic thrusts for Flextensions:
* **Software Engineering**. How do we build Flextensions, a software tool for assignment extensions, that works across a wide array of courses? How do we make it open-source and encourage collaboration and open discussion among teaching assitants and instructors? How do we design a sustainable support system for this tool?
* **Impact on Teaching and Learning**. How do flexible assignment extensions impact student ability to achieve learning outcomes? How do different course policies impact student ability to complete work? How does a tool like Flextensions support teachers by reducing adminitrative workload to creating more flexible, adaptable classrooms? What are reasonable course policies that appropriately balance student accessibility with student accountability?

Since 2023, this project has spawned numerous opportunities for undergraduate and Master's student research.

### Proceedings and Presentations

* [proceedings, poster, to appear]	Teresa Luo, Chenkun Sheng, and Lisa Yan. "Supporting Students at Scale: Profiling Student Behaviors on Usage and Impact of the Student Support System." Proceedings of the 56th ACM Technical Symposium on Computer Science Education (SIGCSE), Pittsburgh, PA, February 2025. [doi](https://doi.org/10.1145/3641555.3705258)
* [proceedings, WIP] Dana Benedicto, Jordan Schwartz, Narges Norouzi, and Lisa Yan. "WIP: Automated Flexible Extensions for Improving Learning Equity in Large Scale Computing Classrooms." In IEEE Frontiers in Education Conference (FIE), October 2024. 
[slides](https://docs.google.com/presentation/d/1C8QcfhtUjb6yT6mlrxLdmraYfd2QH-gs/edit?usp=drive_link&ouid=113745915748997113650&rtpof=true&sd=true)
* [proceedings, WIP] Charisse Liu, Yuerou Tang, Narges Norouzi, and Lisa Yan. "WIP: Examining the Impact of a Flexible Extension Policy on Student Learning Experience in a Large-Scale Computing Course." In IEEE Frontiers in Education Conference (FIE), October 2024. [slides](https://docs.google.com/presentation/d/1jIHNSKI26pUBrVgWzgQCIjOz1clWIzKf/edit?usp=drive_link&ouid=113745915748997113650&rtpof=true&sd=true)
* [public talk] Jordan Schwartz and Yuerou Tang. "Automated Support for Flexible Extensions." Teaching and Learning Conference, UC Berkeley. May 2024. [slides](https://docs.google.com/presentation/d/1Fwtr7vfWDEM8JkAQdmATEO67BV2yVOLEjxlWvohEi8c/edit?usp=drive_link)
* [technical report] Dana Benedicto. "Flextensions." Data Science Undergraduate Honors Thesis, UC Berkeley. May 2024. [poster](), report available on request
* [proceedings, poster] Jordan Schwartz, Madison Bohannan, Jacob Yim, Yuerou Tang, Dana Benedicto, Charisse Liu, Armando Fox, Lisa Yan, and Narges Norouzi. "Automated Support for Flexible Extensions." In Proceedings of the 55th ACM Technical Symposium on Computer Science Education (SIGCSE), Portland, OR, March 2024. [doi](https://doi.org/10.1145/3626253.3635628), [poster](https://docs.google.com/drawings/d/1fl_hidH4o11INuAQtsWgQE-_g7YbvMUeHJxNQjUUhlU/edit?usp=drive_link)
* [proceedings, poster] Yuerou Tang, Jacob Yim, Jordan Schwartz, Madison Bohannan, Dana Benedicto, Charisse Liu, Armando Fox, Lisa Yan, and Narges Norouzi. "Supporting Mastery Learning with Flexible Extensions." In Proceedings of the 55th ACM Technical Symposium on Computer Science Education (SIGCSE), Portland, OR, March 2024. [doi](https://doi.org/10.1145/3626253.3635615), [poster](https://docs.google.com/drawings/d/1z_uoNy8kQywQ6XC2djNtCmrUxoORkBBnLoCXQO26Gq0/edit?usp=drive_link)
* [talk] Lisa Yan and Michael Ball. Council of College Deans Micro Grant presentation,  UC Berkeley. January 2024. [slides](https://docs.google.com/presentation/d/1QDADS4dZagDvUNSZcdn6OXXACeX_KEXXHv-9gqwcep0/edit?usp=drive_link)
* [technical report] Fuzail Shakir, “Flextensions: Exploring the Impact of Flexible Extensions,” Armando Fox and Dan Garcia, Editors, EECS Department, University of California, Berkeley, Technical Report UCB/EECS-2023-117, May 2023. [report](https://www2.eecs.berkeley.edu/Pubs/TechRpts/2023/EECS-2023-117.html)

# Contact
Lisa Yan and Michael Ball, EECS/Data Faculty
